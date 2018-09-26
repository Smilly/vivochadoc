---
title: "Routing"
excerpt: ""
---
Routing is a feature which allows a customer contact request, whether a chat, a phone call or a video call, to be automatically distributed to one or more available agents, according to a combination of predefined and configurable rules. This document describes how routing works in Vivocha.

In this section are all the settings that an admin can configure in the different ways to determine how contacts must be distributed among the agents.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/8f5f4e1-Screen_Shot_2015-07-28_at_11.30.24.png",
        "Screen Shot 2015-07-28 at 11.30.24.png",
        895,
        850,
        "#f7f7f7"
      ],
      "border": true
    }
  ]
}
[/block]
###**Routing presets:**
set the distribution algorithm to one of the five predefined ones (**broadcast, skill-based, round-robin, least-loaded, dynamic**).

###**Forced pause**
 automatically pause an agent if a starred contact is not accepted within delay seconds;

###**Show pending contacts while paused**
set whether incoming contacts are displayed in the Agent Desktop when in the paused state;

###**Idle chat timeout in seconds**
it must be between 60 and 600 (0 to disable it) and represents the number of seconds after which a chat if considered to be idle if no messages are exchanged and no sharing tools are used;

[block:callout]
{
  "type": "warning",
  "body": "The chat idle timeout can be disabled by setting is value to 0. <br>\nThis means that contacts will always deemed as active, even when no messages are exchanged between the parts. This entails the contacts keep to have a weight in the calculating of the agent's load for the routing and distribution.<br>\n[➡ Read more about \"active and idle contacts, chat limit and agent's load\" in the Routing and distribution section](doc:routing-and-distribution#section-agent-load-assigned-active-and-idle-chats)"
}
[/block]
###**Attempts**
It must be between 1 and 10 and indicates the maximum number of distribution attempts;

###**Delay between attempts in seconds** 
It must be between 5 and 300 and it indicates how long to wait before a new distribution attempt for a contact;

###**Routing weight** 
Relative weight of the three distribution component, load, idle, tags. Changing the weight to custom values automatically sets the algorithm to custom.

<br>
##**Transfer**
As shown in the image below, there are three more parameters that regulate the behaviour of the Transfer feature:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2167259-Screen_Shot_2017-03-27_at_09.59.52.png",
        "Screen Shot 2017-03-27 at 09.59.52.png",
        952,
        228,
        "#f8f8f8"
      ],
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
###**Disable Transfer bounce back:** 
if enabled, it prevents the contact appears again in the pending contacts queue to the agent who tried to transfer it. Finally the transfer timeout will expire and that contact will be dissuaded.

###**Allow transfer to busy agents:**  
if enabled a contact could be transferred also to the agents who in that moment are already busy.

###**Transfer contact priority**:  
it must be between 1 and 30, 15 is the value of priority assigned by default to a contact that is not transferred to a specific group, (i.e from an agent to another agent or towards a service). 

[block:callout]
{
  "type": "info",
  "body": "For more details on how Vivocha routes contacts, please refer to the **[Routing and Distribution](doc:routing-and-distribution)** page.",
  "title": "Info"
}
[/block]