---
title: "Contacts Report"
excerpt: ""
---
In the Contacts Report you can see the data collected on the various contacts for your account, you can also see a chat history after clicking on a specific contact.
 
On your Vivocha Console, click on "Reports", then on "Contacts":
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/cf04bc9-Screen_Shot_2017-02-20_at_15.36.27.png",
        "Screen Shot 2017-02-20 at 15.36.27.png",
        1439,
        824,
        "#ececeb"
      ],
      "border": true,
      "sizing": "full"
    }
  ]
}
[/block]
By clicking the dropdown bars on the top you can access the Filter Panel and select which data visualize by filtering services, agents and media. You can also determine the desired period, selecting among the last 7, 15 or 30 days or by choosing a starting date and ending date. 

For the contacts you can also submit the query for the search of a specific word or a text.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2808bb1-Screen_Shot_2017-02-21_at_11.46.49.png",
        "Screen Shot 2017-02-21 at 11.46.49.png",
        1147,
        347,
        "#eaeaea"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
The contact list is divided into 6 different sections:

* **Contact Request Time:** shows the time and date that the contact was accepted
* **Agent: shows the name:** of the agent that accepted the contact
* **Duration:** represents the amount of time that the contact lasted
* **Contact Type:** shows the media of the contact
* **User Nickname:** shows the name of the customer that requested a contact (or "Customer" if undefined)
* **Service:** shows the name of the service that the contact was requested on

##Contact Details Page
If you select a particular chat session from the contacts list you will enter the **contact details page** where you can see numerous info about this contact:
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/b5ed1ed-Screen_Shot_2017-02-22_at_12.05.28.png",
        "Screen Shot 2017-02-22 at 12.05.28.png",
        1919,
        1011,
        "#e5e6e4"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
###General information
here are reported the detailed info for the single contact:
* The name of the **customer** if he has been identified by the system
- the **agent** who managed the contact
- its **duration**
- the timestamp of the **contact request**.
- from which **IP** address came the contact (with the possibility to ban this IP in case of harassment)
- the georeferenced info about the **position** of the customer with the possibility to visualize it in a map
- the **service** from which the contact came through
- the **first page** from where the contact has been requested
- the number of **messages** of the conversation
- the number of the **video calls** 
- the number of the **audio** session 
- the customer's **operative system** 
- the **browser** he used

###Data collection information
here are reported the data collected by the data collection widgets placed onto a service before starting the chat and which allow the agents to get more information about customers by adapting the customer service directly to the individual. 

###Contact history: visited pages and chat transcript
In addition to these information, below in the page you find the history of the contact, reporting in sequence all the website pages visited by the customer during the interaction, indicating for each of them:
* the name
* the time when he landed on it
* the staying time in that page 
* the corresponding URL

Very helpful for a supervisor also is to have the entire transcript of the conversation between customer and the agent, with all the exchanged messages and the possibility to download eventual embedded attachments as well as the ability to reproduce the recording and download the single registration both for the agent and the customer.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/c28612e-Screen_Shot_2017-02-23_at_12.21.16.png",
        "Screen Shot 2017-02-23 at 12.21.16.png",
        1919,
        1005,
        "#e6e5e3"
      ],
      "sizing": "full",
      "border": true
    }
  ]
}
[/block]
<br>
###The possible outcomes of the contacts are: 

**successful**
to be deemed as a successful, a chat must have a minimum number of 3 messages exchanged from both sides, in particular they must be bidirectional with at least one message from each side and a minimum of 3 messages in total.

**no_Interaction**
contacts without the minimum number of 3 bidirectional messages are considered as  no_interaction. They could include also contacts where the connection has been established but due to network problems it's not possible to send and/or receive messages and to start the interaction.


**cancelled**
relies on a event sent by the client browser, it happens when the client closes the chat **before 10 seconds** and before an agent joins the contact. In some cases due to network problems or to the browser being closed the event may be lost.

**abandoned**
relies on a event sent by the client browser, it happens when the client closes the chat **after 10 seconds** and before an agent joins the contact. In some cases due to network problems or to the browser being closed the event may be lost.

**dissuaded**
relies on a event sent by the client browser, it is triggered when the client waits that an agent accepting his contact request for more than amount of time defined in the dissuasion configuration (the dissuasion timeout is currently set to 30 seconds). 

**unfinalized/failed/other**
when a contact can't be classified as successful, abandoned, cancelled, no_interaction or dissuaded, it is counted as failed. That may happen due to technical problems: network errors, page closed before the client software send the event, browser crashes, etc.


**transferred**
transferred contacts 


## Download Export
All our reports can be download thanks to the "Download export" button, which will allow you to send a .xls file to an email address.
[block:callout]
{
  "type": "warning",
  "body": "The data export is not immediate. You will receive an email with the download link when the data will be ready for the export."
}
[/block]