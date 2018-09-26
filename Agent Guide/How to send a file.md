---
title: "How to send a file"
excerpt: ""
---
[block:callout]
{
  "type": "danger",
  "body": "The file transfer feature do not offer any guarantee regarding the content of the documents and the responsibility to verify the reliability of the files is entirely up to the customer. Possible checks that we carry out, are due the fact that we need the preserve the continuity of the service that we deliver, and they are purely internal to the functioning of the platform therefore their details are not exposed outside."
}
[/block]
Vivocha allows you to send file (pdf, images, executable etc) from both agent and customer side.
 
##The file transfer tool agent side
When an incoming contact is accepted, the contact card is opened and you can see the file transfer trigger on the top, the icon with an upward arrow. 

When you click on the icon, a file upload popup appears. By default you can send files up to 5 MB for single upload. You can also add a description if you wish.
[block:callout]
{
  "type": "warning",
  "body": "The maximum size for the files uploading depends on the details of plan subscribed for the account and it can be extended to 30MB on request."
}
[/block]
Click on the choose file button to open your desktop explorer to choose the file you want to transfer. Select the file you want to send and then click *open*: the name of the choosen file now appears close to the choose file button, you can add a description of the file but this is optional. When you are done click the OK button.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/SUsSuraXRH289cLJY6Sp_agent-sending-a-file.gif",
        "agent-sending-a-file.gif",
        "1277",
        "887",
        "#d77f5a",
        ""
      ],
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
When the upload is complete the file is displayed in the chat with the description (or simply the name of the file if no description has been inserted) and a blu download button.  If the file is an image you will preview a portion of it directly in the chat transcript.

You can click on the **image preview** on the chat to expand it;  to return to the chat simply click outside the image area or on the rounded x button located on the top-right angle.

The customer will now see a message with a blue link and by clicking on it the file will be open.

<br>

##The file transfer tool: customer side
The customer too may need to send files to the agent.  Widgets have been update with this new functionality. The customer will see a **paperclip icon** in the text input field. Click on the icon to prompt your file chooser.

Once the customer has picked the file to send, a description can be added with the attachment (optional). 

The customers then **digits enter to send the file**. After the upload is complete a blu link icon with the added description, or file name, is displayed in the chat transcript.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/PijkyMATCfpKCxa1wsAg_customer-sending-a-file.gif",
        "customer-sending-a-file.gif",
        "865",
        "621",
        "#9a471c",
        ""
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
The agent now will be able to both preview the file and download It. If the file is an image, the agent may click on the preview to view it fullscreen.

<br>

##The file transfer tool: SDK version
SDK version has been equipped as well with the file transfer feature. Here you can see how the interface appears on IOS and Android devices. In both cases  the customer simply taps on the paperclip icon in the bottom left corner to open the system folder/gallery and choose a file to send. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/wA8VirZQ9SKllpTK1vsg_file%20transfer%20ios.PNG",
        "file transfer ios.PNG",
        "360",
        "640",
        "#5b8baa",
        ""
      ],
      "sizing": "smart",
      "caption": "File transfer on iOS",
      "border": true
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/3DeYBzTrQ6X5yP3C0UXw_file%20transfer%20android.png",
        "file transfer android.png",
        "360",
        "640",
        "#447ca4",
        ""
      ],
      "caption": "File transfer on Android",
      "border": true
    }
  ]
}
[/block]
All your attached files are displayed in the *Reports > Contacts > Contact details  screen*.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/4DSSfpZStyRGAbf3RCIN_reports.png",
        "reports.png",
        "1417",
        "783",
        "#bd7555",
        ""
      ],
      "caption": "Here you can find all the attachments",
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
##Attachments Security

The security of the attachments exchanged during chats is ensured by the complexity of the generated URL which allows to access the resource and to download it.

This complexity is achieved by using the SHA-384 cryptographic algorithm, which is a truncated version of the SHA-512 hash function belonging to the SHA- 2 set. The digest (hash values) so computed is made up of 128 bit representing the id of the contact and other 256 bit used for the attachment.

To improve the security level of the attachments files, their corresponding URLs just obtained allow to access the resources only in specific circumstances:

1) **during the contact** the URLs are always accessible both from the customer and the agent

2) **once the contact is closed** the files transferred during it are still available through the URLs until the contact report does not expire (that means that the contact, with all its related data and info, must be still stored in our database) and in these circumstances:

* when there is a valid account session: a user with the access to the Reports Section, an admin of the account or the supervisor of the agent that managed the contact, can download the attachments directly from the contact detail page

* the customer who received an attachment can still access it through the URL of thre file if the used browser to request the contact has got the **vvcu** cookie. 
[block:callout]
{
  "type": "warning",
  "body": "The vvcu cookie identifies the visitor that requests a contact and then it used for the Reports and for the next contacts that he can eventually do. This cookie has a validity of 3 years and it is renewed everytime a page is visited.\n\nNB: it remains valid in the browser if is not deleted and the contact report is not expired"
}
[/block]
* The URL of a transferred file can opened also in browsers that opened the attachment while the contact is on going. It could be the case of a contact from the mobile app (SDK), where an attachment is open within the browser set as default, or in case this URL is forwarded to a third actor, (i.e: from the agent handling the contact to his supervisor). 
When the contact is active and the attachment URL is open an other cookie is set in the browser. it is the **vvca** and its duration corresponds to the life of the contact in the reports.