---
title: "Transfer Groups"
excerpt: ""
---
The ability to transfer a contact between an agent and another one is already present withVivocha but in Vivocha 5.0 we make some enhancements with the introduction of groups and prioritization.

Now you have a new tab into your Vivocha Account that is called Transfer Group in which you can just add a new group and if you do so you will not able to transfer a contact to a service anymore but you will just be able to transfer to a group instead.

So this means that the transfer to a service feature is substituted by the transfer to a group, which works basically in the same way but it ends up to be much more clear for the agents using it.
In fact with the Transfer Groups feature there is no more need to have the whole list of the services that are configured in the account during a transfer, but you have the groups that you have defined in corresponding section in the Settings.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/4f569c0-transfer_groups_1.png",
        "transfer_groups_1.png",
        1438,
        646,
        "#e2e2e2"
      ],
      "caption": ""
    }
  ]
}
[/block]
As you can see in the image we have already two groups, one is called Support one is called Sales, they were assigned with different priority, Support is priority 13, Sales is priority 15 and with different types as well. The assigned tags are those that are shared by the agents you want to be in these particular groups, so for example all the agents with the “sales” tag are included in the group Sales, and all the agents with the “support” and “help” tags are part of the Support group.

So basically if you click the **:fa-users: Add a new group** button, you see what is shown in this second image that is a very a simple panel in which you have to define the name of the group, the transfer priority and the tags just as we saw before.

A contact transferred to the agents in a group will appear in a position in the waiting section for the pending contacts that depends from the priority parameter assigned to that group. The more high is the priority the more high is the position of the transferred contact will appear in the waiting section.
You can also define more groups which share the same set of tags and give them a different priority, in order that you can transfer a contact to a particular group of agents who have those tags but with a different level of priority depending on the needs.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b186b87-transfer_groups.png",
        "transfer_groups.png",
        930,
        612,
        "#e2e2e2"
      ],
      "sizing": "full"
    }
  ]
}
[/block]
Transfer Groups contact can be set between 1 and 30 and 15 is the default value. 

[block:callout]
{
  "type": "info",
  "body": "As Adminitrator you can to set other two important parameters which affect the contacts transfer. To do this go to **[Routing](doc:routing-config#section-transfer)** panel.",
  "title": "Info"
}
[/block]
And finally during a contact transfer, you will see these groups appearing as well as the possibility to transfer to an agent because this one is still available, so you are always been able to transfer to a specific agent or you are able to choose a different group between Support, Sales and the ones you will be configuring.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/a2735b8-transfer_group_3.png",
        "transfer_group_3.png",
        1439,
        802,
        "#ececeb"
      ]
    }
  ]
}
[/block]
there are colours now, green and red, so green is for both the agents that are logged into Vivocha and available to engage contacts, and for groups that contains at least an agent available for contacts. Instead the red color is for groups that in a particular moment don’t have available agents. For each group we have also other information like the number of **available agents**, the amount of **available media slots**, which says how many contacts could be still transferred to the agents of that group, as well as the assigned tags.

For each agent, the ID, name, nickname, assigned tags and status are shown.