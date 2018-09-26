---
title: "Applications"
excerpt: ""
---
##What is an external application and how to configure it.

An external application is a code that allows you to expand the Vivocha Console's functionality with an unlimited number of features.

For example you can:
* integrate it with your custom CRM software, or with another one such as [Salesforce.com](http://www.salesforce.com).
* automate fetching of your customer's tickets. That's, if you are offering an online help desk, integrate the Vivocha Console with a ticketing system such as [Zendesk](http://www.zendesk.com).
* access the customer's shopping basket for your site, and/or to integrate it with your preferred e-commerce platform such as [hybris](http://www.hybris.com) or [Magento](http://www.magento.com).

These are few little examples, but it is worth noting that the usage of our API is not a strict requirement: **your applications do not have to include our API in order to be loaded by the Vivocha Console**. For example, you can provide access to your internal knowledge base without having to interact with incoming Vivocha contacts: you are just bringing your agent activities together in one place. Of course, it is worth providing i.e. an automatic search of your KB based on customer messages instead letting the agent to do this manually, but this is your choice!

To see all the applications configured in the account, both the Default System ones than the Custom ones,  whether they are enabled or disabled, you simply need to go to the "Applications" section of your "Settings" menu. To configure a new application in the account you simply click on the "New application" button.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d5ed181-applications.png",
        "applications.png",
        1669,
        987,
        "#dfdfdf"
      ],
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
A new panel opens and you can decide if you want create a new custom application or integrate Vivocha with the available Third-Party Applications. To create a custom application click on the corresponding button to add a new module:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d42ab38-applications_new_application.png",
        "applications_new_application.png",
        1669,
        984,
        "#e5e5e5"
      ],
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
One example of a custom application which can be created an administrator is provided by the **Emailer** app which allows to send as email the transcript of a just terminated chat directly to the customer. To start to configure such a app add simply click on the Delivery Service button and follow the instructions in the document **[Email Delivery Service App](doc:emailer)**