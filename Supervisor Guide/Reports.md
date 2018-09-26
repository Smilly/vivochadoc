---
title: "Reports"
excerpt: ""
---
<> (This is a comment, it will not be included)
[comment]: (in  the output file unless you use it in)

[//]: <> 
(it's worth to highlight the meaning of some of information that you can find when you export)
 the data of this report:
The fields busyness and fully_busy are functional only when the limit of chats for the agent is set. If the number of chats per agent is unlimited, those values are not computed (see the following link showing localization of the option at the Users configuration menu).
Those two values take in consideration how active the contacts are. In other words, an agent can have a limit of 5 chats, but if those are not active, that is, messages are not being exchanged in a timely manner, they stop being computed on the agent load until the parts start to exchange messages again. In this way it can be normal to see an agent with more contacts then what is actually configured, because the contacts aren't actually demanding too much effort. Other characteristic of those parameters is that they are sampled from the dynamic values in the system every few seconds. 
busyness: the total time during which the agent was at least partially busy, that is, had at least on interaction in progress.
fully busy:The total time during which the agent had reached the limit of chats, video and voice contacts configured to him/her. Note that an agent can have only one video or voice call at a time. In that case the agent will be considered fully busy independent of how many chats he/she has in progress.
Two other significant information are user_pause and forced_pause
user pause:  The total time during which the agent was in pause
forced pause: The total time during which the agent was put in forced pause by the system after not picking a contact.  The forced pause prevents the system showing undesired widgets when the agent forgets his console open in available state, but leaves his post or stops picking contacts because some other task requires his/her attention for too long. In such situation, the system will automatically put the agent in forced pause and stop assuming that he/she can take contacts)
-->
[//]: <>