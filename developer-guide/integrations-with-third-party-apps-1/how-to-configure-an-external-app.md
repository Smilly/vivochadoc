---
title: How to Configure an External App
excerpt: ''
---

# How to Configure an External App

## What is an external application?

An external application is a code that allows you to expand the Vivocha Console's functionality with an unlimited number of features.

For example you can:

* integrate it with your custom CRM software, or with another one such as Salesforce.com.
* automate fetching of your customer's tickets. That's, if you are offering an online help desk, integrate the Vivocha Console with a ticketing system such as Zendesk.
* access the customer's shopping basket for your site, and/or to integrate it with your preferred e-commerce platform such as hybris or Magento.

These are few little examples, but it is worth noting that the usage of our API is not a strict requirement: **your applications do not have to include our API in order to be loaded by the Vivocha Console**. For example, you can provide access to your internal knowledge base without having to interact with incoming Vivocha contacts: you are just bringing your agent activities together in one place. Of course, it is worth providing i.e. an automatic search of your KB based on customer messages instead letting the agent to do this manually, but this is your choice!

## How to configure an external application:

To add your application in your Vivocha Console you simply need to go to the "Applications" section of your "Settings" menu: \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/f74bc5a-applications.png](https://files.readme.io/f74bc5a-applications.png)", "applications.png", 1444, 800, "\#dddcdc" \], "border": true, "sizing": "80" } \] } \[/block\] After that click on the "Custom Application" button to add a new module: \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/b2a9d4d-img\_2.png](https://files.readme.io/b2a9d4d-img_2.png)", "img 2.png", 1444, 800, "\#e0dfdf" \] } \] } \[/block\] You can add the custom app in two different ways:

### Vivocha hosted app

Vivocha hosts the application for you: you simply need to write the HTML code in the editor area. To test this we suggest you cut & paste the social app code above. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/11a70a2-img\_3.png](https://files.readme.io/11a70a2-img_3.png)", "img 3.png", 1444, 800, "\#dedcdc" \] } \] } \[/block\]

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/ff4e287-img\_4.png](https://files.readme.io/ff4e287-img_4.png)", "img 4.png", 1444, 800, "\#ced8e5" \] } \] } \[/block\]

### Self hosted app

If you decide to use your own web server or CRM to configure your application you have to insert the public application URL \(please note that this URL must be reachable by the agents\).

As a test you could host the Social Network search application analyzed before \( Social Netwok App \): \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e9f2b0f-img\_5.png](https://files.readme.io/e9f2b0f-img_5.png)", "img 5.png", 1444, 800, "\#dfdfde" \] } \] } \[/block\]

### Save and use your just added application

To save the change you just have to click the save button in the bottom.

All Done!! The integration is complete. To use your new application now you simply need to click on the application icon in the top left corner during a contact.

## Simple Social Network Search application:

This is an example of an HTML application that, when the user provides an e-mail, it will automatically retrieve the user information from the social network: \[block:code\] { "codes": \[ { "code": "&lt;!DOCTYPE html&gt;\n\n\n\n @import url\(http://fonts.googleapis.com/css?family=Ubuntu:700\);\n .content{\n transition: all 0.6s ease 0s;\n -moz-transition: all 0.6s ease 0s;\n -webkit-transition: all 0.6s ease 0s;\n -o-transition: all 0.6s ease 0s;\n color: \#2D4A7F;\n letter-spacing: 0.2em;\n font: normal 18px 'ubuntu';\n text-align: center;\n text-transform: uppercase;\n }\n \n .logo,\n .loading,\n .not\_found{\n width: auto;\n min-width: 500px;\n }\n \n .logo{\n height: auto;\n min-height: 300px;\n position: relative;\n }\n \n .loading{\n height: 40px;\n position: relative;\n }\n \n .not\_found{\n display: none;\n }\n \n\n\n /\*\n \* In order not to waste memory, use our internal\n \* copy of jQuery to bind the document ready event.\n \*/\n VivochaContact.jQuery\(document\).ready\(function\($\) {\n // This function is called when the iframe is fully loaded.\n /\*\n \* Bind the Vivocha Console ready event, which is\n \* triggered when the Vivocha Console has finished all setup\n \* operations and the VivochaContact object is ready.\n \*/\n VivochaContact.ready\(function\(params\) {\n \n var social = 'https://pipl.com/search/?q='; // social search website\n \n retriveInformation\(social\);\n }\);\n }\);\n \n \n \n function retriveInformation\(social\){\n var email = VivochaContact.Utility.searchData\('email'\); // Search email field\n \n if\(email.length &gt; 0\){ // if the function found at least one mail\n window.location = social + email\[0\]; // redirect to pipl with the first mail in the array\n return;\n }\n \n VivochaContact.jQuery\('.loading'\).fadeOut\(function\(\){\n VivochaContact.jQuery\('.not\_found'\).fadeIn\(\);\n }\);\n }\n \n \n\n\n\n\n ![](https://github.com/Smilly/vivochadoc/tree/b817a1941984576e8436f7d5995548bf11c2df0a/Developer%20Guide/Integrations%20with%20Third-Party%20Apps//%22https:/s3.amazonaws.com/vivocha/www/images/vivocha_orange_500.png/%22)\n\n\n retrieving user information\n  
\n ![](https://github.com/Smilly/vivochadoc/tree/b817a1941984576e8436f7d5995548bf11c2df0a/Developer%20Guide/Integrations%20with%20Third-Party%20Apps//%22https:/s3.amazonaws.com/vivocha/www/images/loading.gif/%22)\n\nE Mail not provided\n\n\n", "language": "html", "name": "Social.html" } \] } \[/block\]

