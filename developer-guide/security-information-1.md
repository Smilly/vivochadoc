---
title: Security Information
excerpt: ''
---

# Vivocha Security Features

## **Introduction**

Vivocha is a secure cloud application. This is a bold statement that nevertheless embodies one of the core principles of the platform: we take data security and integrity very seriously.

Vivocha is an online engagement service, and as such conversations between our users and their customers flow through our systems. On top of that we provide a rich set of API that our users can use to create rich applications that store or analyse the messages exchanged between the parties: we make sure that all our customer's data is safe at every endpoint on our platform.

Vivocha Data Security Features consists of:

* **Secure Data Transmission**, how data is transmitted to and from our systems
* **Secure Data Storage**, how data is stored in our systems.
* **End-To-End Encryption**, advanced encryption protocol for the highest level of data safety
* **Key Management**, how encryption keys are managed
* **API Cryptographic Signatures**, message authentication codes on outbound API calls.

## **Secure Data Transmission**

Secure Data Transmission is the basic level of security on Vivocha and it cannot be turned off: all customer data and messages are always transmitted over SSL connections using strong encryption \(at least 256 bytes public keys\). All API calls performed by our users, both using our communication clients and third party integrations, must use HTTPS.

Users connecting to the service via XMPP/Jabber clients must do so over a TLS connection.

Vivocha Mobile SDKs must also connect to the system via SSL/TLS.

Vivocha can send notifications for significant events, including messages exchanged between users and agents, via webhooks that can be dynamically registered using our APIs: we do not mandate these webhooks to be HTTPS services, but if they are, the certificates presented by the remote servers must be valid and signed by trusted Root Certification Authorities.

## **Secure Data Storage**

Messages and customer data are stored for the sole purpose of providing the online engagement features of Vivocha.

Data is stored, for the maximum amount of time which depends on both the billing profile and settings of each customer account. Data is kept only in ISO 27001 certified data centers, validated as Level 1 service providers under the Payment Card Industry \(PCI\) Data Security Standard \(DSS\). Vivocha runs on hardened Linux servers. For more details, see our \[Security Policy\].

For Business accounts \(Solo, Starter and Plus plan subscribers\) the data is stored unencrypted.

For Enterprise accounts the data is stored, by default, strongly encrypted through AES-256, using a different key for each contact \(a contact is any communication session, e.g. a chat, a CallBack, a VoIP call\).

The encryption is, by default, applied at the servers and the encryption keys are stored in a separate database from the actual data.

## **End-To-End Encryption**

Enterprise customers can enable a more advanced encryption protocol, where messages are encrypted and decrypted, using AES-256, directly on the communication clients of the engaging parties \(agents and visitors\). In this case the plaintext is never exposed on the server, and data is stored already encrypted.

This option is available to both web clients and applications using our Mobile SDKs. It is not available, on the agent side, when using third party XMPP clients.

## **Key Management**

When encryption is enabled, each communication session is secured using a different key. Keys are, by default, stored on our systems, in separate databases from the communication data.

For maximum security, our Enterprise customers can opt to use an External Key Manager: in this case, Vivocha neither generates nor stores the encryption keys, delegating these operations to an external secure key manager. The access to the keys is therefore controlled and regulated by our customers, who are also in charge of their storage.

In order to provide this functionality, our customers must implement a web service compliant with our Key Manager API.

The combination of External Key Management and End-To-End Encryption provides an unparalleled level of data security in the industry.

## **API Cryptographic Signatures**

Whenever Vivocha invokes a webhook registered through our APIs, it includes a cryptographic signature using the industry standard HMAC-SHA1. This way our customers can be sure that the request is coming from our systems.

The signature uses the account's secret token, accessible through the Security Settings.   
 \[block:callout\] { "type": "info", "title": "Make sure to check out our other documents on Security:", "body": "If you are wondering what's included in the Security page under Setting in the Vivocha Console you may be interested in: [**Security**](doc:security-config)\n\nIf you want more specific information on Vivocha Security in general look at our [**Security Policy**](doc:security-policy)\n\nIf you're a developer and you need some Technical Information on Vivocha Security you can find it in [**Security - Technical Information**](doc:security-technical-information)" } \[/block\]

