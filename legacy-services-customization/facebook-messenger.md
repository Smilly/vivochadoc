---
title: Facebook Messenger
excerpt: ''
---

# Facebook Messenger

In addition to the other communication channels supported by Vivocha allowing your customers to engage with you online directly on the website, thanks to our new integration with the platform **Facebook Messenger**, they can interact with you using the popular instant messaging interface directly from the Facebook page of your Brand, Company or Organization. This represents a new way through which customers can get in touch with you with a different custom experience and it provides you the possibility to reach a larger audience as well.

Once you have integrated Messenger with our platform following the steps that we are going to explain in this section, your customers are eventually able to use the engagement button on your page on facebook to interact with your agents, who will see the sent messages in the form of a contact appearing on their Agent Desktop, just as it would been created by a normal Vivocha service.

To configure a Facebook Messenger service within Vivocha some operations are needed that integrate the functionalities of this platform with the tools that we provide to create your own customized services. Formally it consists in connecting your Facebook Page with a Vivocha service that you are going to create as well, through a dedicated Facebook Application that essentially works as a bridge between the two parts.

## **1. Use or create a Page**

Use the existing page or create a new one for your Company, Association, brand, ecc... For full instructions, see [**Help Center, How do I create a Page?**](https://www.facebook.com/pages/create) \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/bd4288c-2\_facebook\_create\_page.png](https://files.readme.io/bd4288c-2_facebook_create_page.png)", "2\_facebook\_create\_page.png", 1581, 921, "\#eeedf3" \], "sizing": "full", "border": true, "caption": "Create a page" } \] } \[/block\]

## **2. Create a Facebook App**

To create a Facebook App you need a Facebook developer account to have access to their developer tools. If you don't have it you will need to create one on the page [**Facebok for developers**](https://developers.facebook.com). \[block:callout\] { "type": "info", "body": "To subscribe a Facebook App to a specific web page you must have the **administrator** role for that Page.", "title": "Note" } \[/block\]

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/cef2cf3-1\_facebook\_for\_developers.png](https://files.readme.io/cef2cf3-1_facebook_for_developers.png)", "1\_facebook\_for\_developers.png", 1414, 893, "\#595856" \], "border": true, "sizing": "full", "caption": "Facebook for developers" } \] } \[/block\] Clicking on the **Create App** button a dialog box opens where you can enter the first information to create a new **App ID**:

* The **Name** to associate with this App ID.
* A contact **Email** used for important communication about your app.
* A **Category** to describe the tipology of the app.

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/aefee14-3\_facebook\_create\_app\_ID.png](https://files.readme.io/aefee14-3_facebook_create_app_ID.png)", "3\_facebook\_create\_app\_ID.png", 1618, 896, "\#9d9d9d" \], "border": true, "sizing": "full", "caption": "Create a new App ID" } \] } \[/block\] A security check requires to you to submit a captcha code before generating the App ID. After doing this you will be redirected to the App Dashboard under Product Settings where you need to select "Messenger" for this purpose.

In this example now we have an application we've called _Acme Chat_ and an univocal App ID assigned to it.

Next step consists in select what kind of application/product we want setup. Among the proposed in the list you need add **Messenger**. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/84f3d75-4\_facebook\_select\_product.png](https://files.readme.io/84f3d75-4_facebook_select_product.png)", "4\_facebook\_select\_product.png", 1920, 1080, "\#ebebeb" \], "border": true, "sizing": "full", "caption": "select Messenger for the App" } \] } \[/block\] Facebook Messenger is automatically integrated with every Facebook Page so people can connect directly and easily using the chat to send messages. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/1485370-Schermata\_2017-01-24\_alle\_16.44.58.png](https://files.readme.io/1485370-Schermata_2017-01-24_alle_16.44.58.png)", "Schermata 2017-01-24 alle 16.44.58.png", 1443, 808, "\#e6e6e7" \], "sizing": "full", "border": true, "caption": "Facebook Page, chat and message button" } \] } \[/block\] By connecting this Page to the App that we are configuring the messages sent by customers through Messenger will appear to Agents in the form of a normal contact directly in their Agent Desktop.

Once we added Messenger as product, the next step consists in selecting the Facebook Page that we want to connect to our just created app. In our example we use a page created for this purpose that we have called _Acme Corp_. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/fb49c05-5\_token\_generation.png](https://files.readme.io/fb49c05-5_token_generation.png)", "5\_token\_generation.png", 1920, 1080, "\#ececed" \], "border": true, "sizing": "full", "caption": "Token generation" } \] } \[/block\] You will be asked to grant the required permissions to the app in order to manage the page. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/6dc07b6-media\_availability\_1.009.png](https://files.readme.io/6dc07b6-media_availability_1.009.png)", "media availability 1.009.png", 1920, 1080, "\#415c96" \], "caption": "grant required permissions to the App" } \] } \[/block\] After clicking the ok button a new **Page Access Token** is generated; this means that the app is now connected with the Facebook Page. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e7033a8-Screen\_Shot\_2017-01-19\_at\_16.51.26.png](https://files.readme.io/e7033a8-Screen_Shot_2017-01-19_at_16.51.26.png)", "Screen Shot 2017-01-19 at 16.51.26.png", 1920, 1080, "\#ececed" \], "sizing": "full", "border": true, "caption": "setup the Webhooks" } \] } \[/block\] Once the App has been created and connected to the Facebook Page, now you have to connect it to the Vivocha service which will allow the agents to receive messages sent by customers on facebook, directly in their Agent Desktop as a normal contact that arrives from a service configured on the website.

To start to configure the **Vivocha Messenger Service** you need the following information from the app:

* the **Facebook App ID**
* the **Facebook Secret Key**
* the **Facebook Page Access Token**

While, as we have seen, the Page Access Token is shown on the Product/Messenger settings, you can find the App Id and the Secret Key directly under the Dashboard \(to visualize and copy the Secret Key click on the show button and provide the password of the Facebook account\).

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/180a981-Screen\_Shot\_2017-01-19\_at\_17.58.07.png](https://files.readme.io/180a981-Screen_Shot_2017-01-19_at_17.58.07.png)", "Screen Shot 2017-01-19 at 17.58.07.png", 1920, 1080, "\#ececec" \], "sizing": "full", "border": true, "caption": "Facebook App ID and Secret key" } \] } \[/block\] With these info you can now create a new Vivocha Messenger Servive by going to the Services page on your Vivocha account. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/386411d-6\_Vivocha\_Messemger\_service\_creation.png](https://files.readme.io/386411d-6_Vivocha_Messemger_service_creation.png)", "6\_Vivocha Messemger\_service\_creation.png", 1440, 900, "\#e4e3e3" \], "sizing": "full", "border": true, "caption": "create a Messenger Service" } \] } \[/block\] You need to fill the corresponding fields and configure some other optional information such as the service color ant the list of tags and of the optional tags. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/79f0f15-Screen\_Shot\_2017-01-19\_at\_18.50.57.png](https://files.readme.io/79f0f15-Screen_Shot_2017-01-19_at_18.50.57.png)", "Screen Shot 2017-01-19 at 18.50.57.png", 1920, 1080, "\#e0e0e0" \], "sizing": "full", "border": true, "caption": "setup the Messenger Service" } \] } \[/block\] After you click the save button two new parameters will be provided:

* the **Facebook App Webhook URL**
* the **Verify Token**

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/bde01ac-Screen_Shot_2017-01-19_at_18.51.08.png",
    "Screen Shot 2017-01-19 at 18.51.08.png",
    1920,
    1080,
    "#e0e0e0"
  ],
  "sizing": "full",
  "caption": "Facebook App Webhook URL and Verify Token"
  ```

    }

  \]

  }

  \[/block\]

  These are info that you need to setup the **Webhook** for your Messenger App.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/a4018e9-Screen_Shot_2017-01-19_at_18.52.26.png",
    "Screen Shot 2017-01-19 at 18.52.26.png",
    1920,
    1080,
    "#ebebec"
  ],
  "border": true,
  "sizing": "full",
  "caption": "setup the Webhook"
  ```

    }

  \]

  }

  \[/block\]

  Use the **Facebook app webhook url** and the **verify token** to fill the corresponding fields in the popup window: 

* **Callback URL**
* **Verify Token**

After this you select the subscription fields, representing the webhooks events for which you want to receive updates. You need to check **messages** and **messages\_deliveries** \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e77be67-Screen\_Shot\_2017-01-19\_at\_18.53.13.png](https://files.readme.io/e77be67-Screen_Shot_2017-01-19_at_18.53.13.png)", "Screen Shot 2017-01-19 at 18.53.13.png", 1920, 1080, "\#909091" \], "sizing": "full", "border": true, "caption": "select the Webhook Events" } \] } \[/block\] As last task you need to select the page to subscribe your webhook to the page events. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/a1ab745-Screen\_Shot\_2017-01-19\_at\_18.54.29.png](https://files.readme.io/a1ab745-Screen_Shot_2017-01-19_at_18.54.29.png)", "Screen Shot 2017-01-19 at 18.54.29.png", 1920, 1080, "\#ebebec" \], "border": true, "sizing": "full", "caption": "select the Page to subscribe your Webhook to the Page Events" } \] } \[/block\]

##  **Submit the app for review and wait for approval**

All the operations and steps performed so far are required to setup the Messenger Application that will allow your customers to interact with the agents by sending them messages directly from the subscribed Facebook Page thanks to the fact that it is now connected to a specific service in your Vivocha account.

Until now, actually the app is still under a development mode, therefore the integration just created can work properly only if you have permissions for the app, that means that is necessary a role as **administrator**, or as **developer** or **tester** for using it.

To assign a new role and grant the needed permission for development and test purposes to a user go to the App Dashboard under the Roles section. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/d206040-Screen\_Shot\_2017-01-23\_at\_17.18.48.png](https://files.readme.io/d206040-Screen_Shot_2017-01-23_at_17.18.48.png)", "Screen Shot 2017-01-23 at 17.18.48.png", 1920, 1080, "\#ececed" \], "sizing": "full", "border": true, "caption": "add a developer role to control which people can edit and view the App" } \] } \[/block\] In the whole configuration process this is an important step because otherwise even if the agents are able to receive messages from the Messenger chat in the Facebook Page directly in the Agent Console in the form of contact, they cannot respond to them until they don't have the needed permissions or the app is not available for a public use.

To make the App available to everyone it needs to be released, and to get this it must go through an approval process.

Go the Messenger tab in the App Dashboard. Find the App Review section and select the **pages\_messaging** permission to enable your App to send and receive messages using a Facebook Page. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/8309505-Screen\_Shot\_2017-01-23\_at\_13.17.10.png](https://files.readme.io/8309505-Screen_Shot_2017-01-23_at_13.17.10.png)", "Screen Shot 2017-01-23 at 13.17.10.png", 1920, 1080, "\#ececed" \], "border": true, "sizing": "full", "caption": "select the page\_messaging permission to submit" } \] } \[/block\] After selecting the permission you can edit the notes for it. Click on Edit Notes and be sure to complete each form and any other missing items. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/5bddd97-edit\_notes\_submit\_for\_review.001.png](https://files.readme.io/5bddd97-edit_notes_submit_for_review.001.png)", "edit\_notes\_submit for review.001.png", 1920, 1080, "\#eeeff5" \], "sizing": "full", "caption": "edit notes for the selected permission" } \] } \[/block\] Before clicking Submit for Review you may be asked to set an icon for the App and enter the URL of your Privacy Policy in the corresponding fields under the Settings/basic section of the App Dashboard. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/36444a7-Screen\_Shot\_2017-01-24\_at\_11.17.59.png](https://files.readme.io/36444a7-Screen_Shot_2017-01-24_at_11.17.59.png)", "Screen Shot 2017-01-24 at 11.17.59.png", 1542, 922, "\#4a5262" \], "sizing": "full", "border": true, "caption": "setup the App icon and the Privacy Policy URL" } \] } \[/block\] When you click Submit for Review you are asked to accept the _Facebook Platform Terms and Conditions_, then when your app is approved, a Facebook notification will be sent to you. Also, the App Review section will show the status as approved and now it is possible to make it public and available to all. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/baf610e-Screen\_Shot\_2017-11-15\_at\_17.23.50.png](https://files.readme.io/baf610e-Screen_Shot_2017-11-15_at_17.23.50.png)", "Screen Shot 2017-11-15 at 17.23.50.png", 2452, 1544, "\#4b5362" \], "sizing": "full", "border": true, "caption": "make the App public and available to all" } \] } \[/block\] As already said, once completed the steps to configure your messenger service, agents will be able to answer to the customers who are interacting from the Facebook page as well as they already do for normal contacts.

This is how messenger contacts are visualized in the Agent Desktop. They are characterized by the appearance of the facebook icon beside the name of the customer and also by some other info that are reported in the Customer Info section, directly taken from his facebook profile. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/8d477e9-Screen\_Shot\_2017-01-25\_at\_12.39.49.png](https://files.readme.io/8d477e9-Screen_Shot_2017-01-25_at_12.39.49.png)", "Screen Shot 2017-01-25 at 12.39.49.png", 1440, 900, "\#ebeaea" \], "border": true, "sizing": "full", "caption": "Messenger contacts in the Agent Desktop" } \] } \[/block\]

