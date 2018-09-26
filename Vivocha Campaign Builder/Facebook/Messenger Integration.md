---
title: "Messenger Integration"
excerpt: ""
---
[Use or create a Page](#section--use-or-create-a-page-)
[Create a Facebook App](#section--create-a-facebook-app-)
[&nbsp;&nbsp;&nbsp;&nbsp;Create a New App ID](#section--create-a-new-app-id-)
[&nbsp;&nbsp;&nbsp;&nbsp;Messenger platform integration](#section--messenger-platform-integration-)
[&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Connect the Page to the App and get the Page Access Token](#section--connect-the-page-to-the-app-and-get-the-page-access-token-)
[&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Configure the Facebook page in the campaign Builder](#section--configure-the-facebook-page-in-the-campaign-builder-)
[&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Webhooks Setup](#section--webhooks-setup-)
[&nbsp;&nbsp;&nbsp;&nbsp;Submit the app for review and wait for approval*](#section--submit-the-app-for-review-and-wait-for-approval-)
<br>



To configure the Facebook Messenger service it's necessary to carry out some operations that integrate the functionalities of this platform with the tools that we provide in the Campaign Builder.

Formally they allow to connect your Facebook Page added as Entry Point in the Campaign, through a dedicated Facebook Application that essentially works as a bridge between the two parts.

Below are the required steps: 

#**Use or create a Page**
Use the existing page or create a new one for your Company, Association, brand, ecc... For full instructions, see **[Help Center, How do I create a Page?](https://www.facebook.com/pages/create)**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/bd4288c-2_facebook_create_page.png",
        "2_facebook_create_page.png",
        1581,
        921,
        "#eeedf3"
      ],
      "sizing": "80",
      "border": true,
      "caption": "Create a page"
    }
  ]
}
[/block]
#**2. Create a Facebook App**
To create a Facebook App you need a Facebook developer account to have access to their developer tools. If you don't have it you will need to create one on the page **[Facebok for developers](https://developers.facebook.com)**.
[block:callout]
{
  "type": "info",
  "body": "To subscribe a Facebook App to a specific web page you must have the **administrator** role for that Page.",
  "title": "Note"
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/c8c7f9c-FB-Create_app.png",
        "FB-Create app.png",
        1436,
        823,
        "#b5b6b5"
      ],
      "border": true,
      "sizing": "80",
      "caption": "Facebook for developers"
    }
  ]
}
[/block]
##**Create a New App ID**
By moving with the mouse pointer over the **My Apps** in the topbar a menu is shown and by clicking on it you have access to all the apps configured for the account.

By clicking on **"+ Add a New App"** button a dialog box opens where you can enter the first information to create a **New App ID**:

* The **Name** to associate with this App ID. 
* A contact **Email** used for important communication about your app.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2c8a5ba-FB-apps-2.png",
        "FB-apps-2.png",
        1439,
        823,
        "#7a7c7e"
      ],
      "border": true,
      "sizing": "80",
      "caption": "Create a new App ID"
    }
  ]
}
[/block]
A security check requires to you to submit a captcha code before generating the App ID. After doing this you will be redirected to the App Dashboard where you need to select "Messenger" for this purpose. 

In this example now we have an application we've called *Acme Chat* and an univocal App ID assigned to it.

##**Messenger platform integration**
Next step consists in select what kind of application/product we want setup. Among the proposed in the list you need add **Messenger**. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/78776f5-FB-new-app.png",
        "FB-new-app.png",
        1437,
        818,
        "#e8eaeb"
      ],
      "border": true,
      "sizing": "80",
      "caption": "select Messenger for the App"
    }
  ]
}
[/block]
###**Connect the Page to the App and get the Page Access Token**
Facebook Messenger is automatically integrated with every Facebook Page so people can connect directly and easily using the chat to send messages.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/1485370-Schermata_2017-01-24_alle_16.44.58.png",
        "Schermata 2017-01-24 alle 16.44.58.png",
        1443,
        808,
        "#e6e6e7"
      ],
      "sizing": "80",
      "border": true,
      "caption": "Facebook Page, chat and message button"
    }
  ]
}
[/block]
By connecting this Page to the App that we are configuring the messages sent by customers through Messenger will appear to Agents in the form of a normal contact directly in their Agent Desktop.

Once we added Messenger as product, the next step consists in selecting the Facebook Page that we want to connect to our just created app. In our example we use a page created for this purpose that we have called *Acme Corp*.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/12814a5-FB-Product_Messenger.png",
        "FB-Product Messenger.png",
        1917,
        1000,
        "#e8eaed"
      ],
      "border": true,
      "sizing": "80",
      "caption": "Token generation"
    }
  ]
}
[/block]
You will be asked to grant the required permissions to the app in order to manage the page. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/6dc07b6-media_availability_1.009.png",
        "media availability 1.009.png",
        1920,
        1080,
        "#415c96"
      ],
      "caption": "grant required permissions to the App",
      "sizing": "80"
    }
  ]
}
[/block]
After clicking the ok button a new **Page Access Token** is generated; this means that the app is now connected with the Facebook Page.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/4a57507-FB-Page_Access_Token.png",
        "FB-Page Access Token.png",
        1918,
        958,
        "#eff0f1"
      ],
      "sizing": "80",
      "border": true,
      "caption": "Page Access Token"
    }
  ]
}
[/block]
###**Configure the Facebook page in the campaign Builder**
Once the App has been created and connected to the Facebook Page, now you have to connect to its equivalent Entry Point set in the Campaign, which will allow the agents to receive messages sent by customers on facebook, directly in their Agent Desktop as a normal contact that arrives from a service configured on the website. 

For this purpose yu need the following information from the app:

* the **Facebook App ID**
* the **Facebook Secret Key**
* the **Facebook Page Access Token**

While, as we have seen, the Page Access Token is shown on the Product/Messenger settings as shown in the previous image, you can find the App Id and the Secret Key directly under the Settings > Basics panel that you can access from the left navigation menu (to visualize and copy the Secret Key click on the show button and provide the password of the Facebook account in use).
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/21d1a8a-FB-Settings_basics.png",
        "FB-Settings_basics.png",
        1269,
        790,
        "#eaebed"
      ],
      "sizing": "80",
      "border": true,
      "caption": "Facebook App ID and Secret key"
    }
  ]
}
[/block]
Once you have got them, you can now set these parameters in the Messenger panel of the Facebook page set in the Campaign Builder.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8737b82-VCB-FB-App_parameters.png",
        "VCB-FB-App parameters.png",
        1320,
        940,
        "#fafafa"
      ],
      "sizing": "80",
      "border": true,
      "caption": "set the App ID, Secret Key and the Page Access Token"
    }
  ]
}
[/block]
###**Webhooks Setup**
Next step is to set the other two parameters that are automatically generated when clicking on the **Get Webhook** button and that are displayed in the Webhook card at the top of this panel.

* the **Webhook URL**
* the **Verify Token**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/a6aaf4e-VCB-FB-webhook_2.png",
        "VCB-FB-webhook 2.png",
        1322,
        425,
        "#f6f6f6"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
Go back to the Facebook App in the Messenger > Settings section where you will enable the webhooks integration to receive messages and other events sent by Messenger users.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/419357c-FB-setup_webhook.png",
        "FB-setup webhook.png",
        1435,
        822,
        "#ebedee"
      ],
      "border": true,
      "sizing": "80",
      "caption": "setup the webhooks integration"
    }
  ]
}
[/block]
Use the **Webhook url** and the **verify token** parameters shown above, that you can also easily copy in the clipboard by clicking on , to fill the corresponding fields in the popup window: 
* **Callback URL**
* **Verify Token**

Also you select the subscription fields, representing the webhooks events for which you want to receive updates. You need to check **messages** and **messages_deliveries**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2e657c1-FB-setup_webhook_2.png",
        "FB-setup webhook 2.png",
        1435,
        823,
        "#aeafb0"
      ],
      "sizing": "80",
      "border": true,
      "caption": "select the Webhook Events"
    }
  ]
}
[/block]
As last task you need to select the page to subscribe your webhook to the page events. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/280a9f5-Screen_Shot_2018-03-16_at_10.40.44.png",
        "Screen Shot 2018-03-16 at 10.40.44.png",
        1917,
        991,
        "#e9ecee"
      ],
      "border": true,
      "sizing": "80",
      "caption": "select the Page to subscribe your Webhook to the Page Events"
    }
  ]
}
[/block]
##** Submit the app for review and wait for approval**
All the operations and steps performed so far are required to setup the Messenger Application that will allow your customers to interact with the agents by sending them messages directly from the subscribed Facebook Page thanks to the fact that it is now connected to a specific service in your Vivocha account.
 
Until now, actually the app is still under a development mode, therefore the integration just created can work properly only if you have permissions for the app, that means that is necessary a role as **administrator**, or as **developer** or **tester** for using it.

To assign a new role and grant the needed permission for development and test purposes to a user go to the App Dashboard under the Roles section.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/98e3b4d-Screen_Shot_2018-03-16_at_12.00.20.png",
        "Screen Shot 2018-03-16 at 12.00.20.png",
        1917,
        1002,
        "#e9ebed"
      ],
      "sizing": "80",
      "border": true,
      "caption": "add a developer role to control which people can edit and view the App"
    }
  ]
}
[/block]
In the whole configuration process this is an important step because otherwise even if the agents are able to receive messages from the Messenger chat in the Facebook Page directly in the Agent Console in the form of contact, they cannot respond to them until they don't have the needed permissions or the app is not available for a public use.

To make the App available to everyone it needs to be released, and to get this it must go through an approval process. 

Go the Messenger tab in the App Dashboard. Find the App Review section and select the **pages_messaging** permission to enable your App to send and receive messages using a Facebook Page.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/a900f1b-Screen_Shot_2018-03-16_at_10.48.39.png",
        "Screen Shot 2018-03-16 at 10.48.39.png",
        1917,
        977,
        "#e9ebed"
      ],
      "border": true,
      "sizing": "80",
      "caption": "select the page_messaging permission to submit"
    }
  ]
}
[/block]
After selecting the permission you can edit the notes for it. Click on Edit Notes and be sure to complete each form and any other missing items.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/f5421ff-Screen_Shot_2018-03-16_at_11.02.33.png",
        "Screen Shot 2018-03-16 at 11.02.33.png",
        848,
        739,
        "#f7f7f8"
      ],
      "sizing": "80",
      "caption": "edit notes for the selected permission",
      "border": true
    }
  ]
}
[/block]
Before clicking Submit for Review you may be asked to set an icon for the App and enter the URL of your Privacy Policy  in the corresponding fields under the Settings/basic section of the App Dashboard. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/6d3929d-Screen_Shot_2018-03-16_at_11.51.07.png",
        "Screen Shot 2018-03-16 at 11.51.07.png",
        1919,
        999,
        "#e7e9ec"
      ],
      "sizing": "80",
      "border": true,
      "caption": "setup the App icon and the Privacy Policy URL"
    }
  ]
}
[/block]
When you click Submit for Review you are asked to accept the *Facebook Platform Terms and Conditions*, then when your app is approved, a Facebook notification will be sent to you. Also, the App Review section will show the status as approved and now it is possible to make it public and available to all.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/baf610e-Screen_Shot_2017-11-15_at_17.23.50.png",
        "Screen Shot 2017-11-15 at 17.23.50.png",
        2452,
        1544,
        "#4b5362"
      ],
      "sizing": "80",
      "border": true,
      "caption": "make the App public and available to all"
    }
  ]
}
[/block]
As already said, once completed the steps to configure your messenger service, agents will be able to answer to the customers who are interacting from the Facebook page as well as they already do for normal contacts. 

This is how messenger contacts are visualized in the Agent Desktop. They are characterized by the appearance of the facebook icon beside the name of the customer and also by some other info that are reported in the Customer Info section, directly taken from his facebook profile.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8d477e9-Screen_Shot_2017-01-25_at_12.39.49.png",
        "Screen Shot 2017-01-25 at 12.39.49.png",
        1440,
        900,
        "#ebeaea"
      ],
      "border": true,
      "sizing": "80",
      "caption": "Messenger contacts in the Agent Desktop"
    }
  ]
}
[/block]