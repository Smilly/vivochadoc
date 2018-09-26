---
title: "Security"
excerpt: ""
---
In this section you can find all of the different information needed for your Vivocha Security.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5c99926-Screen_Shot_2017-03-21_at_19.51.26.png",
        "Screen Shot 2017-03-21 at 19.51.26.png",
        1919,
        1007,
        "#f3f3f3"
      ]
    }
  ]
}
[/block]
##Password policy
You can now set several parameters for your password policy, that will apply to all the new accounts users being created or edited from that moment on. You can set the followings:
* password maximum length
* forbid user id within password field
* lowercase letter
* uppercase letter
* digit
* special character

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8459353-Screen_Shot_2015-10-06_at_16.08.00.png",
        "Screen Shot 2015-10-06 at 16.08.00.png",
        881,
        205,
        "#f9f9f9"
      ],
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
When creating a new user in the User Editor, a popup will inform you of the set requirements for the new password to be set.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/1a91a4a-Screen_Shot_2017-03-22_at_17.43.55.png",
        "Screen Shot 2017-03-22 at 17.43.55.png",
        1020,
        570,
        "#e2e0de"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
##Privacy
The privacy settings section is made up of the following fields:

**Unique visitor cookie duration** 
This cookie is used to identify a unique user, modifying the duration of this cookie will change the number of unique visitors in the reports and in the creation of a contact. This cookie is renewed for every visited page or Vivocha action (such as a contact or a message sent) this means that the cookie expiration time starts from the last customer action.

**Visit cookie duration** 
This cookie is used to identify the visit in your site, modifying the duration of this cookie will change the number of visits generated in your website in the Vivocha reports. This cookie is renewed for every visited page or Vivocha action (such as a contact or a message sent) that means that the visit ends when the cookie duration is reached without any activity on your site by the user.

**Disable contact geolocalization features** 
This disable the functionality that allows to save the visitor's IP address and to obtain from it all the geolocalisation info that are shown to agents during the contact and in its detail report (such as city, state, map in the customer info app). 

**Disable Agent Console on iframe**
This option enabled prevents the possibilty to open an embedded version of the agent console directly in a new window/iframe.

**Formsharing forms selection**
It's possible to decide which are the forms in the page to be shared with the agents
* **All Compliants forms:** all the forms that are in the page 
* **Only selected (by vvc_form_enabled class):** only the form that have assigned with the specific class *vvc_form_enabled*

**Formsharing fields selection**
It's also possible to decide which are the form fields in the page to be shared with the agents
* **All Compliants form fields:** all the form fields that are in the page 
* **Only selected (by vvc_form_enabled class):** only the form fields that have assigned with the specific class *vvc_form_enabled*

**Share fields readonly mode if not explicitly enabled**
if you enable this option the elements are shared in the readonly mode
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/e2e38bf-Screen_Shot_2017-03-22_at_17.47.05.png",
        "Screen Shot 2017-03-22 at 17.47.05.png",
        424,
        582,
        "#f7f7f7"
      ],
      "border": true
    }
  ]
}
[/block]
##Encryption
The encryption settings section is made up of the following fields:

**Secret Token** 
used to compute API signatures and used to encrypt/decrypt keys when using the Key Manager API
[block:callout]
{
  "type": "warning",
  "body": "the secret token is available only for the account owner.",
  "title": "Info"
}
[/block]
**Chat Encryption** 
The encryption of the chat transcripts (exchanged messages) can be set to Transmission Only (basic security, all traffic uses HTTPS/SSL/TLS), Transmission & Storage (data is encrypted by the servers before storage) and End-To-End (data is encrypted directly by the clients and is stored already encrypted)

**Data Collection Encryption** 
Encryption of the data collected before and during a contact (includes data entered by the visitors on data collection forms, data attached to the contact via API and data edited by the agent)

**Key Manager**
Set the Key Manager to Internal (the default) or External

**Key Manager URL** 
The URL of the customer supplied Key Manager, when the Key Manager mode is External. Keys are always transmitted encrypted with the secret token, even when using HTTP. Nevertheless, for better protection, we strongly advise to use only HTTPS URLs.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/736b89e-Screen_Shot_2017-03-22_at_17.57.41.png",
        "Screen Shot 2017-03-22 at 17.57.41.png",
        972,
        540,
        "#f4f4f4"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
##Access restriction
It is now possible to restrict the access to the Vivocha console by defining a range of authorised IP addresses, using the CIDR-v4 format.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d34b209-Screen_Shot_2017-03-24_at_18.53.45.png",
        "Screen Shot 2017-03-24 at 18.53.45.png",
        912,
        387,
        "#f9f9f9"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]