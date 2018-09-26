---
title: "Telephony"
excerpt: ""
---
In the Telephony section you can configure the integration between Vivocha and Twilio platform (www.twilio.com) to handle the voice services: Inbound, Outbound and Call Back.

Adding phone numbers is not strictly necessary, in fact you can have no numbers. In this case you can make browser-to-browser (VoIP) and manual calls only.

On this page you can add, edit and delete the phone numbers that are used for your account.

To enable voice services you must have a Twilio account connected to your Vivocha account.

If you already have a Twilio account, you need to copy the **ACCOUNT SID** and **AUTH TOKEN** (see the API Credentials in your Twilio account) in the configuration page then click on the **Connect** button to connect it to your Vivocha account.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/778ab23-Screen_Shot_2017-03-22_at_14.53.21.png",
        "Screen Shot 2017-03-22 at 14.53.21.png",
        1438,
        822,
        "#f2f2f2"
      ],
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
After you have completed the connection, you will see the list of numbers that you have configured previously in your Twilio account.

You can add as many phone numbers you want. If no default phone number for the account is specified, the first one will be the default.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7ac6bf3-Screen_Shot_2017-03-21_at_19.34.01.png",
        "Screen Shot 2017-03-21 at 19.34.01.png",
        1660,
        883,
        "#f2f2f2"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
If you add a new number in your Twilio account, simply click on **Refresh numbers** to update the list of numbers.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5a8967b-refresh_numbers.jpeg",
        "refresh_numbers.jpeg",
        147,
        57,
        "#eef2f1"
      ],
      "border": true
    }
  ]
}
[/block]
By clicking the **Buy a new number** you will go in the Twilio website where you will be able to buy a new twilio number. The numbers purchased can be used for all voice services.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/3f89381-buy_new_numbers.jpeg",
        "buy_new_numbers.jpeg",
        200,
        72,
        "#eff2f1"
      ],
      "border": true
    }
  ]
}
[/block]
By clicking on the **Verify existing number** you will go in the Twilio website to verify an existing phone number (not bought on Twilio). This number will appear on the Customer phone when you make calls for **Outbound** services and for the **Call Back**. You have to enter your phone number and we'll call you to enter a verification code.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b9f16db-verify_existing_numbers.jpeg",
        "verify_existing_numbers.jpeg",
        200,
        60,
        "#eff2f1"
      ],
      "border": true
    }
  ]
}
[/block]
Verified numbers can be associated to each Vivocha user, and **every user can share a common phone number.** Therefore e.g. if a user makes a phone callback, that phone callback will have the specified caller ID.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/c8185a2-Screen_Shot_2017-03-22_at_15.08.33.png",
        "Screen Shot 2017-03-22 at 15.08.33.png",
        1590,
        851,
        "#e2e2e2"
      ],
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
Voice recording: by enabling this feature all phone calls for all voice services will be recorded. The recording of conversation is available in the contact report in each the detail of the contact.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/20031be-Screen_Shot_2017-03-22_at_16.25.07.png",
        "Screen Shot 2017-03-22 at 16.25.07.png",
        330,
        200,
        "#ededec"
      ],
      "border": true
    }
  ]
}
[/block]
When the Voice Recording is activated, you will be able to listen to the recording of the voice call directly into the detail of the contact.
[block:image]
{
  "images": [
    {
      "image": []
    }
  ]
}
[/block]
Disconnect from SID: by clicking on the **Disconnect from SID** button your Vivocha account will be disconnected from your Twilio account. 

If you disconnect your Twilio account the inbound services are disabled.

When you will reconnect your Twilio account, you need to edit and save to re-enable your inbound services.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/f7fad86-Screen_Shot_2017-03-22_at_15.10.24.png",
        "Screen Shot 2017-03-22 at 15.10.24.png",
        212,
        60,
        "#c5765e"
      ],
      "border": true
    }
  ]
}
[/block]
After these steps, if your agent is available on voice media, you can start using [Call Back.](doc:how-to-handle-a-call-back-now) and [Outbound Call](doc:outbound). 

After you have created an [Inbound Telephony Service](https://vivocha.atlassian.net/wiki/display/VVCJ/Inbound+Telephony+Service) the agents will be able to handle [Inbound Calls](doc:inbound-call)