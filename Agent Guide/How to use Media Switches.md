---
title: "How to use Media Switches"
excerpt: ""
---
[Status notifier](#section-status-notifier)
[Chat, video and voice switches](#section-chat-voice-and-video-switches)
[The pause button](#section-the-pause-button)
[Forced Paused](#section-forced-paused)
[Offline](#section-offline)

<br>

**Media switches** are located in the top right area of the Vivocha’s top bar. They consisted of a pause/start button, up to **three individual switches for chat, voice and video channels**, and of **a status notifier** that changes according to the agent's availability on the console.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/N3RtKUIjQoacbTR4k2Uk_media-switches.gif",
        "media-switches.gif",
        "480",
        "270",
        "#d27f59",
        ""
      ],
      "sizing": "full"
    }
  ]
}
[/block]
##Status notifier
The status notifier is placed on the right of the start/pause button. It is composed by a **coloured dot in addition to a description that indicates whether the agent is ready to receive contacts or he is in pause. 

* **green dot + READY** means the agent is ready to accept contacts;
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/pZ1PQAbnSuqBTDYEt2Gm_ready-status.jpg",
        "ready-status.jpg",
        "324",
        "37",
        "#e0e5c9",
        ""
      ]
    }
  ]
}
[/block]
- **yellow dot + PAUSED** means the agent is in pause mode 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/11oZumidRGO8Tg5NYS1h_pause-status.jpg",
        "pause-status.jpg",
        "324",
        "37",
        "#b4a07e",
        ""
      ]
    }
  ]
}
[/block]
- **red dot + DISCONNECTED** means the agent is offline and he is not able to receive contacts.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/kecTrH6lTc69sdm1uTcN_disconnected-status.jpg",
        "disconnected-status.jpg",
        "357",
        "37",
        "#e1e1c9",
        ""
      ]
    }
  ]
}
[/block]
##Chat, voice and video switches
An agent can handle different types of contacts, using the media channels of chat, voice call and video call, depending on the settings set up in his profile by his supervisor or by an administrator (please refer at this section in the documentation [User Settings](doc:admin-users#section-the-user-editor)).

To each channel corresponds  a button, shown when the agent is enabled to the use of that media, and which can be manually switch on or off to set his availability to receive and handle contact of that particular type.

These buttons are represented with icons: a baloon (chat), a phone (voice call) and a videocamera (video call).
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/LRRqESdqReU0myqOJaGQ_one-media-off.png",
        "one-media-off.png",
        "211",
        "41",
        "#89b574",
        ""
      ],
      "caption": ""
    }
  ]
}
[/block]
they can assume different colours:

**GREEN:** it means that the agent has the media **switched on** and he's ready to accept new contacts on that.

**RED:** it means that the agent has the media **switched off**, therefore he can't receive contacts on that;

**YELLOW:** it means that the agent is **paused**.

in the example of the figure above the agent can handle contacts from all the three media type and in fact all the three channel are enabled in the settings of his profile. Since he has manually disabled the video call channel he has notified the system that he is not more available on the video channel, therefore the customers that are having a chat with him cannot eventually request to switch to a video call.

Chat, voice and video switches can be handled separately from each other, so an agent can decide to turn off one of them because for a while he don't want receive the chat contacts, or callback or either because he don't want to give customers the possibility to ask for a video call durning a normal chat. 

Moreover the status of the media channel, enabled (green) or disabled (red), is not propagated if an agent is logged into the console in more than one session from different workstations; this is allowed for example when an agent want to handle the chats and the voicecalls in a workstation whereas he prefer to receive the videocalls only in a workstation that perhaps is equipped with a more performing videocamera that allow to have video call with a better quality.
In this circumstance the same agent can have two active sessions and in front of him two screen with two agent desktops where only the chat and the voice switches are green (enabled) and the video is red (disabled) in the first, whereas in the second the chat and voice channels are red and only the video is green.
[block:callout]
{
  "type": "warning",
  "body": "It's important to point out that even the agent has two active sessions, that is he logged into two different workstations to handle separately the different types of contacts that he can receive, he still count as one for the evaluation of the real time stats and to determine how many contacts are still manageable from the online agents and how many widgets is possible to show to customers in the website"
}
[/block]
##The Pause Button
A circular button with a *pause/play* symbol allows to enter/exit from the pause state: by clicking it the current status of the available media channels change at once.

When the pause button is triggered the media channels that in that moment are in green become yellow and the button itself turns to green by showing the *play* symbol in the center; the Status Notifier confirms that the agent is not available for contacts by blinking the word **Paused** for a few seconds.
[block:callout]
{
  "type": "warning",
  "body": "Differently from the status of the chats, voice and video media switches, that are manageable separately across the different active sessions of an agent for the reason that we have explained above, the status online/paused is shared across the active sessions. A change of the status from online to paused and viceversa is propagated across al the sessions, that means that when an agent set himself in pause in a session active in a browser, this mode is shared also with the other active sessions on other browsers."
}
[/block]
When he is paused an agent can handle existing contacts and even see and accept the new incoming ones if the appropriate option is enables in the agent menù at the top right corner of the Agent Console. 
[block:callout]
{
  "type": "warning",
  "body": "This is a browser option, that means that the contacts are still proposed when the agent is paused on this browser. If he access the console from another browser where this option is disabled, when he is paused the incoming contacts are not more visible for him."
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d8e5093-Screen_Shot_2017-06-20_at_12.33.48.png",
        "Screen Shot 2017-06-20 at 12.33.48.png",
        430,
        441,
        "#dee3e2"
      ]
    }
  ]
}
[/block]
The agent can exit the paused mode by clicking again on the button, with the channels that will switch back from yellow to green.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/9w3CkCA6RtWfnHtGb5h9_pause:unpause.gif",
        "pause:unpause.gif",
        "397",
        "35",
        "#dbe9d3",
        ""
      ]
    }
  ]
}
[/block]

[block:callout]
{
  "type": "warning",
  "body": "A switched off media is not affected by the agent changing his status, and it remains red, since he is not allowed to use this channel even when he is ready and not paused. This helps to remind that media has been manually disabled."
}
[/block]
##Forced Paused
When agent fails to accept a contact, he may be automatically paused by the system under certain conditions.

In this case the **pause is not triggered by the agent** himself but it is the system that set this status if the relative option is configured in the account settings.

A yellow popup appears just on top of the waiting contacts area to warn the agent that Forced Pause has been triggered. The status notifier is yellow and a “Pause” writing blinks.

This happens for instance when there is only one agent available and he is not able to accept all the incoming contacts. He can still handle the existing contacts but his status is set to pause by the system to prevent other contacts are distributed to him.

To exit this forced pause state, agent must simply click on the pause button as for the normal pause state.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/f1ee58b-Screen_Shot_2017-03-16_at_10.42.28.png",
        "Screen Shot 2017-03-16 at 10.42.28.png",
        1437,
        822,
        "#ecebe8"
      ],
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
##Offline
Most of times the loss of connection is due to some network problems.

When connection with the server is lost, a popup is displayed in the waiting contact area. The status notifier displays a red dot followed by the writing "Disconnetcted".

The popup fades out and the status notifier turns green as soon as the connection is re-established.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7d8af8c-Screen_Shot_2017-03-16_at_11.22.07.png",
        "Screen Shot 2017-03-16 at 11.22.07.png",
        1439,
        823,
        "#eae8e7"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]