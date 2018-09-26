---
title: "Technical Details"
excerpt: ""
---
###**API Signatures**

API signatures are computed, using HMAC-SHA1, on the entire JSON body to the request and using the Secret Token of the account (found in Settings->Security) as the key.
The signature is transmitted in the custom header field "x-vvc-hmac" of the HTTP/HTTPS request as a hexadecimal string.

<br>
###**Data Encryption**

Data is encrypted using AES-256 in CBC (cipher-block chaining) mode. The keys used by Vivocha are 96 byte long hexadecimal strings: the first 32 bytes are the Initialisation Vector (IV) and the last 64 bytes are the actual Key. Once converted into binary they correspond to a 128 bit IV and a 256 bit Key.

As chat communications are encrypted message by message, and messages tend to be short and repetitive, Vivocha uses an additional security measure on top of AES to guarantee a much higher protection against cryptanalytic attacks: before encryption, the plaintext is always prepended with 8 random bytes, represented as a 16 byte long hexadecimal string.

Consequently, after decoding a message, the first 16 bytes of the resulting plaintext must be discarded.

The cyphertext is always stored and transmitted Base64-encoded.

###Node.js Sample code
The following Node.js code implements a sample encryption function, compatible with what Vivocha uses:
[block:code]
{
  "codes": [
    {
      "code": "function encrypt(_key, _data) {\n    if (_key.length != (128 + 256) / 8 * 2) throw new Error('invalid_key');\n \n    var iv = new Buffer(_key.substr(0, 128 / 8 * 2), 'hex');\n    var key = new Buffer(_key.substr(128 / 8 * 2), 'hex');\n    var data = crypto.randomBytes(8).toString('hex') + _data;\n \n    var e = crypto.createCipheriv('AES256', key, iv);\n    var c = e.update(data, 'utf8', 'base64');\n    c += e.final('base64');\n    return c;\n}",
      "language": "javascript"
    }
  ]
}
[/block]
The following Node.js code implements a sample decryption function, compatible with what Vivocha uses:
[block:code]
{
  "codes": [
    {
      "code": "function decrypt(_key, data)\n    if (_key.length != (128 + 256) / 8 * 2) throw new Error('invalid_key');\n  \n    var iv = new Buffer(_key.substr(0, 128 / 8 * 2), 'hex');\n    var key = new Buffer(_key.substr(128 / 8 * 2), 'hex');\n  \n    var d = crypto.createDecipheriv('AES256', key, iv);\n    var p = d.update(data, 'base64', 'utf8');\n    p += d.final('utf8');\n    return p;\n}",
      "language": "javascript"
    }
  ]
}
[/block]
<br>
###Browser sample
The following Javascript code implements the same functions using the CryptoJS library. 
Encrypt:
[block:code]
{
  "codes": [
    {
      "code": "function encrypt(_key, _data) {\n    if (_key.length != (128 + 256) / 8 * 2) throw new Error('invalid_key');\n \n    var iv = CryptoJS.enc.Hex.parse(_key.substr(0, 128 / 8 * 2));\n    var key = CryptoJS.enc.Hex.parse(_key.substr(128 / 8 * 2));\n    var data = CryptoJS.lib.WordArray.random(8).toString() + _data;\n \n    return CryptoJS.AES.encrypt(data, key, { iv: iv }).toString();\n};",
      "language": "javascript"
    }
  ]
}
[/block]
Decrypt:
[block:code]
{
  "codes": [
    {
      "code": "function decrypt(_key, _data) {\n    if (_key.length != (128 + 256) / 8 * 2) throw new Error('invalid_key');\n \n    var iv = CryptoJS.enc.Hex.parse(_key.substr(0, 128 / 8 * 2));\n    var key = CryptoJS.enc.Hex.parse(_key.substr(128 / 8 * 2));\n \n    return CryptoJS.AES.decrypt(_data, key, { iv: iv }).toString(CryptoJS.enc.Utf8).slice(16);\n};",
      "language": "javascript"
    }
  ]
}
[/block]
<br>
###**Key Manager API**
Our customers willing to use the External Key Management feature must make a RESTful web service available on the Internet.

The URL specified in the account configuration (Settings-->Security-->External Key Manager URL) is accessed with both GET and POST methods. Vivocha expects posts JSON data and expects JSON responses (Content-Type set to "application/json"). Calls to the External Key Manager are HMAC'ed (see above).

The service must implement three operations:
#### **Create Key**
invoked to request the generation of a new Key, given a Contact Identifier. The storage of a persistent association between the specified Contact ID and the newly generated key is the responsibility of the webservice.
* **Method:**
  * POST
* **Request arguments:**
  * id, identifier of the contact for which the creation of a key is being requested
* **Response arguments:**
  * key, the newly created key, encrypted using the Secret Token according to the algorithm specified in the previous paragraph and encoded in Base64.

####**Copy key**
invoked to request that an existing key associated with a previous Contact be associated with another, specified Contact. This operation is used only when a Contact is transferred between agents: in case of transferred contacts, each leg of the Contact has a different ID, but they must all share the same encryption key.
* **Method:**
  * POST
* **Request arguments:**
  * id, identifier of the contact to which the key should be copied.
  * copyFrom, identifier of the contact from which the key should be copied.
* **Response arguments:**
  * key, the encrypted copied key.

#### **Get Key**
invoked to retrieve a key given a Contact ID. This API is invoked when Vivocha need to decrypt a Contact (e.g. when displaying the transcript of a Contact to a logged in Supervisor/Administrator through the reporting interface). It is left to the webservice to decide whether to provide the key or not, according to customer specific business/security rules.

* **Method:**
  * GET
* **Request arguments:**
  * id, identifier of the contact whose key is being requested
* **Response arguments:**
  * key, the encrypted key.

<br>
Click on the following link to see a published sample of the reference implementation of a compliant webservice : https://github.com/vivocha/keymanager
[block:callout]
{
  "type": "warning",
  "body": "**IMPORTANT: DO NOT USE IT FOR PRODUCTION** (it will always return the same hardcoded key)",
  "title": "Warning"
}
[/block]
If you need any more details on Vivocha Security you find them in [Security Information](doc:security-information)