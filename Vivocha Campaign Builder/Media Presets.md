---
title: "Media Presets"
excerpt: ""
---
The Media Presets section allows to create new type of presets in addition the the built-in ones, so they can be used by setting up possible interaction modes of the engagement widgets.

[➡ Read about the "Interaction modes" in our documentation](doc:vcb-web-engagement-widgets#section--proposed-media-)

The panel shows the list of presets supported by default: **chat, voice, video, sms** and **weblead**. The built-in media presets cannot be modified.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/548ca02-Screen_Shot_2018-09-14_at_14.07.45.png",
        "Screen Shot 2018-09-14 at 14.07.45.png",
        1420,
        809,
        "#cecece"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
You can create a new one from scratch by clicking the **Add new** button or you can clone a built-in one and then modify the default configuration.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7c3c129-Screen_Shot_2018-09-14_at_14.21.58.png",
        "Screen Shot 2018-09-14 at 14.21.58.png",
        1069,
        385,
        "#fbfbfb"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
Custom presets meet the need to change the standard functioning of a built-in media to be used in a particular scenario. A custom preset can also groups more media and each of them can be set up changing its configuration parameters.

For example you may want a preset that along with the standard chat and the sharing channels that enables to the use of the sharing tools, during contacts presents a WebRTC voice session working in a bi-directional way but the WebRTC video session is in mono-directional with only the user able to visualize the agent

the necessary steps to configure such custom preset are here described:

1. Select and add the **Chat** media by enabling it both in Transmission and Reception

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7af02a2-Screen_Shot_2018-09-14_at_15.19.35.png",
        "Screen Shot 2018-09-14 at 15.19.35.png",
        1071,
        600,
        "#fbfbfb"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
2. Select and add the **Sharing** channel ( it is already enabled both in Transmission and Reception by default)
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/ce451ee-Screen_Shot_2018-09-14_at_15.24.23.png",
        "Screen Shot 2018-09-14 at 15.24.23.png",
        1058,
        593,
        "#fbfbfb"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
3. Select and add the **Voice** media, enabled it both in Transmission and Reception by specifying *WebRTC* as engine and setting the *Net* option in the via parameter.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/10c6994-Screen_Shot_2018-09-14_at_15.27.11.png",
        "Screen Shot 2018-09-14 at 15.27.11.png",
        1065,
        697,
        "#fbfbfb"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
4. Select and add the **Video** media, disabling it for the Transmission but enabling it for the Reception. Also specify *WebRTC* as engine and setting the *Net* option in the via parameter.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/30fd17d-Screen_Shot_2018-09-14_at_15.43.09.png",
        "Screen Shot 2018-09-14 at 15.43.09.png",
        1057,
        740,
        "#fbfbfb"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
At this point, after saving, in the main panel will appear the custom presets section containing the new custom preset just configured.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b619236-Screen_Shot_2018-09-14_at_15.59.41.png",
        "Screen Shot 2018-09-14 at 15.59.41.png",
        1069,
        582,
        "#fcfcfc"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]