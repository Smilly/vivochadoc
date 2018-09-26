---
title: "How to handle a contact"
excerpt: ""
---
[Waiting contacts section](#section-waiting-contacts-section)
[Dissuasion time](#section-dissuasion-time)
[Assigned contacts area](#section-assigned-contacts-section)
[Assign a color to the contact](#section-assign-a-color-to-the-contact)
[Multimedia Interactions](#section-multimedia-interactions)

<br>

In Vivocha a contact is a multimedia interaction: it can take off as a chat and continue as a phone call or video; the chat channel might be dropped as soon as a phone connection is established, or a video interaction can be launched depending on browser capabilities.
The right section of your console is the area where you can manage your contacts (chat, voice and video) and it is basically divided in two parts: **waiting** and **assigned**

##Waiting contacts section
When a your customer using a web browser enters your website and requests for a contact from a page where a Vivocha widget has been configured, you are notified of the request as appears in the image below.

A waiting contact, also referred as **pending** could be generically addressed to all the team that manage a service (shown to all the agents matching the service tags) or to a specific agent and, in this case, the contact will be matched by a star. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/3sHnKIjfT1GFLM6joBUC_waiting.jpg",
        "waiting.jpg",
        "621",
        "360",
        "#316078",
        ""
      ],
      "border": true
    }
  ]
}
[/block]
1. The number of contacts are waiting for being managed.
2. Customer name (the customer name could be collected or directly detected by the system in different ways).
3. Customer nationality.
4. This label tells you that the contact is from a new visitor.
5. [Dissuasion](#section-dissuasion-time) countdown.
6. The star indicates that this contact is to the agent or distributed only to him/her (no other agent is currently eligible to handle it).
7. The service language.
8. The service name.
9. The site from which the customer came from.


###Dissuasion time
To let the agents to have the needed amount of time to accept a pending contact, it's been defined a maximum slot of waiting time (which can be set for each service) called **dissuasion time**, represented by a loader that become progressively red when the time is ending. To pick up the contact preventing the dissuasion of it you have to click the loader before the time runs out.

The icon in the center indicates which kind of contact is (chat, voice, video etc).
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/iRWjtItVSSati07dYcfA_Screen%20Shot%202016-07-13%20at%202.57.13%20PM.png",
        "Screen Shot 2016-07-13 at 2.57.13 PM.png",
        "82",
        "80",
        "#dd5b62",
        ""
      ],
      "caption": "",
      "border": false
    }
  ]
}
[/block]
The waiting contact number is indicated on the top and, by clicking on the contact box, the system will assign to the agent the contact who waited for more time. 

If you don't want to manage the first available contact, you can choose another one from the pending contacts. To do that you have only to pass over the waiting area and a drawer will open and show the details about the waiting contacts.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/hBw36QaSY6YEj5iQSfOA_pending-contacts.gif",
        "pending-contacts.gif",
        "1278",
        "885",
        "#c66157",
        ""
      ],
      "caption": "For choosing another contact just pass over the waiting area"
    }
  ]
}
[/block]
<br>
##Assigned contacts section
Clicking on a pending contact, the contact is assigned to the agent and moved in the assigned group. There’s an interaction panel per each contact and only on panel is fully expanded at any time. When a new message or event is received on a collapsed panel, a flashing message is displayed. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/e60eeb7-Screen_Shot_2015-03-27_at_10.07.21.png",
        "Screen Shot 2015-03-27 at 10.07.21.png",
        433,
        833,
        "#ececeb"
      ],
      "border": true,
      "sizing": "smart"
    }
  ]
}
[/block]
The box of an assigned contact is composed by different areas with different functionalities.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/6GDnvQJQV2enTiEs8kpj_chat-box.png",
        "chat-box.png",
        "637",
        "466",
        "#295a71",
        ""
      ]
    }
  ]
}
[/block]
On the top:

* **customer's name (1)**
* the clock icon :fa-clock-o:  with the **duration** of the contact **(4)**
* the information about the **status** of the contact and the customer activity **(5)** represented by different icons.
[block:parameters]
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
    "2-0": "<span style=\"color:#dd565a\"> :fa-comment: </span>",
    "2-1": "there is message of the customer non read yet"
  },
  "cols": 2,
  "rows": 5
}
[/block]
just below, on the left, you find the icons of the **media channels**  that depending on their states are shown in different colors: green circles, blackish and light grey. 
[block:parameters]
{
  "data": {
    "1-0": "7 - :fa-comments:",
    "h-0": "icon",
    "h-1": "channel",
    "1-1": "Chat",
    "0-0": "6 - :fa-share-alt:",
    "0-1": "Data sharing",
    "2-0": "2 - :fa-phone:",
    "2-1": "Voice",
    "3-0": "3 - :fa-video-camera:",
    "3-1": "Video"
  },
  "cols": 2,
  "rows": 4
}
[/block]
* When a channel is **green with a white icon in the centre**, that means it is active.
* When is **orange with a white icon in the centre**, that means it is connecting. 
* when the icon is **dark-grey** that channel is available and can be activated by clicking on it.  
* A **light-grey** coloured icon communicates that the channel is not available and cannot be established.


On the right you can find a set of tools.
[block:parameters]
{
  "data": {
    "0-0": "8 -   :fa-upload:",
    "0-1": "Upload a file",
    "h-0": "Icon",
    "h-1": "function",
    "h-2": "Meaning",
    "0-2": "",
    "1-0": "9 -   :fa-flag:",
    "2-0": "10 - :fa-tag:",
    "3-0": "11 - :fa-close:",
    "1-1": "Translations",
    "1-2": "",
    "2-1": "Assign a color to the contact",
    "2-2": "",
    "3-1": "Stop the contact",
    "3-2": ""
  },
  "cols": 2,
  "rows": 4
}
[/block]
###Assign a color to the contact
The agent can **assign colors** to contacts to help himself to **identify the subject** before they answer it. 

In this way you can establish which are contact to be managed first, giving them a priority, or who is better suitable to answer a particular contact in case of a transfer. Each color can have a different meaning: technical support, general inquire, problems to fill up forms, cannot find information on the website, etc. 

The agent can **set the contact color** clicking on the color tag tool inside the contact box area.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/fd8af1f-Screen_Shot_2017-03-13_at_11.31.41.png",
        "Screen Shot 2017-03-13 at 11.31.41.png",
        429,
        379,
        "#ced3d0"
      ]
    }
  ]
}
[/block]

[block:callout]
{
  "type": "info",
  "body": "A contact could already have a color because of the service settings. The administrator can in fact decide to attribute a color to all the contacts came from a specific service."
}
[/block]
Assign a color to a contact is not the only functionality that agents can use. For example, they can exploit the automatic translation if the customer is chatting in a different language, they can push a link and redirect the customer to that page or send him a file. 

You can red more about all these tools at the relative documents: 
* **[automatic translations](doc:how-to-handle-a-chat#section-automatic-translations)**
* **[how to push a link](doc:how-to-push-a-link)**
* **[how to send a file](doc:how-to-send-a-file)**

As we said in Vivocha a contact is a multimedia interaction: depending of the different customer support experience of support that you want to offer as well as from the customer's preference itself, they can engage your agents in different ways by taking advantage of different media channels.  

The main types of a contact are: **Chat**, **CallBack**, **Call** and **Video Call**, **WebLead**

After the customer has requested a contact to receive assistance by an agent, it could be necessary to take advantage of another channel different from the one he initially he chose. Here are presented some of the possible scenarios of how a multimedia interaction can take place

##Multimedia interactions

###From messages to video-chat and return
**Case 1: chat interaction requested via widget and accepted by an agent turned into video chat is activated and then dropped.**
Agent Mike decides to engage the customer in a video interaction: to do this he simply click on the video-camera icon. The interaction proceeds as follow:
* on agent side both voice and video icons turn into orange circles (loading state) and a waiting message appear within the media channel toolbar.
* the customer is prompted a video interaction request.
* customer may choose to start a video interaction, showing his local video or to opt in for a voice interaction only, in that case he will see the agent without being seen
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7c2e7a7-Screen_Shot_2017-03-12_at_22.29.57.png",
        "Screen Shot 2017-03-12 at 22.29.57.png",
        1254,
        708,
        "#eeeeed"
      ]
    }
  ]
}
[/block]

[block:callout]
{
  "type": "warning",
  "body": "Please note that video requires Google Chrome or Firefox to work."
}
[/block]
* Customer accepts the video request and after having allowed access to both camera and microphone (depending on browser settings) the video interaction starts: all the media icons are green both for agent and customer!
 
On the media toolbar you may notice two buttons:
* expand/collapse button to detach the video
* mute button to enable/disable the microphone

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/e35f938-Screen_Shot_2017-03-12_at_22.37.34.png",
        "Screen Shot 2017-03-12 at 22.37.34.png",
        1180,
        711,
        "#e7e7e6"
      ]
    }
  ]
}
[/block]
Once there's no need to continue with a video interaction, both customer and agent may return to a chat-only contact by clicking the green video icon. Doing this they interrupt their video call returning to the previous state

###From messages to video-chat and return
That of a video interaction established starting from a chat, is not the only possible scenario. That was simply to show you how the new media apps engine works. 
We're going to simulate another situation with different media: this time we'll start from a chat and then establish a phone call dropping the chat accordingly.

**Case 2: the customer requests a chat interaction and agent accepts the contact. After some messages they decide to make a phone call.**
The agent clicks on the voice-phone icon. A popup with a voice type menu  appears. In this case the agent goes for a phone call using twilio (browser call triggers a *browser to browser* call instead).
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5482cd5-Screen_Shot_2015-06-17_at_13.45.36.png",
        "Screen Shot 2015-06-17 at 13.45.36.png",
        431,
        378,
        "#d6dada"
      ]
    }
  ]
}
[/block]
The agent is asked to provide a valid phone number, then it's possible to click 'call' and continue.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/63398e1-Screen_Shot_2015-06-17_at_13.46.18.png",
        "Screen Shot 2015-06-17 at 13.46.18.png",
        432,
        339,
        "#cbd1d1"
      ]
    }
  ]
}
[/block]
the call starts, the corresponding icon in orange means that the connecting is in progress
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/33973fd-Screen_Shot_2015-06-17_at_13.46.52.png",
        "Screen Shot 2015-06-17 at 13.46.52.png",
        430,
        368,
        "#f4f4f4"
      ]
    }
  ]
}
[/block]
Once the customer answers both chat and voice icons are in active state. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/0926193-Screen_Shot_2015-06-17_at_14.04.57.png",
        "Screen Shot 2015-06-17 at 14.04.57.png",
        427,
        348,
        "#f5f5f5"
      ]
    }
  ]
}
[/block]
The customer then drops the chat closing the widget on his browser, and on the contact cart this result in the chat being disabled (light-grey icon): the chat channel is now closed but the contact itself is not as it's being carried on as a phone call.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/4464cc0-Screen_Shot_2015-06-17_at_13.50.47.png",
        "Screen Shot 2015-06-17 at 13.50.47.png",
        431,
        339,
        "#e7e8e7"
      ]
    }
  ]
}
[/block]
To close the contact simply click on the x button placed on the right. A popup appears and it is possibile to cancel the action or close the contact.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/f09ee16-Screen_Shot_2015-06-17_at_15.29.36.png",
        "Screen Shot 2015-06-17 at 15.29.36.png",
        431,
        279,
        "#c7cfcb"
      ]
    }
  ]
}
[/block]