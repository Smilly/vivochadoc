---
title: Web Entry Points
excerpt: ''
---

# Web Entry Points

[General](web-entry-points.md#section--general-) [Web Pages](web-entry-points.md#section--web-pages-) [Languages](web-entry-points.md#section--languages-) [Advanced](web-entry-points.md#section--advanced-)

An Entry Point is where the contacts are requested from; for the web Channel it is basically the webpages of a website.

A Campaign published on the web must have at least a configured web Entry Point with an associated Engagement Widget to start a contact.

To add a new web Entry Point, that is a website and its webpages, click on the **Add new** button in the main card. It will opens the [General](doc:vcb-web-entry-points#section-general) section to set main settings of this web Entry Point. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/f146353-WEB-Entry\_point\_empty-2.png](https://files.readme.io/f146353-WEB-Entry_point_empty-2.png)", "WEB-Entry point empty-2.png", 839, 484, "\#f5f5f5" \], "border": true, "sizing": "80" } \] } \[/block\] It's also possible to disable all the web Entry Points in the Channel selecting the checkbox field. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e3246b5-WEB-Entry\_point\_disabled-2.png](https://files.readme.io/e3246b5-WEB-Entry_point_disabled-2.png)", "WEB-Entry point disabled-2.png", 840, 581, "\#f6f5f5" \], "border": true, "sizing": "80" } \] } \[/block\] The web Entry Points section presents all the configured websites/webpages in the Campaign. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/d36b4c0-WEB-entry\_points\_list-4.png](https://files.readme.io/d36b4c0-WEB-entry_points_list-4.png)", "WEB-entry points list-4.png", 779, 215, "\#f2f2f2" \], "sizing": "80", "border": true } \] } \[/block\] Each one is represented by a box reporting information such as the name, the activation flag, a series of icons providing further details and the button  :fa-ellipsis-v:  that give access to the commands to disable it, edit its settings and delete it.

The table reports icons that can be displayed for each configured web Entry Point box and what they represent. \[block:parameters\] { "data": { "0-0": ":fa-unlock:", "1-0": ":fa-lock:", "0-1": "No page restriction", "1-1": "Website with page restriction", "h-0": "Icon", "h-1": "Meaning", "2-0": ":fa-language:", "2-1": "language detection strategies enabled" }, "cols": 2, "rows": 3 } \[/block\] By clicking on the name in the box the web Entry Point configuration panel opens.

## **General**

The General panel of a web Entry Point allows to set the name of it and its state.

The state of the Entry Point determines if it's active or not. Disabling a web Entry Point stops receiving contacts from a website and its pages. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/67e47e0-WEB-Entry\_point\_General\_-2.png](https://files.readme.io/67e47e0-WEB-Entry_point_General_-2.png)", "WEB-Entry point General -2.png", 842, 759, "\#f6f6f6" \], "sizing": "80", "border": true } \] } \[/block\] At the bottom of the page a button let you to go back to the main section with the list of all web Entry Points.

## **Web pages**

Engagement Widgets associated to the web Entry Point will be displayed to all users that visit a site which contains the [**Vivocha script**](doc:settings).

It is possible to identify specific sections of a website where you want to show the Engagement Widget and other where you do not want. You can explicitly include or exclude web pages or domains specifying the whole paths or by setting a filter to define a pattern used to match against these paths.

So, for example you can include all the pages under a specific domain and at the same time add a new rule to exclude only the ones that match with a specific path or that contain a particular word. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e01da54-WEB-Entry\_point\_web\_pages-3.png](https://files.readme.io/e01da54-WEB-Entry_point_web_pages-3.png)", "WEB-Entry point web pages-3.png", 1323, 929, "\#f8f7f7" \], "sizing": "80" } \] } \[/block\] The available filters allow to define rules that verify if a web page or a domain is **equal** to a specific path or it  **starts**, **ends**, **contains** a particular word or string or further, if it **matches** against with a regular expression.

A web Entry Point configured with pages restrictions shows the icon  :fa-lock:  in the box that represents it in the list. On the other hand if there're not web pages restrictions the icon shown is  :fa-unlock: 

You can remove a web pages rule by clicking the corresponding  :fa-trash:  button

## **Languages**

When a web Entry Point is created it gets the default language set for the Campaign. **Languages** section in the General settings allows to add as many languages as you want to support in the Campaign and to select the one that must be used by default. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/cbef8b7-WEB-Entry\_point\_languages-7.png](https://files.readme.io/cbef8b7-WEB-Entry_point_languages-7.png)", "WEB-Entry point languages-7.png", 844, 483, "\#f3f3f3" \], "border": true, "sizing": "80" } \] } \[/block\] If you choose to use the predefined language, all widgets displayed in this web Entry Point will use that language.

Alternatively you can automatically detect the best language for the users by defining one or more **Language Detection Strategies** by selecting them from the dropdown list and clicking the add button. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/bfd26a4-WEB-Entry\_point\_languages-8.png](https://files.readme.io/bfd26a4-WEB-Entry_point_languages-8.png)", "WEB-Entry point languages-8.png", 841, 760, "\#f5f5f5" \], "sizing": "80", "border": true } \] } \[/block\] Language Detection Strategies will be evaluated in order until a match is found.

You can remove a strategy by clicking the corresponding  :fa-trash:  button \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/77ba508-WEB-Entry\_point\_languages-9.png](https://files.readme.io/77ba508-WEB-Entry_point_languages-9.png)", "WEB-Entry point languages-9.png", 906, 767, "\#f7f7f7" \], "border": true, "sizing": "80" } \] } \[/block\] Strategies are based on:

### **Domain**

This strategy is based on the recognizing of the country code top-level domain \(ccTLD\) encoded in the name of the website.

### **User-agent**

This strategy is based on the recognizing of the User-Agent of the customer's browser.

### **GEOIP**

It's based on the geolacalization of the IP address of the device used by the visitor of the website.

### **URL**

It checks if in the URL is present a language code, for example:

* www.mysite.com/l/**en**/sales/privatearea 
* www.mysite.com/l/**ch-it**/sales/mobile

### **Custom Javascript Code**

You can write a custom javascript code to implement a strategy that detects the proper language from an external web service or from a variable with a value assigned from a specific logic. By selecting this strategy the card expands showing the inline code editor where you can write down the code implementing this logic. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/5096a12-WEB-Entry\_point\_languages-5.png](https://files.readme.io/5096a12-WEB-Entry_point_languages-5.png)", "WEB-Entry point languages-5.png", 896, 765, "\#c9c9c9" \], "sizing": "80", "border": true } \] } \[/block\]

## **Advanced**

One of the key concept of the Campaign Builder is that it allows to implement the granularity for the most of the configurations that you can set in a Campaign.

A Campaign groups together a set of configurations so that it is not necessary to define these in more points, unless it's not requested to have a different behaviour in the various Channels within the same Campaign, or even if you want to apply different rules to the different Engagements within the same Channel.

The Advanced panel provides the opportunity to redefine, at the web Entry Point level, some of these configurations that are inherited from directly the Campaign. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/f3966d9-WEB-EP-Advanced\_2.png](https://files.readme.io/f3966d9-WEB-EP-Advanced_2.png)", "WEB-EP-Advanced 2.png", 842, 541, "\#f5f5f5" \], "border": true, "sizing": "80" } \] } \[/block\] From the dropdown you can select the configurations you may want redefine and for each of the options the interface is dynamically loaded providing the possibility to differentiate the settings. \[block:callout\] { "type": "info", "body": "By selecting one of the available options from the dropdown list the relative configuration area opens and display these settings inherited from the higher level." } \[/block\] Any eventual changes that have overwritten the inherited settings can be removed by clicking the big red button that is shown in the new card that appears just below.

The configurations that you are able to redefine for a web Entry Point are relative to:

* [Media](doc:vcb-media)
* [Business Hours](doc:vcb-general#section--business-hours-)
* [Routing/ Tags and Color](doc:vcb-routing#section-tags-and-color)
* [Routing/Pause](doc:vcb-routing#section-pause)
* [Routing/Transfer](doc:vcb-routing#section-transfer)
* [Routing/Rules](doc:vcb-routing#section-routing-rules)

So for a particular web Entry Point you may want to disable the media voice and also enable the video only on the Agent side. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/0b99d6e-WEB-EP\_-Advanced\_3.png](https://files.readme.io/0b99d6e-WEB-EP_-Advanced_3.png)", "WEB-EP -Advanced 3.png", 1380, 929, "\#f8f3f3" \], "border": true, "sizing": "80" } \] } \[/block\] Also you might want to reschedule the business hours for the single web Entry Points set into a Campaign, in order to apply to them diversified working times. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/bec1079-WEB-EP-Advanced\_4.png](https://files.readme.io/bec1079-WEB-EP-Advanced_4.png)", "WEB-EP-Advanced 4.png", 1380, 944, "\#f9f4f4" \], "border": true, "sizing": "80" } \] } \[/block\]

