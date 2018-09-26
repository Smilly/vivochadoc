---
title: Settings
excerpt: ''
---

# Settings

[Transfer groups](settings-1.md#section-transfer-groups) [Applications](settings-1.md#section-applications)

The Settings tab is used to see the whole saved information and settings for your account. For the Supervisor user this includes the location, language, users, shortcuts, services, phone numbers, applications, billing information, etc.

[**Users**](doc:users): In this section you can see all of the users for your account, add new users and edit or delete existing users. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/557263e-Screen\_Shot\_2016-11-16\_at\_12.47.13.png](https://files.readme.io/557263e-Screen_Shot_2016-11-16_at_12.47.13.png)", "Screen Shot 2016-11-16 at 12.47.13.png", 1440, 900, "\#e0e0e0" \] } \] } \[/block\]

## Transfer groups

Transfer groups are groups of tags with the same purpose and each agent that has at least one group's tag is considered to be a member of the group. From the group list is possible to:

* filter groups
* edit a group clicking on :fa-cog:
* delete a group clicking on :fa-times-circle-o:  

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/ZnCx1rESNORibqUcvNvw_transferGroups-1.png",
    "transferGroups-1.png",
    "3702",
    "2322",
    "#c4785a",
    ""
  ],
  "caption": "Transfer groups list"
  ```

    }

  \]

  }

  \[/block\]

  In order to create a new group, click on :fa-users: button.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/thfackuSbOW6zbft7L6g_Schermata%202016-06-23%20alle%2015.19.51.png",
    "Schermata 2016-06-23 alle 15.19.51.png",
    "3830",
    "2242",
    "#c4765b",
    ""
  ],
  "caption": "Transfer group creation"
  ```

    }

  \]

  }

  \[/block\]

  Each group has:

* a name
* a priority \( a value between **1** and **30**, default **15**, lower number means **high** priority \)
* one or more tags

## Transfer a contact to Transfer groups

In the Transfer app, if there are configured Transfer Groups, the services will be hidden. For each group is displayed the number of available agents and the available number of media slots that is the sum of all manageable medias by available agents. Each contact transferred to a group automatically receives group's priority. On the left of each group is displayed an indicator that could be **green** if the group can handle contacts, otherwise is **red**. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/SCeg9tmBQvOT2gAm53ag\_Schermata 2016-06-23 alle 16.40.41.png](https://files.readme.io/SCeg9tmBQvOT2gAm53ag_Schermata%202016-06-23%20alle%2016.40.41.png)", "Schermata 2016-06-23 alle 16.40.41.png", "3830", "2242", "\#60728a", "" \], "caption": "Transfer contact to a group: the logged agent is in the \"Sales\" group and it's the only available agent, so the indicator is red" } \] } \[/block\]

## Applications

[Email transcript](settings-1.md#section-email-transcript)

### Email transcript

Supervisors and Administrators can create new Email Transcript apps by selecting **DELIVERY SERVICE** from the available applications list.

\[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/Xxn8oUffSWWOdRzZf5ep\_Schermata 2016-07-07 alle 15.16.33.png](https://files.readme.io/Xxn8oUffSWWOdRzZf5ep_Schermata%202016-07-07%20alle%2015.16.33.png)", "Schermata 2016-07-07 alle 15.16.33.png", "2330", "1226", "\#335786", "" \], "caption": "Available application list on new app creation" } \] } \[/block\] In order to create the Emailer application, some required fields must be inserted in the configuration form:

* Application Name \(if no value is provided a default will be used\)
* Sender Email
* Subject

  The "Sender Email" has to be verified and the verification request can be done after the app is saved.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/ymI1ZXhsQgWXK5cm4gNi_Schermata%202016-07-07%20alle%2015.40.00.png",
    "Schermata 2016-07-07 alle 15.40.00.png",
    "2438",
    "1612",
    "#c4755d",
    ""
  ],
  "caption": "Email Transcript configuration form"
  ```

    }

  \]

  }

  \[/block\]

  It's also possible to edit html and text templates using a web based code editor.

  **IMPORTANT** data inside double brackets \(  \) will be replaced with real values, don't remove them unless you know what you're doing.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/qzG28caNTcCK0cDy8ex0_Schermata%202016-07-07%20alle%2015.40.12.png",
    "Schermata 2016-07-07 alle 15.40.12.png",
    "2296",
    "1590",
    "#2e4a55",
    ""
  ],
  "caption": "Html and text email templates are editables"
  ```

    }

  \]

  }

  \[/block\]

