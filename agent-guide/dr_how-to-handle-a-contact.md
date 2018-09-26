---
title: dr_how to handle a contact
excerpt: ''
---

# dr\_how to handle a contact

_Topics_

[Waiting contacts section](dr_how-to-handle-a-contact.md#section-waiting-contacts-section) [Dissuasion time](dr_how-to-handle-a-contact.md#section-dissuasion-time) [Assigned contacts area](dr_how-to-handle-a-contact.md#section-assigned-contacts-section) [How to handle a chat](dr_how-to-handle-a-contact.md#section-how-to-handle-a-chat) [How to handle a video contact](dr_how-to-handle-a-contact.md#section-how-to-handle-a-video-contact) [How to send a link and redirect the customer to it](dr_how-to-handle-a-contact.md#section-how-to-send-a-link-and-redirect-the-customer-to-it) [How to send a file](dr_how-to-handle-a-contact.md#section-how-to-send-a-file) [Automatic translations](dr_how-to-handle-a-contact.md#section-automatic-translations)

In Vivocha a contact is a multimedia interaction: it can take off as a chat and continue as a phone call or video; the chat channel might be dropped as soon as a phone connection is established, or a video interaction can be launched depending on browser capabilities. The right section of your console is the area where you can manage your contacts \(chat, voice and video\) and it is basically divided in two parts: **waiting** and **assigned**

## Waiting contacts section

When a your customer using a web browser enters your website and requests for a contact from a page where a Vivocha widget has been configured, you are notified of the request as appears in the image below.

A waiting contact, also referred as **pending** could be generically addressed to all the team that manage a service \(shown to all the agents matching the service tags\) or to a specific agent and, in this case, the contact will be matched by a star. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/3sHnKIjfT1GFLM6joBUC\_waiting.jpg](https://files.readme.io/3sHnKIjfT1GFLM6joBUC_waiting.jpg)", "waiting.jpg", "621", "360", "\#316078", "" \], "border": true } \] } \[/block\] 1. The number of contacts are waiting for being managed. 2. Customer name \(the customer name could be collected or directly detected by the system in different ways\). 3. Customer nationality. 4. This label tells you that the contact is from a new visitor. 5. [Dissuasion](dr_how-to-handle-a-contact.md#section-dissuasion-time) countdown. 6. The star indicates that this contact is to the agent or distributed only to him/her \(no other agent is currently eligible to handle it\). 7. The service language. 8. The service name. 9. The site from which the customer came from.

### Dissuasion time

To let the agents to have the needed amount of time to accept a pending contact, it's been defined a maximum slot of waiting time \(which can be set for each service\) called **dissuasion time**, represented by a loader that become progressively red when the time is ending. To pick up the contact preventing the dissuasion of it you have to click the loader before the time runs out.

The icon in the center indicates which kind of contact is \(chat, voice, video etc\). \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/iRWjtItVSSati07dYcfA\_Screen Shot 2016-07-13 at 2.57.13 PM.png](https://files.readme.io/iRWjtItVSSati07dYcfA_Screen%20Shot%202016-07-13%20at%202.57.13%20PM.png)", "Screen Shot 2016-07-13 at 2.57.13 PM.png", "82", "80", "\#dd5b62", "" \], "caption": "", "border": false } \] } \[/block\] The waiting contact number is indicated on the top and, by clicking on the contact box, the system will assign to the agent the contact who waited for more time.

If you don't want to manage the first available contact, you can choose another one from the pending contacts. To do that you have only to pass over the waiting area and a drawer will open and show the details about the waiting contacts. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/hBw36QaSY6YEj5iQSfOA\_pending-contacts.gif](https://files.readme.io/hBw36QaSY6YEj5iQSfOA_pending-contacts.gif)", "pending-contacts.gif", "1278", "885", "\#c66157", "" \], "caption": "For choosing another contact just pass over the waiting area" } \] } \[/block\]   


## Assigned contacts section

Clicking on a pending contact, the contact is assigned to the agent and moved in the assigned group. There’s an interaction panel per each contact and only on panel is fully expanded at any time. When a new message or event is received on a collapsed panel, a flashing message is displayed. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e60eeb7-Screen\_Shot\_2015-03-27\_at\_10.07.21.png](https://files.readme.io/e60eeb7-Screen_Shot_2015-03-27_at_10.07.21.png)", "Screen Shot 2015-03-27 at 10.07.21.png", 433, 833, "\#ececeb" \], "border": true, "sizing": "smart" } \] } \[/block\] The box of an assigned contact is composed by different areas with different functionalities. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/6GDnvQJQV2enTiEs8kpj\_chat-box.png](https://files.readme.io/6GDnvQJQV2enTiEs8kpj_chat-box.png)", "chat-box.png", "637", "466", "\#295a71", "" \] } \] } \[/block\] On the top:

* **customer's name \(1\)**
* the clock icon :fa-clock-o:  with the **duration** of the contact **\(4\)**
* the information about the **status** of the contact and the customer activity **\(5\)** represented by different icons.

  \[block:parameters\]

  {

  "data": {

    "h-0": "Icon",

    "h-1": "Meaning",

    "0-0": ":fa-globe:",

    "0-1": "the customer is changing the page on the website",

    "3-0": "zZZ",

    "3-1": "the contact is in the **idle** status, that means that for a while there are no messages being exchanged between the agent and the customer",

    "4-0": ":fa-close:",

    "4-1": "contact has been terminated",

    "1-0": ":fa-pencil:",

    "1-1": "the customer is writing a message",

    "2-0": " :fa-comment:",

    "2-1": "there is message of the customer non read yet"

  },

  "cols": 2,

  "rows": 5

  }

  \[/block\]

  just below, on the left, you find the icons of the **media channels**  that depending on their states are shown in different colors: green circles, blackish and light grey. 

  \[block:parameters\]

  {

  "data": {

    "1-0": ":fa-comments:",

    "h-0": "icon",

    "h-1": "channel",

    "1-1": "Chat",

    "0-0": ":fa-share-alt:",

    "0-1": "Data sharing",

    "2-0": ":fa-phone:",

    "2-1": "Voice",

    "3-0": ":fa-video-camera:",

    "3-1": "Video"

  },

  "cols": 2,

  "rows": 4

  }

  \[/block\]

* When a channel is **green with a white icon in the centre**, that means it is active.
* When is **orange with a white icon in the centre**, that means it is connecting. 
* when the icon is **dark-grey** that channel is available and can be activated by clicking on it.  
* A **light-grey** coloured icon communicates that the channel is not available and cannot be established.

On the right you can find a set of tools. \[block:parameters\] { "data": { "0-0": ":fa-upload:", "0-1": "Upload a file", "h-0": "Icon", "h-1": "function", "h-2": "Meaning", "0-2": "", "1-0": ":fa-flag:", "2-0": ":fa-tag:", "3-0": ":fa-close:", "1-1": "Translations", "1-2": "", "2-1": "Assign a color to the contact", "2-2": "", "3-1": "Stop the contact", "3-2": "" }, "cols": 2, "rows": 4 } \[/block\]

## How to handle a chat

When a customer asks for support throught the chat, the agent has to click on the dissuasion timer in the waiting area. The contact will start immediately and without others actions. Through the chat you can also [send a file](dr_how-to-handle-a-contact.md#section-how-to-send-a-file), [send a link and redirect the customer to it](dr_how-to-handle-a-contact.md#section-how-to-send-a-link-and-redirect-the-customer-to-it).

## How to handle a video contact

A video contact can start from the agent or from the customer.

### Video contact started by the agent

The **agent** who wants to start a video contact has to **click on the video icon** inside the chat area and wait for the client confirmation. While the agent waits for the customer confirmation, the icons of voice and video media tools will became orange.

When the agent asks a video call to the customer, the customer can choose to **decline the video** contact and **keep activated only the voice channel** \(or decline both video and voice contact\). \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/9djBXYxSTWC7piAvCJiN\_agent-starts-video.gif](https://files.readme.io/9djBXYxSTWC7piAvCJiN_agent-starts-video.gif)", "agent-starts-video.gif", "428", "556", "\#df6068", "" \], "caption": "If the agent start a video contact" } \] } \[/block\]

### Video contact started by the customer

The **customer** who wants to start a video contact has to **click on the video icon** inside the chat area and wait for the agent confirmation. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/u2p2xsQJSYWOdZXnnKhA\_customer-request-video.png](https://files.readme.io/u2p2xsQJSYWOdZXnnKhA_customer-request-video.png)", "customer-request-video.png", "279", "565", "\#91776b", "" \], "caption": "If the customer starts a video contact" } \] } \[/block\] To accept the request, the agent has to click _ENGAGE_. If the agent doesn't want to have a video contact with the customer, he can **decline the request** by clicking the _NOT NOW_ button. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/Q3FyfHi2T4av34C5SjjM\_customer-requests-video2.png](https://files.readme.io/Q3FyfHi2T4av34C5SjjM_customer-requests-video2.png)", "customer-requests-video2.png", "430", "338", "\#c1cccc", "" \] } \] } \[/block\]

## How to send a link and redirect the customer to it

Sometime an agent needs to send a specific link to the customer and/or redirect him to a specific page of the website. Because of this he can send the link in two ways. 1. First way by simply write the address of the link they want to send and sending it to the customer. By clicking on the link the customer will be redirect to the link the agent sent. 2. Second way is a way to create a special kind of link that allows the agent to redirect the customer to the page he linked him. With the mouse on the link just sent, the agent'll see the hint "Click to send immediately" which is the second way to send a link. By clicking on the link the customer will be redirect to the link the agent sent, as before. But if is the agent that clicks this link, the customer will be redirect to the link without to any action. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/9d3e52c-Screen\_Shot\_2016-07-22\_at\_12.25.12\_PM.png](https://files.readme.io/9d3e52c-Screen_Shot_2016-07-22_at_12.25.12_PM.png)", "Screen Shot 2016-07-22 at 12.25.12 PM.png", 425, 332, "\#f7f7f7" \] } \] } \[/block\]

## How to send a file

Vivocha allows you to send file \(pdf, images, executable etc\) from both agent and customer side.

### The file transfer tool agent side

When an incoming contact is accepted, the contact card is opened and you can see the file transfer trigger on the top, the icon with an upward arrow.

* When you click on the icon, a file upload popup appears. You can send file up to **10 MB for single upload**. You can also add a **description** if you wish.
* Click on the choose file button to open your desktop explorer to choose the file you want to transfer. Select the file you want to send and then click _open_: the name of the choosen file now appears close to the choose file button, you can add a description of the file but this is optional. When you are done click the OK button.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/SUsSuraXRH289cLJY6Sp_agent-sending-a-file.gif",
    "agent-sending-a-file.gif",
    "1277",
    "887",
    "#d77f5a",
    ""
  ]
  ```

    }

  \]

  }

  \[/block\]

  When the upload is complete the file is displayed in the chat with the description \(or simply the name of the file if no description has been inserted\) and a blu download button.  If the file is an image you will preview a portion of it directly in the chat transcript.

You can click on the **image preview** on the chat to expand it; to return to the chat simply click outside the image area or on the rounded x button located on the top-right angle. The customer will now see a message with a blue link and by clicking on it the file will be open.

### The file transfer tool: customer side

The customer too may need to send files to the agent. Widgets have been update with this new functionality.

The customer will see a **paperclip icon** in the text input field. Click on the icon to prompt your file chooser. Once the customer has picked the file to send, a description can be added with the attachment \(optional\). The customers then **digits enter to send the file**. After the upload is complete a blu link icon with the added description, or file name, is displayed in the chat transcript. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/PijkyMATCfpKCxa1wsAg\_customer-sending-a-file.gif](https://files.readme.io/PijkyMATCfpKCxa1wsAg_customer-sending-a-file.gif)", "customer-sending-a-file.gif", "865", "621", "\#9a471c", "" \] } \] } \[/block\] The agent now will be able to both preview the file and download It. If the file is an image, the agent may click on the preview to view it fullscreen.

### The file transfer tool: SDK version

SDK version has been equipped as well with the file transfer feature. Here you can see how the interface appears on IOS and Android devices. In both cases the customer simply taps on the paperclip icon in the bottom left corner to open the system folder/gallery and choose a file to send. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/wA8VirZQ9SKllpTK1vsg\_file transfer ios.PNG](https://files.readme.io/wA8VirZQ9SKllpTK1vsg_file%20transfer%20ios.PNG)", "file transfer ios.PNG", "360", "640", "\#5b8baa", "" \], "sizing": "smart", "caption": "File transfer on iOS" } \] } \[/block\]

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/3DeYBzTrQ6X5yP3C0UXw\_file transfer android.png](https://files.readme.io/3DeYBzTrQ6X5yP3C0UXw_file%20transfer%20android.png)", "file transfer android.png", "360", "640", "\#447ca4", "" \], "caption": "File transfer on Android" } \] } \[/block\] All your attached files are displayed in the _Reports &gt; Contacts &gt; Contact details screen_. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/4DSSfpZStyRGAbf3RCIN\_reports.png](https://files.readme.io/4DSSfpZStyRGAbf3RCIN_reports.png)", "reports.png", "1417", "783", "\#bd7555", "" \], "caption": "Here you can find all the attachments" } \] } \[/block\]

## Automatic translations

If the agent doesn't understand the customer language, he can use the automatic translation. Using it is very simple: to translate the customer message, he must only click on the flag, choose the idioma and press _ok_. To translate his own message he must not do nothing, only write it with the translator opened and the message will be automatically translated.

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/7PQp1fGySVKfrlkq4LCZ\_translation.gif](https://files.readme.io/7PQp1fGySVKfrlkq4LCZ_translation.gif)", "translation.gif", "426", "431", "\#4e575e", "" \] } \] } \[/block\]

## How to transfer a contact

**Transfer groups** are agents grouped to simplify the identification of a set of services/tags that describe the skills needed by the transfer recipients. After the administrator has set them up, an agent can transfer a contact to the proper area he is looking for.

For transfer a contact click on **Transfer button** on the left menu. Here choose the group or agent you want to transfer the contact. Write a message for give some information about the customer. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/IbrSjR4tQKEVfHzgyGLZ\_transfer-contact-1st-agent.gif](https://files.readme.io/IbrSjR4tQKEVfHzgyGLZ_transfer-contact-1st-agent.gif)", "transfer-contact-1st-agent.gif", "1278", "886", "\#d9855c", "" \], "caption": "How to transfer a contact to another agent" } \] } \[/block\] The contact will be redirected to another agent. The second agent will display the message written by the first agent and will start managing the contact. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/N5lLo6XaQIVSlG7bRhw2\_transfer-contact-2nd-agent.gif](https://files.readme.io/N5lLo6XaQIVSlG7bRhw2_transfer-contact-2nd-agent.gif)", "transfer-contact-2nd-agent.gif", "427", "645", "\#ba4f54", "" \], "caption": "How to handle a transferred contact" } \] } \[/block\] This picture shows what the customer will see. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/QAkntWGlSyC2LtsZCZBF\_Screen Shot 2016-06-28 at 3.57.20 PM.png](https://files.readme.io/QAkntWGlSyC2LtsZCZBF_Screen%20Shot%202016-06-28%20at%203.57.20%20PM.png)", "Screen Shot 2016-06-28 at 3.57.20 PM.png", "281", "531", "\#a36746", "" \], "caption": "This is what the customer will see." } \] } \[/block\]

