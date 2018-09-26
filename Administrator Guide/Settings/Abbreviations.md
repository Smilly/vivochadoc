---
title: "Abbreviations"
excerpt: ""
---
Abbreviations are shortcuts for the most common phrases used by an agent or by an user with other role that is having a chat with a customer. By typing or clicking on an abbreviation he can answer a customer's question in no time at all, sending to him a canned response or a pre-prepared phrase.

By clicking the "Abbreviations" button on the Settings sidetab you will be taken to the abbreviations page where you can see all of the existing shortcuts configured on your account and you can also add, edit and delete them. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8095707-abbreviations_administrator.png",
        "abbreviations_administrator.png",
        1457,
        787,
        "#e1e1e0"
      ],
      "sizing": "full"
    }
  ]
}
[/block]
To add a new shortcut click on "Add new shortcut" in the top-left part of the page.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/3f2c9fd-new_abbreviation_button.png",
        "new_abbreviation_button.png",
        302,
        95,
        "#e6e6e6"
      ],
      "sizing": "original"
    }
  ]
}
[/block]
a new page will open where is possible to configure a new abbreviation by setting the shortcut that an agent can type in place of the entire content of the canned response that will be sent to the customer. 
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/6436c09-new_abbreviation_page.png",
        "new_abbreviation_page.png",
        1358,
        770,
        "#e3e3e3"
      ],
      "sizing": "full"
    }
  ]
}
[/block]
To edit an already existing abbreviation you have to click on the relative :fa-cog: button and the same page will open in the editing mode.

An abbreviation may be associated with one or more tags by which is possible to determine in which services and which users are allowed to visualize and use it during a chat with a customer.

The general rule in the use of tags is valid also for the abbreviations so **a shortcut with some specific tags is visible only in those services and for those users that share those tags or a subset of it.**

To add a tag to the abbreviation simply type the tag in the tag bar. When a user with the administrator/supervisor role creates a new abbreviation, his own tags are assigned to it by default.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/d1e45f4-abbreviation_tag_field.png",
        "abbreviation_tag_field.png",
        493,
        232,
        "#e4e4e4"
      ]
    }
  ]
}
[/block]
You can delete an abbreviation by clicking on the corresponding :fa-times-circle-o: action, then click on "Yes" when you are asked whether you want to permanently delete the shortcut.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/3571347-delete_abbreviation.png",
        "delete_abbreviation.png",
        1237,
        242,
        "#e3e3e2"
      ],
      "sizing": "full"
    }
  ]
}
[/block]
It's also possible to set an **autorun shortcut** so it can be sent immediately as the chat begins, enabling the 'autorun' flag. To do so enter the abbreviation page in editing mode and check the "Automatic send" field. Only one shortcut can be put in "autorun" mode.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/774c9f1-autorun_message.png",
        "autorun_message.png",
        1103,
        459,
        "#e6e6e6"
      ],
      "sizing": "full"
    }
  ]
}
[/block]
The "autorun" abbreviation item is displayed first in the shortcut list and given a greenish background and icon.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/33d926a-abbreviation_page_autorun_.png",
        "abbreviation_page_autorun_.png",
        1109,
        355,
        "#e2e1e0"
      ]
    }
  ]
}
[/block]
### The Shortcuts contact tool
This is how the shortcuts are displayed in the shortcut application tool. The green item is the one set as autosend.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5d126ac-abbreviations_tool.png",
        "abbreviations_tool.png",
        960,
        475,
        "#e9eae5"
      ],
      "sizing": "full"
    }
  ]
}
[/block]
The image below shows the available action buttons for each item.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/27453d0-abbreviations_buttons.png",
        "abbreviations_buttons.png",
        383,
        202,
        "#e8eae2"
      ]
    }
  ]
}
[/block]
1. To copy and paste a shortcut in your textarea.
2. To send a shortcut immediately click the play button.
3. This icon indicates the number of tags associated to an item.
4. The "Down arrow" expand or collapse all the list items at once. Clicking on a list item you will expand it: this will display its tags and the whole shortcut content. To collapse an item simply click on it again.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/4758c60-expanded_abbreviation_tool.png",
        "expanded abbreviation tool.png",
        968,
        496,
        "#e8eae1"
      ]
    }
  ]
}
[/block]
To use a canned response while chatting you simply have to type in the shortcut (e.g. "_ge") or click on the shortcut in the list of possible shortcuts.

<br />

During the configuration of the macro's contents, Vivocha provides a set of special strings (placeholder) which will be automatically replaced by the system with the current agent data:
 
* **${agent.full_name}** : this placeholder will be replaced by the name and the surname set for the user account.
* **${agent.nick_name}** : this placeholder will be replaced by the nickname set for the user account.
 
<br /> 

If you wish to give **special formatting** to your messages you need to use a special syntax:

* **\_message_** o **\__message__**: italics ( result: _message_ );
* **\*message* ** o **\*\*message**** : bold ( result: **message** );
* **http://www.vivocha.com** : send a link  ( result: http://www.vivocha.com );
* "**link**”:http://www.vivocha.com: give a label to a link (result: [link](http://www.vivocha.com));