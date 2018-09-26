---
title: "Requirements"
excerpt: ""
---
##**General requirements**
* Vivocha is a web application
* **Cloud:** the architecture and the physical placement of servers are transparent to the user.
* **Accessible to everyone** through the Internet.
* **Secure:** uses HTTPS.

##**Network requirements**
###**Standard application (Settings + Chat)**

If you have any Proxy or Firewall your system must allow your network to have a free access on the following domain:
[block:parameters]
{
  "data": {
    "0-0": "***.vivocha.com**",
    "0-1": "vivocha",
    "1-0": "**d3btqb6knwd3a4.cloudfront.net**",
    "1-1": "static assets",
    "2-0": "**fonts.googleapis.com**",
    "2-1": "not mandatory - fonts, fallback",
    "4-0": "**www.google-analytics.com**",
    "4-1": "usage status",
    "5-0": "**s3.amazonaws.com**",
    "5-1": "static assets",
    "3-0": "**maps.googleapis.com**",
    "3-1": "not mandatory - maps",
    "h-0": "",
    "h-1": ""
  },
  "cols": 2,
  "rows": 6
}
[/block]

[block:callout]
{
  "type": "info",
  "body": "Vivocha uses WebSockets for the real-time chat channel. You can test if your browser and network are compatible with WebSockets here: http://websocketstest.com/"
}
[/block]
###**Multimedia support (Voice + Video)**
Vivocha uses WebRTC for multimedia communication (https://webrtc.org/)

ICE server: ice.vivocha.com
443 - 444 TCP UDP
5060 - 5061 TCP UDP
49152 - 65535 UDP

Recorder server: recorder.vivocha.com
443 TCP
30000 - 60000 UDP
[block:callout]
{
  "type": "info",
  "title": "",
  "body": "You can test your network capabilities using the following test provided by the WebRTC consortium: https://test.webrtc.org/"
}
[/block]
##**Network bandwidth ( for each agent ):**
[block:parameters]
{
  "data": {
    "0-0": "CHAT",
    "0-1": "10 kbit/s",
    "1-0": "CHAT + Contact Apps (Co-Browsing, etc..)",
    "2-0": "VOICE + VIDEO",
    "1-1": "100 kbit/s",
    "2-1": "300 kbit/s"
  },
  "cols": 2,
  "rows": 3
}
[/block]
The latency of the network must be **under 20 millisecond**.

##**Browser requirements**
The Vivocha Web client supports several browsers. There are some Vivocha features that are not supported by all browsers (e.g. WebRTC multimedia).

###**Standard application (Settings + Chat)**
Officially supported browser are:
* Google Chrome (latest version);
* Mozilla Firefox (latest version);
* Apple Safari (latest version);
* Microsoft Internet Explorer 11 (only on Windows 7, Windows 8.1 and Windows 10 Operative Systems)
* Microsoft Edge (latest version);

###**Multimedia support (Voice + video)**
To use the multimedia features you need a WebRTC compatible browser. The currently **desktop browsers** supported are:
* Google Chrome (latest version);
* Mozilla Firefox (latest version);

The currently **mobile browsers** supported are:
* Google Chrome (Android only)

Multimedia features are supported by our **Native SDK's** for the following operative systems:
* Android 6 +
* iOS 9 +
[block:callout]
{
  "type": "info",
  "body": "To have the best experience with Vivocha, and to ensure that all the console/widgets features will work properly, we highly recommend to use modern browsers like Google Chrome or Mozilla Firefox, to update the browser regularly, and do not install any browser extensions."
}
[/block]
###**Feature Limitations:**
The following table describes the feature limitations and known issues with the supported browsers.
* **Real-time stats:** available on modern browsers (IE11+);
* **Dissuasion timer** (graphical component): available on modern browsers (IE11+);
* **Browser notification:** available on Google Chrome and Mozilla Firefox ONLY.
* **Others:** other limitations could be applied if the browsers technology doesn't support the feature like:
 * Graphics components;
 * Performances updates;
 * New particular browser-linked features;
 * etc.

##**Website requirements**
The **web pages requirements** are:
* It must be based on Javascript code, **running on the user's browser.**
* The user's browser must allow the execution of Javascript code.
* The **Vivocha Activation Code (VAC)** must be present in every page in which Vivocha’s features are to be used.

**Vivocha Activation Code**
[block:code]
{
  "codes": [
    {
      "code": "<script type=\"text/javascript\">\n(function(){\n  window.vvc_ready_handlers = [];\n  window.vivocha = { ready: function(cb) { window.vvc_ready_handlers.push(cb); }}\n  var t = document.createElement(\"script\");\n  t.type=\"text/javascript\"; t.async=true;\n  t.src=\"//www.vivocha.com/a/ACCOUNTID/api/vivocha.js\";\n  var n=document.getElementsByTagName(\"script\")[0];\n  n.parentNode.insertBefore(t,n);\n})();\n</script>",
      "language": "javascript"
    }
  ]
}
[/block]
The **Form Sharing requirements** are:
* Forms must be **compliant** with the **HTML standards.**
* Can be **limited/disabled** through specific CSS classes (optional).
<br />

##**Computer/Hardware requirements**
[block:parameters]
{
  "data": {
    "h-0": "Suggested",
    "h-1": "Minimum",
    "0-0": "Full HD Monitor",
    "1-0": "Speakers",
    "2-0": "Headphone with noise cancellation microphone",
    "3-0": "Full HD Webcam (compatible with selected OS)",
    "0-1": "HD Ready monitor",
    "1-1": "Speakers",
    "2-1": "Headphone with noise cancellation microphone",
    "3-1": "Webcam (compatible with selected OS)"
  },
  "cols": 2,
  "rows": 4
}
[/block]
The computer hardware must allow the execution of the browser without slowing down due to the inadequacy of cpu and/or ram.

**Supported Operating Systems:**
* Microsoft Windows 7 +;
* Apple OS X - 10.8 +;

##**Privacy - cookie description:**
[block:parameters]
{
  "data": {
    "h-0": "Profiling",
    "0-0": "vvcu",
    "0-1": "3 years (renewed every visited page)",
    "0-2": "unique identifier of the user, used for reports and for the creation of a contact",
    "1-0": "vvct",
    "1-1": "30 minutes (renewed every visited page)",
    "1-2": "unique identifier of the visit, which is used for the report and for the creation of a contact"
  },
  "cols": 3,
  "rows": 2
}
[/block]

[block:parameters]
{
  "data": {
    "h-0": "Technical",
    "0-0": "vvc_vp / vp",
    "1-0": "vvc_wv_ID /wv_ID",
    "0-1": "session",
    "1-1": "session",
    "0-2": "number of page views used for the rule of proactivity",
    "1-2": "number of views of the widget used for the rule of proactivity"
  },
  "cols": 3,
  "rows": 2
}
[/block]

[block:parameters]
{
  "data": {
    "0-0": "vvc_host / host",
    "1-0": "vvc_mediaid / mediaid",
    "2-0": "vvc_contactid /contactid",
    "3-0": "vvc_nick / nick",
    "0-1": "session",
    "1-1": "session",
    "2-1": "session",
    "3-1": "session",
    "0-2": "primary node on which is connected the chat (may change during the contact), used to restore the chat while browsing",
    "1-2": "configuration widget, used to represent the chat used to restore the chat while browsing",
    "2-2": "id of contact, used to restore the chat while browsing",
    "3-2": "nickname of the user, used to restore the chat while browsing",
    "h-0": "Session"
  },
  "cols": 3,
  "rows": 4
}
[/block]