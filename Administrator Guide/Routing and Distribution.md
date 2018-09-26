---
title: "Routing and Distribution"
excerpt: ""
---
[How routing works](#section-how-routing-works)
[Agent Filtrering](#section-agent-filtering)
[Contact Distribution](#section-contact-distribution)
[&nbsp;&nbsp;&nbsp;Custom Contact Distribution](#section-custom-contact-distribution)
[Agent load, assigned, active and idle chats](#section-agent-load-assigned-active-and-idle-chats)
[Failed Distribution and Forced Pause](#section-failed-distribution-and-forced-pause)
<br>

Routing is a feature which allows a customer contact request, whether a chat, a phone call or a video call, to be automatically distributed to one or more available agents, according to a combination of predefined and configurable rules. This document describes how routing works in Vivocha.

#How routing works
The process of routing a customer contact request to an agent goes through four distinct phases:
1. **pre-routing**, during this phase Vivocha determines if a contact request is possible at all, verifying that service configuration rules are satisfied and that there is at least on available agent who could handle the request. Usually, if the preconditions are not verified, either no engagement widget is displayed to the customer or the customer is presented only with the options to request an offline contact (weblead, call back later);
2. **contact creation**, immediately after the customer requests to interact with an agent, Vivocha attempts to create a new contact. During this phase, the system builds the list of all the agents that are eligible to handle the request. If the list is empty, the contact creation request is rejected: this event is recorded in the reporting tools are a "no_agents" dissuasion, and it can happen if the availability of agents changes between pre-routing and contact creation;
3. **route planning**, the distribution plan for the contact is decided: by default, the contact request is to be forwarded to all the agents in the list simultaneously. Enterprise account can configure alternative distribution algorithms, such as round-robin, skill-based and more;
4. **distribution**, the contact is distributed to the agents according to the distribution plan.

#Agent Filtering
Both phases 1 and 2 of the routing process require a list of eligible agents: in the case of the pre-routing, the list is used to decide whether to display an engagement widget and what media are available. When creating the contact, the list is needed to make sure that the contact being requested can be served by an agent.

The process of building the list is called **agent filtering** and an agent is included in the list if she/he satisfies all the following criteria:
* The agent must be logged-in and connected to Vivocha using the Agent Desktop (or the Vivocha Agent SDK);
* The agent must be ready to accept contacts (i.e. not paused);
* The agent must be configured to handled the requested media type;
* The agent must not have disabled the requested media in her/her Agent Desktop;
* The agent must be using a browser capable of handling the requested media; (e.g. Video requires a WebRTC-capable browser, like Chrome and Firefox)
* If the service for which the agent list of being created is tagged, the agents must have at least all the main tags of service (i.e. the main/required tags of the service must be a subset of the agent's tags);
* The current work load of the agent must be low enough to handle the load of new contact.

The load of a contact is the load of the heaviest media in a contact, which in turn is calculated using max number of concurrent sessions an agent can handle for each media type. For example, suppose an agent is configured with following media limits:
[block:parameters]
{
  "data": {
    "h-0": "Media",
    "h-1": "Max concurrent sessions per agent",
    "h-2": "Load increase per session",
    "0-0": "Chat",
    "1-0": "Voice",
    "2-0": "Video",
    "0-1": "4",
    "0-2": "25%",
    "1-1": "1",
    "1-2": "100%",
    "2-1": "1",
    "2-2": "100%"
  },
  "cols": 3,
  "rows": 3
}
[/block]
Each chat handled by the agent will increase her/his load by 25%. If, the agent is handling 3 chats, the load is 75%. If the agent is handling 4 chats, or a single voice or video call, the load is 100% and she/he will not be available to handle new contacts.

If a contact includes both chat and audio, the load is not 125%, but rather the load of the most expensive media, in the case 100%.

The load of an agent is calculated by:
* adding the load of all active contacts being handled by the agent;
* adding the load of all pending **starred** contacts;
* subtracting the load of all **idle chat** contacts.

A **starred contact** is a contact that is exclusive to the agent: it could either be a contact that was transferred directly to the agent by another agent, or distributed only to the agent (no other agent is currently eligible to handle it). The name comes from the fact that this type of contacts have a "star" when displayed in the waiting contacts list.

An **idle chat** contact is a contacts whose only active media is chat and it has being idle (no messages being exchanged and no sharing tools being used) for more than the configurable time out (default 60 seconds). Idle chats can be disabled setting the timeout to 0 in the routing settings.

#Contact Distribution
The default algorithm used to distribute contacts to agents is **broadcast**: new contacts are displayed simultaneously in the Agent Desktop of all agent that pass the Agent Filtering process.

This algorithm, which is also the only one available to non-enterprise accounts, is suitable for most small online contact center and guarantees the best possible response time: the first agent to click on the pending contact will be assigned to it. The average response time of the contacts is exactly the same as the average response time of the agents working on them.

In addition to the default algorithm, enterprise accounts have access to four other algorithms and a configuration tool to define custom ones: **skill-based, round-robin, least-loaded** and **dynamic**.

All algorithms work by:
* assigning a score from 0 (minimum) to 1 (maximum) to each agent
* group agents based on the their scores, up to a configurable number of groups
* trying to distribute the contacts to each group in order

The only difference between the algorithms is how the score is calculated:
* **broadcast**, the default, all agents are assigned the same score (0) and are therefore all inserted into the same group and tried at the same time;
* **skill-based**, the highest score is assigned to the agents that has the best match with the optional tags of the contact (the more optional tags of the contacts the agent has, the higher her/his score);
* **round-robin**, agent scores are assigned according to the amount of time passed since the last time a contact was accepted;
* **least-loaded**, the highest scores are assigned to the agents with the lowest load;
* **dynamic**, a combination of skill-based, round-robin and least-loaded.

The number of distribution attempts, called **steps**, and the **delay** between steps are configurable parameters and their default values are respectively **3** and **12** seconds. Understanding these parameters and how they affect the distribution of contacts is very important to obtain a good performance.

The following examples describe the effect of different step and delay settings. The examples will use the least-loaded algorithm: as explained above, the other algorithms only differ in how the agents' scores are calculated.

Suppose we have the following **available** agents (i.e. agents that passed the filtering phase):
[block:parameters]
{
  "data": {
    "h-0": "Agent ID",
    "h-1": "Current chats",
    "h-2": "Current load",
    "0-0": "Agent1",
    "0-1": "0",
    "0-2": "0%",
    "1-0": "Agent2",
    "2-0": "Agent3",
    "3-0": "Agent4",
    "4-0": "Agent5",
    "1-1": "1",
    "1-2": "25%",
    "2-1": "1",
    "2-2": "25%",
    "3-1": "2",
    "3-2": "50%",
    "4-1": "3",
    "4-2": "75%"
  },
  "cols": 3,
  "rows": 5
}
[/block]
In our first example will use 4 steps and a 6 seconds delay. Vivocha creates at most 4 groups of agents, which in our case are:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/09768ca-Screen_Shot_2017-03-26_at_19.56.05.png",
        "Screen Shot 2017-03-26 at 19.56.05.png",
        466,
        296,
        "#50a156"
      ],
      "border": true
    }
  ]
}
[/block]
The contact is forwarded immediately to Agent1: Subsequently, if she/he doesn't accept it in 6 seconds, it's forwarded to agents Agent2 and Agent3 together, then in 6 seconds to Agent4 and so on.

Settings the steps to 3 would produce the following results:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7e198b5-Screen_Shot_2017-03-26_at_19.56.15.png",
        "Screen Shot 2017-03-26 at 19.56.15.png",
        461,
        293,
        "#52a158"
      ],
      "border": true
    }
  ]
}
[/block]
Similarly, using two steps will have all agents except Agent1 on the second attempt. Using a single step produces the same result as using the broadcast algorithm:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/7654213-Screen_Shot_2017-03-26_at_19.56.33.png",
        "Screen Shot 2017-03-26 at 19.56.33.png",
        465,
        305,
        "#4da354"
      ],
      "border": true
    }
  ]
}
[/block]
##Custom Contact Distribution
In addition to the five predefined distribution algorithms (**broadcast, skill-based, round-robin, least-loaded, dynamic**), Enterprise accounts can defined **custom** ones through the advanced routing settings interface.
Custom algorithms are defined by selecting the relative importance of the three components that make up the agent score:
* **load**, load percentage of the agent;
* **idle**, time passed since last time an agent accepted a contact;
* **tags**, number of matching optional tags the the request.

Possible range of values to the three components is from 0 to 1, where 0 means that the component will be ignored, while 1 means it'll have to maximum weight.
*Please note that for the tags component to be used, it is necessary the configure services with optional tags.*

#Agent load, assigned, active and idle chats
The maximum number of chats that an agent is able to handle simultaneously is not constant. Actually it can vary depending on the state of the chats [assigned](doc:how-to-handle-a-contact#section-assigned-contacts-section) to him, whether they are **active** or **idle**.

A chat is active when the agent is interacting with the user, as messages have been exchanged before the expiring of an amount of time which is specified by a parameter. 

On the other hand a chat is idle when, even if it still on going and the user is at the other side, no messages have been exchanged within the set amount of time, and actually the agent is not engaged with him. When in this state, chats do not affect his total load.  

The parameter that set the duration of this interval is named **idle chat timeout** and it can be configured at level of the [Account](https://docs.vivocha.com/docs/routing-config#section--idle-chat-timeout-in-seconds-) or directly for the single [Campaign](doc:vcb-routing#section--chat-idle-timeout-).

The Media slider in the [User settings](doc:admin-users) allows to enable him to accept voice and video contacts, along with the number of the chats.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/0ac45f0-Screen_Shot_2018-04-10_at_18.53.54.png",
        "Screen Shot 2018-04-10 at 18.53.54.png",
        523,
        170,
        "#e2dfde"
      ],
      "border": true
    }
  ]
}
[/block]

[block:callout]
{
  "type": "warning",
  "body": "Actually this value represents **the minimum number of the chats that must be active at the same time so the System consider the agent as busy.**<br>\nIt's important to point out that it do not necessarily corresponds to the total number of contacts that could be assigned to an agent.<br>\nThis limit in the number of chats does not prevent him to accept and manage more others: in case one or more of the assigned chats are idle, the agent is not more deemed as busy by the System, consequently the contacts can be distributed also to him.<br>\nThe main purpose of this value in the number of chats it's to point out when the System have to consider the agent as busy so to build the distribution list of those are eligible to handle the request and to evaluate whether keep showing the Engagement Widget to users or not."
}
[/block]
#Failed Distribution and Forced Pause
Ideally a contact should always be accepted as quickly as possible, and always at the first attempt/step. When this doesn't happen, it obviously translates into a poor customer experience, with customers having to wait for a long time for their contact requests to be picked up.

There are several possible reasons behind this kind of problems:
* agents are not instructed to accept contacts quickly;
* agents are failing to set their state to "paused" when leaving the agent desktop unattended;
* agents are more loaded than the system believes they are.

While the first two can be solved easily with better agent training and monitoring, the last one could be caused by a sub-optimal configuration of the routing parameters. For instance, in a contact center where the skills of the agents are very heterogeneous while the incoming requests tend to be mostly homogeneous (i.e. most customers requests skills that only few agents have), the skill-based routing will tend to overload some agents, leaving other relatively idle.
In this scenario, a possible solution could be the use of a custom algorithm that gives importance to both the agent skills/tags and the agent load.

In any case, Vivocha by default provides a safeguard mechanism, that tries to minimize the effect of overloaded or missing agents: it's called **Forced Pause**, and it automatically puts an agent into the **paused** state whenever she/he doesn't accept a starred contact. The agent won't be included in any future contact distribution plan until she/he explicitly returns to the **ready** state. The feature can be disabled in the advanced routing settings.