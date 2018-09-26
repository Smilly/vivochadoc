---
title: SMS Inbound
excerpt: ''
---

# SMS Inbound

[General](sms-inbound.md#section--general-) [Twilio](sms-inbound.md#section--twilio-) [    Phone Number](sms-inbound.md#section--phone-number-) [    Webhook](sms-inbound.md#section--webhook-)   
 \[block:callout\] { "type": "info", "body": "**To configure the SMS Inbound Channel you must have a TWILIO account \(**[https://www.twilio.com/](https://www.twilio.com/)**\) with one or more phone inbound numbers registered to set the Entry Points**" } \[/block\] The SMS Inbound Channel allows users to engage an agent in a contact by sending a message to a Twilio phone inbound number which is associated to one of the Entry Points that can be set for this Channel. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/18996de-Screen\_Shot\_2018-03-29\_at\_12.43.44.png](https://files.readme.io/18996de-Screen_Shot_2018-03-29_at_12.43.44.png)", "Screen Shot 2018-03-29 at 12.43.44.png", 1436, 822, "\#c3bfbd" \], "border": true, "sizing": "80" } \] } \[/block\] You could set more Entry Points, each one is associated to a different Twilio inbound number. Normally they could be used to satisfy different needs by providing different types of customer service.

All the Entry Points set for the SMS Channel are represented by a box reporting information such as the name, the activation flag, a series of icons providing further details and the button  :fa-ellipsis-v:  that give access to the commands to disable it, edit its settings and delete it.

It's also possible to disable all the Entry Points at once selecting the checkbox field. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/8cad392-Screen\_Shot\_2018-03-29\_at\_12.57.52.png](https://files.readme.io/8cad392-Screen_Shot_2018-03-29_at_12.57.52.png)", "Screen Shot 2018-03-29 at 12.57.52.png", 841, 553, "\#f5f5f5" \], "border": true, "sizing": "80" } \] } \[/block\] To add a new SMS Entry Point,click on the **Add new** button in the main card and open the General section

## **General**

The General panel of a SMS Entry Point allows to set the main info such as:

* **info:** every Entry Point must have a name.
* **language:** it can be selected among the ones that are supported in the Campaign. Depending on the set up language you will associate a number among the ones available in twilio account. 
* **state:** The state of the Entry Point determines if it's active or not. Disabling it stops receiving contacts as SMS messages sent to the associated number.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/d1d4681-Screen_Shot_2018-03-29_at_15.53.22.png",
    "Screen Shot 2018-03-29 at 15.53.22.png",
    1382,
    946,
    "#f7f7f7"
  ],
  "border": true,
  "sizing": "80"
  ```

    }

  \]

  }

  \[/block\]

  **Twilio**

  As stated at the beginning of this section, the SMS Inbound Channel in order to define its Entry Points needs to have one or more available phone numbers. These numbers are registered and can be managed within Twilio \([https://www.twilio.com](https://www.twilio.com)\) the popular cloud communications platform that can be integrated with Vivocha.

Users can use these numbers to send SMS messages that agents see exactly like standard contacts, at the same way of the ones coming from the web Channel or requested from a Facebook page. \[block:callout\] { "type": "info", "body": "You can configure the integration between Vivocha and Twilio by following the instructions reported in the section [Settings &gt; Configurations &gt; Telephony](doc:telephony-config).  
\nHere you are asked to provide the **ACCOUNT SID** and **AUTH TOKEN** that are available into your Twilio Profile, then you can connect them to your Vivocha account by clicking the button.  
\nEntry Points set for the SMS Channel inherited these parameters from the settings of the Vivocha account." } \[/block\]

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/07c71b1-Screen\_Shot\_2018-03-29\_at\_16.39.04.png](https://files.readme.io/07c71b1-Screen_Shot_2018-03-29_at_16.39.04.png)", "Screen Shot 2018-03-29 at 16.39.04.png", 900, 764, "\#f7f7f7" \], "border": true, "sizing": "80" } \] } \[/block\]

### **Phone Number**

In this card it's possible associate a Twilio number to the Entry Point: in the dropdown list are shown the ones registered in your Twilio account, with the info whether that numbers is already in use with other Entry Points or not \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/9eb9e1b-Screen\_Shot\_2018-03-29\_at\_17.02.30.png](https://files.readme.io/9eb9e1b-Screen_Shot_2018-03-29_at_17.02.30.png)", "Screen Shot 2018-03-29 at 17.02.30.png", 896, 283, "\#f6f6f6" \], "border": true, "sizing": "80" } \] } \[/block\]

### **Webhook**

Once selected the twilio number a further card appears below showing the webhook special URL generated to allow communication between your Twilio number and Vivocha.

By clicking **Set webhook**, the webhook will be set by us in your Twilio dashboard for the selected number. If the number already has a webhook, the value will be overwritten. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/1fd6cef-Screen\_Shot\_2018-03-30\_at\_12.12.03.png](https://files.readme.io/1fd6cef-Screen_Shot_2018-03-30_at_12.12.03.png)", "Screen Shot 2018-03-30 at 12.12.03.png", 896, 445, "\#f8f8f8" \], "border": true, "sizing": "80" } \] } \[/block\]

