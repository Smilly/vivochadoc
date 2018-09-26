---
title: "Routing"
excerpt: ""
---
[Tags and Colors](#section--tags-and-colors-)
[&nbsp;&nbsp;&nbsp;Add tags to the Campaign](#section--add-tags-to-the-campaign-)
[&nbsp;&nbsp;&nbsp;Add color](#section--add-color-)
[Pause](#section--pause-)
[&nbsp;&nbsp;&nbsp;Forced pause](#section--forced-pause-)
[&nbsp;&nbsp;&nbsp;Show pending contacts when paused](#section--show-pending-contacts-when-paused-)
[Transfer](#section--transfer-)
[&nbsp;&nbsp;&nbsp;Transfer to busy agents](#section--transfer-to-busy-agents-)
[&nbsp;&nbsp;&nbsp;Transfer back](#section--transfer-back-)
[&nbsp;&nbsp;&nbsp;Transferred contact priority](#section--transferred-contact-priority-)
[&nbsp;&nbsp;&nbsp;Transfer failure timeout](#section--transfer-failure-timeout-)
[Routing rules](#section--routing-rules-)
[&nbsp;&nbsp;&nbsp;Contact routing rules](#section--contact-routing-rules-)
[&nbsp;&nbsp;&nbsp;Dissuasion timeout](#section--dissuasion-timeout-)
[&nbsp;&nbsp;&nbsp;Chat idle timeout](#section--chat-idle-timeout-)
[&nbsp;&nbsp;&nbsp;Contact priority](#section--contact-priority-)
[Hooks](#section--hooks-)
<br>

The Routing section is where you configure the settings and the rules that regulate the distribution of contacts to agents.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8684715-routing.png",
        "routing.png",
        1436,
        822,
        "#c4bfbd"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
The different settings are grouped in tabs depending on the functionality.

#**Tags and Colors**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/1964475-routing_2.png",
        "routing_2.png",
        846,
        656,
        "#f6f6f5"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
##**Add tags to the Campaign**
You can assign one or more tags to the Campaign in order incoming contacts are distributed only the agents who have the same tags.

Further details on **how to use tags** are available at the following link: http://docs.vivocha.com/docs/how-to-use-tags

##**Add color**
You might want to assign a color to all the contacts came from a specific campaign, in order to easily identify them and distinguish from the ones coming from another campaign.
<br>
#**Pause**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/95d9797-routing_pause.png",
        "routing_pause.png",
        842,
        611,
        "#f7f7f7"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
##**Forced pause**
You can enable this feature not only for the campaign at hand but also at account level in the Settings > Routing section. The value set into the campaign replace the one inherited from the one set into the account. 

More information on Forced Pause and hot to set it on the account are available at the following link of this documentation:
http://docs.vivocha.com/docs/routing-config 
http://docs.vivocha.com/docs/media-switches-all#section-forced-paused

##**Show pending contacts when paused**
You can enable this feature to allow agents to see incoming contacts even when they are paused. 

You can configure this feature directly at the account level in the Settings > Routing section. 

The setting of the campaign overrides the account setting, which in turn can be changed by each single agent that enable/disable this feature directly in his/her from the Agent Menu of the agent console

More information available at:  http://docs.vivocha.com/docs/media-switches-all#section-the-pause-button
<br>
#**Transfer**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8d76299-Screen_Shot_2018-09-12_at_19.24.36.png",
        "Screen Shot 2018-09-12 at 19.24.36.png",
        833,
        619,
        "#f6f6f6"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
##**Transfer to busy agents**
You can enable this feature to transfer a contact also to busy agents in case no one have accepted it before. This reduce the possibility that it will be dissuaded.

##**Transfer back**
You can enable the feature that lets a transferred contact to return back and re-proposed to the agent who has transferred it in case it has not been accepted.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b8bc084-Screen_Shot_2018-09-12_at_19.25.31.png",
        "Screen Shot 2018-09-12 at 19.25.31.png",
        800,
        606,
        "#fafafa"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
##**Transferred contact priority**
You can set a value between 1 (highest) and 30 (lowest) to give to the contact a transfer priority; the default value of priority is set to 15.

Higher is the priority and more the transferred contact to an agent or to a transfer group will appear in a higher position in the queue of the pending contacts

##**Transfer failure timeout**
The transfer failure timeout is the dissuasion for a contact that has been transferred. This parameter can be different from the timeout set for the incoming contacts, if you want that the dissuasion event occurs faster or slower for the transferred contacts.
[block:callout]
{
  "type": "info",
  "body": "The transfer features described above can be configured at level of the account; more information available at the following link: http://docs.vivocha.com/docs/routing-config#section--transfer-"
}
[/block]
<br>
#**Routing Rules**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/45ef092-routing_rules.png",
        "routing_rules.png",
        841,
        758,
        "#f6f6f6"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
##**Contact routing rules**
Here you set the distribution algorithm to one of the five predefined ones (broadcast, skill-based, round-robin, least-loaded, dynamic).  All algorithms work by:
- assigning a score from 0 (minimum) to 1 (maximum) to each agent.
- creating groups of agents based on the their scores, up to a configurable number of groups.
- trying to distribute the contacts to each group in order

The only difference between the algorithms is how the score is calculated.

The strategy set by dafault is **broadcast**: The Broadcast strategy assigns the same score to all agents and contacts are distributed to all available agents in the same moment.

Other strategies all assign different scores to agents in different ways; by selecting one of these strategies the card expands to shows further parameters that you can configure:

**optional tags**
optional tags allow to improve the routing of contacts to the agents. The system will assign the contact to the agent that have the closest match with the set of optional tags.

**number of attempts of distribution**
how many attempts of distribution of the contact are performed 

**delay in seconds between consecutive attempts.**
the number of seconds elapsed between an attempt of distribution and the next one

###**Round-robin**
The Round-robin strategy assigns a higher score to the agents which haven't received contacts for a longer time. Contact will be proposed to an agent at time, starting from the agent with the highest score.
###**Skill-based**
The Skill-based strategy assigns an higher score to agents with the highest number of tags matching the optional tags of the Campaign.
###**Least-loaded**
The Least-loaded strategy assigns the highest scores are assigned to the agents with the lowest load.
###**Dynamic**
The Dynamic strategy uses a weighted combination of the Least Loaded, Skill-base e Round-robin strategies.
###**Custom**
In the Custom strategy you manually assign the routing weights to the parameters used in the calculation of the scores:
- agent load, 
- time since last assigned contact 
- optional tags matching
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b3c7fcc-custom_algorhytm.png",
        "custom_algorhytm.png",
        743,
        344,
        "#fbf9f9"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]
##**Dissuasion timeout**
The dissuasion timeout for a contact is the amount of time after which a message is shown to the users that have been waiting for an agent accepted the chat

The duration of this period of time can be set up as it needs, and when it expires, the users will be notified that there is no available agent that can receive the contact, instead of let them wait for a long time with no answer.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/4eeb4b4-dissuasion_time_2.png",
        "dissuasion time 2.png",
        1688,
        636,
        "#fafafa"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
##**Chat idle timeout**
An contact is *idle* when there is not exchange of messages between the customer and the agent, and sharing tools haven't been used for a specific period of time. You can set the value in second of this period.

The system evaluates idle contacts have not weight on the evaluating of the agent load.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/51aa40f-chat_idle_timeout.png",
        "chat idle timeout.png",
        820,
        331,
        "#f8f8f8"
      ],
      "sizing": "80",
      "border": true
    }
  ]
}
[/block]

[block:callout]
{
  "type": "warning",
  "body": "The chat idle timeout can be disabled by setting is value to 0. <br>\nThis means that contacts will always deemed as active, even when no messages are exchanged between the parts. This entails the contacts keep to have a weight in the calculating of the agent's load for the routing and distribution.<br>\n[➡ Read more about \"active and idle contacts, chat limit and agent's load\" in the Routing and distribution section](doc:routing-and-distribution#section-agent-load-assigned-active-and-idle-chats)"
}
[/block]
##**Contact Priority**
You can set a value between 1 (highest) and 30 (lowest) to give to the contact a priority in the queue of how they are proposed in the Waiting Contact section of the Vivocha Agent Console; the default value of priority is set to 15.

Higher is the priority and more the contact will appear in the queue.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/17315bf-contact_priority.png",
        "contact priority.png",
        833,
        327,
        "#f8f8f8"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
#**Hooks**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/22983b2-Screen_Shot_2018-09-14_at_16.51.13.png",
        "Screen Shot 2018-09-14 at 16.51.13.png",
        1809,
        1268,
        "#f6f6f6"
      ],
      "border": true,
      "sizing": "80"
    }
  ]
}
[/block]
You can link your Campaigns to the [External Services set in the Library](doc:vcb-external-services) of your account and use them in order to extend or change the standard functionalities of the platform.

External Services that a campaign can be linked to can be of different types and they allow to gain different results.

##**[Media Hooks](doc:vcb-external-services#section-mediahook)**
Using a Media Hook allows you to use an external service to calculate agent availability, defining the way in which media are shown to the users on the Engagement.

##**[CTI Events](doc:vcb-external-services#section-webhook)**
CTI events allow to you to be notified when specific Vivocha Events happen. These use the Web Hooks previously created in the Library. You can link one or more webhooks to the Campaing

##**[External Router](doc:vcb-external-services#section-external-router)**
The External Router allows external routing settings to be used, overwriting the Vivocha Routing settings.