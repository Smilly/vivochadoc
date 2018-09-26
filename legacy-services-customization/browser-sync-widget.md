---
title: Browser Sync Widget
excerpt: ''
---

# Browser Sync Widget

To allow operators monitoring and provide online support also to customers who don’t start a contact from the web but by phone, we implemented the browser sync, that is a sharing session bootable by a pin.

## Quick start integration

The agent have only to share with the customer the pin generated by the system and ask him to paste at the and of the page URL he is visiting at the moment. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e96069d-Screen\_Shot\_2016-06-23\_at\_18.55.08.png](https://files.readme.io/e96069d-Screen_Shot_2016-06-23_at_18.55.08.png)", "Screen Shot 2016-06-23 at 18.55.08.png", 1280, 935, "\#ddddda" \], "caption": "Notice the \# with the PIN at the end of the URL" } \] } \[/block\]

## Integrated mode

The customer will get a window that asks him to agree for starting the sharing session.

Taken the agreement, the agent will be able to give the support and the customer could be able to end the sharing session whenever he wants. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/d528ce1-Screen\_Shot\_2016-06-23\_at\_19.04.07.png](https://files.readme.io/d528ce1-Screen_Shot_2016-06-23_at_19.04.07.png)", "Screen Shot 2016-06-23 at 19.04.07.png", 1280, 936, "\#3d3d49" \], "caption": "The user has to insert manually the pin in page" } \] } \[/block\]

## Integration example

Here you can see a complete example that shows how to integrate a browser sync widget and handle contact sync.

The example page will ideally show 2 small boxes: \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/4e70196-Schermata\_2016-09-08\_alle\_12.29.53.png](https://files.readme.io/4e70196-Schermata_2016-09-08_alle_12.29.53.png)", "Schermata 2016-09-08 alle 12.29.53.png", 435, 452, "\#e8e8e8" \], "caption": "the first box: the user has to insert the sharing code received from the agent in order to start a sharing session" } \] } \[/block\]

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/f4eee7b-Schermata\_2016-09-08\_alle\_12.33.20.png](https://files.readme.io/f4eee7b-Schermata_2016-09-08_alle_12.33.20.png)", "Schermata 2016-09-08 alle 12.33.20.png", 162, 244, "\#ebebea" \], "caption": "Control box that will appear when the session starts" } \] } \[/block\] This example uses the following Vivocha apis:

* [vivocha.syncContact](https://m1.vivocha.com/a/_/api/doc/VivochaVisitor.html#.syncContact) that syncs the contact using the sharing code
* [vivocha.events.on](https://m1.vivocha.com/a/_/api/doc/VivochaVisitor.html#.events) for handle the **contactSync** event that will occur when the page is loaded with an existing synced contact

Don't forget you can check the Javascript SDK documentation [HERE](https://m1.vivocha.com/a/_/api/doc/). \[block:code\] { "codes": \[ { "code": "\n.vvc\_box {\n background-color: \#efefef;\n border: \#e4e4e4 2px solid;\n border-radius: 4pt;\n}\n\#vvc\_tools {\n display: none;\n width: 66px;\n height: 108px;\n}\n\#vvc\_tools i {\n display: block;\n margin: 32px 22px;\n width: 22px;\n height: 22px;\n cursor: pointer;\n}\n\#vvc\_tools i:first-child {\n margin-top: 16px;\n}\n\#vvc\_tools i:last-child {\n margin-bottom: 16px;\n}\n\#vvc\_tools i\#vvc\_btn\_sharing {\n background: url\(\"&lt;a href="http://d3btqb6knwd3a4.cloudfront.net/a/templates/media/share-grey.png\\"&gt;http://d3btqb6knwd3a4.cloudfront.net/a/templates/media/share-grey.png\&lt;/a&gt;"\) center/100% 100%;\n}\n\#vvc\_tools i\#vvc\_btn\_sharing.vvc\_btn\_on {\n background: url\(\"&lt;a href="http://d3btqb6knwd3a4.cloudfront.net/a/templates/media/share-green.png\\"&gt;http://d3btqb6knwd3a4.cloudfront.net/a/templates/media/share-green.png\&lt;/a&gt;"\) center/100% 100%;\n}\n\#vvc\_tools i\#vvc\_btn\_close {\n background: url\(\"&lt;a href="http://d3btqb6knwd3a4.cloudfront.net/a/templates/media/close-red.png\\"&gt;http://d3btqb6knwd3a4.cloudfront.net/a/templates/media/close-red.png\&lt;/a&gt;"\) center/100% 100%;\n}\n\#vvc\_sharing {\n display: none;\n width: 160px;\n /&lt;em&gt;height: 172px;&lt;/em&gt;/\n padding: 20px;\n\n color: \#555;\n font-size: 13px;\n line-height: 1.2em;\n font-family: arial;\n}\n\#vvc\_sharing h3 {\n margin-top: 0;\n}\n\#vvc\_sharing h6 {\n display: none;\n margin: 0;\n color: \#df585c;\n}\n\#vvc\_sharing input {\n width: 100%;\n}\n\#vvc\_sharing button {\n margin-top: 16px;\n border-top: 0;\n border-left: 0;\n border-right: 0;\n font-size: 12px;\n border-radius: 4pt;\n padding: 6px 12px;\n text-transform: uppercase;\n font-weight: bold;\n text-align: center;\n font-family: 'Open sans',arial,sans-serif;\n -moz-transition: background .2s linear;\n transition: background .2s linear;\n position: relative;\n}\n\#vvc\_sharing button.vvc\_btn\_on {\n background: \#80bc7a;\n border-bottom: 2px solid green;\n color: \#f8f8f8;\n}\n\n\n \n \n\n\n\n \n vivocha.ready\(function \(\) {\n function toggleCodeBox\(\) {\n vivocha.$\('\#vvc\_sharing'\).toggle\(\);\n vivocha.$\('\#vvc\_sharing\_code'\).val\(''\);\n };\n vivocha.$\('h1, \#vvc\_sharing button:not\(.vvc\_btn\_on\)'\).on\(\"click\", function \(\) {\n toggleCodeBox\(\);\n }\);\n vivocha.$\('\#vvc\_sharing button.vvc\_btn\_on'\).click\(function \(\) {\n var syncid = vivocha.$\('\#vvc\_sharing\_code'\).val\(\);\n if \(syncid\) {\n vivocha.syncContact\(syncid, {}, function \(err, res\) {\n if \(err\) {\n console.error\(err\);\n vivocha.$\('\#vvc\_sharing h6'\).show\(\);\n }\n else {\n toggleCodeBox\(\);\n vivocha.$\('\#vvc\_tools'\).toggle\(\);\n vivocha.$\('\#vvc\_btn\_sharing'\).addClass\('vvc\_btn\_on'\);\n vivocha.contact.on\('left', function \(\) {\n vivocha.$\('\#vvc\_btn\_sharing'\).removeClass\('vvc\_btn\_on'\);\n vivocha.contact.leave\(\);\n }\);\n }\n }\);\n }\n else {\n console.error\('undefined syncid'\);\n vivocha.$\('\#vvc\_sharing h6'\).show\(\);\n }\n }\)\n vivocha.$\('\#vvc\_btn\_close'\).click\(function \(\) {\n vivocha.contact.leave\(\);\n vivocha.$\('\#vvc\_tools'\).toggle\(\);\n }\);\n\t\t\t vivocha.events.on\('contactSync', function\(err, ev\){\n\t\t\t \tif\(vivocha.$\('\#vvc\_sharing:visible'\).size\(\) &gt; 0\) {\n\t\t\t \t\ttoggleCodeBox\(\);\n\t\t\t \t}\n\t\t\t vivocha.$\('\#vvc\_tools'\).toggle\(\);\n\t\t\t vivocha.$\('\#vvc\_btn\_sharing'\).addClass\('vvc\_btn\_on'\);\n\t\t\t vivocha.contact.on\('left', function \(\) {\n\t\t\t vivocha.$\('\#vvc\_btn\_sharing'\).removeClass\('vvc\_btn\_on'\);\n\t\t\t vivocha.contact.leave\(\);\n\t\t\t }\);\n\t\t\t }\);\n }\);\n ", "language": "html" } \] } \[/block\]
