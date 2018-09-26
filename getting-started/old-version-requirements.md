---
title: old version requirements
excerpt: ''
---

# old version requirements

The following are the **Vivocha requirements:**

* Vivocha is a web application
* **Cloud:** the architecture and the physical placement of servers are transparent to the user.
* **Accessible to everyone** through the Internet.
* Vivocha works with standard web protocols \(**HTTP** e **HTTPS**\).

If you have any Proxy or Firewall your system must allow your network to have a free access on the following domain: \[block:parameters\] { "data": { "0-0": "**\*.vivocha.com**", "0-1": "vivocha", "1-0": "**d3btqb6knwd3a4.cloudfront.net**", "1-1": "static assets", "2-0": "**fonts.googleapis.com**", "2-1": "not mandatory - fonts, fallback", "4-0": "**www.google-analytics.com**", "4-1": "usage status", "5-0": "**s3.amazonaws.com**", "5-1": "static assets", "3-0": "**maps.googleapis.com**", "3-1": "not mandatory - maps", "h-0": "", "h-1": "" }, "cols": 2, "rows": 6 } \[/block\]   


  
 The **web pages requirements** are:

* It must be based on Javascript code, **running on the user's browser.**
* The user's browser must allow the execution of Javascript code.
* The **Vivocha Activation Code \(VAC\)** must be present in every page in which Vivocha’s features are to be used.

  
 **Vivocha Activation Code** \[block:code\] { "codes": \[ { "code": "\n\(function\(\){\n var t = document.createElement\(\"script\"\);\n t.type=\"text/javascript\"; t.async=true;\n t.src=\"//www.vivocha.com/a/ACCOUNT/api/vivocha.js\";\n var n=document.getElementsByTagName\(\"script\"\)\[0\];\n n.parentNode.insertBefore\(t,n\);\n}\)\(\);\n", "language": "javascript" } \] } \[/block\] The **Form Sharing requirements** are:

* Forms must be **compliant** with the **HTML standards.**
* Can be **limited/disabled** through specific CSS classes \(optional\).

Test your browser and network here: [http://websocketstest.com/](http://websocketstest.com/)   


  
 The **Browser requirements** are:

The Vivocha Web client supports several browsers. There are some Vivocha features that are not supported by all browsers.

Officially supported browser are:

* Google Chrome \(latest version\);
* Mozilla Firefox \(latest version\);
* Apple Safari \(latest version\);
* Microsoft Internet Explorer 9+;

Feature Limitations:

The following table describes the feature limitations and known issues with the supported browsers.

* **Real time stats:** available on modern browsers \(IE9+\);
* **Dissuasion timer** \(graphical component\): available on modern browsers \(IE9+\);
* **Browser notification:** available on Google Chrome and Mozilla Firefox ONLY.
* **Others:** other limitations could be applied if the browsers technology doesn't support the feature like:
  * Graphics components;
  * Performances updates;
  * New particular browser-linked features;
  * etc.

To have the best experience with Vivocha, and to ensure that all the console/widgets features will work properly, we highly recomend to use modern browsers like Google Chrome or Mozilla Firefox, to update the browser regularly, and do not install any browser extensions. \[block:callout\] { "type": "warning", "title": "Warning", "body": "Starting from Vivocha rel 4.3 \([http://tech.vivocha.com/post/115856337168/vivocha-4-3](http://tech.vivocha.com/post/115856337168/vivocha-4-3)\) the platform is **not more fully compatible with IE8.**\n\nThe IE limitations are:\n\n _Some contact apps could not work;\n_ Is not possible to use the Telephony features;\n\* Is not possible to use the Video-chat capabilities;\n\n\nThe new Telephony/Video features are natively supported in all the browsers that support WebRTC like the last version of Google Chrome or Mozilla Firefox and, through flash, is supported in the others browsers." } \[/block\]

  
 **Computer/Hardware:** \[block:parameters\] { "data": { "h-0": "Suggested", "h-1": "Minimum", "0-0": "Full HD Monitor", "1-0": "Speakers", "2-0": "Headphone with noise cancellation microphone", "3-0": "Full HD Webcam \(compatible with selected OS\)", "0-1": "HD Ready monitor", "1-1": "Speakers", "2-1": "Headphone with noise cancellation microphone", "3-1": "Webcam \(compatible with selected OS\)" }, "cols": 2, "rows": 4 } \[/block\] The computer hardware must allow the execution of the browser without slowing down due to inadequacy of cpu and/or ram.

**Network** \( for each agent \): \[block:parameters\] { "data": { "0-0": "CHAT", "0-1": "10 kbit/s", "1-0": "CHAT + Contact Apps \(Co-Browsing, etc..\)", "2-0": "VOICE + VIDEO", "1-1": "100 kbit/s", "2-1": "300 kbit/s" }, "cols": 2, "rows": 3 } \[/block\] The latency of the network must be **under 20 millisecond**.

Supported Operating Systems:

* Microsoft Windows 7 +;
* Apple OS X - 10.8 +;

  
 **Cookie:** \[block:parameters\] { "data": { "h-0": "Profiling", "0-0": "vvcu", "0-1": "3 years \(renewed every visited page\)", "0-2": "unique identifier of the user, used for reports and for the creation of a contact", "1-0": "vvct", "1-1": "30 minutes \(renewed every visited page\)", "1-2": "unique identifier of the visit, which is used for the report and for the creation of a contact" }, "cols": 3, "rows": 2 } \[/block\]

\[block:parameters\] { "data": { "h-0": "Technical", "0-0": "vvc\_vp / vp", "1-0": "vvc\_wv\_ID /wv\_ID", "0-1": "session", "1-1": "session", "0-2": "number of page views used for the rule of proactivity", "1-2": "number of views of the widget used for the rule of proactivity" }, "cols": 3, "rows": 2 } \[/block\]

\[block:parameters\] { "data": { "0-0": "vvc\_host / host", "1-0": "vvc\_mediaid / mediaid", "2-0": "vvc\_contactid /contactid", "3-0": "vvc\_nick / nick", "0-1": "session", "1-1": "session", "2-1": "session", "3-1": "session", "0-2": "primary node on which is connected the chat \(may change during the contact\), used to restore the chat while browsing", "1-2": "configuration widget, used to represent the chat used to restore the chat while browsing", "2-2": "id of contact, used to restore the chat while browsing", "3-2": "nickname of the user, used to restore the chat while browsing", "h-0": "Session" }, "cols": 3, "rows": 4 } \[/block\]

