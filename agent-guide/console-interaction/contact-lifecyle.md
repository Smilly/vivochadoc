---
title: Contact Lifecyle
excerpt: ''
---

# Contact Lifecyle

## What is a contact

A contact is an **interaction between a user and an agent**. The contact starts when the user interacts with the widget looking for the agent support, and finishes when one of them interrupt the interaction. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e7e68a6-contact.png](https://files.readme.io/e7e68a6-contact.png)", "contact.png", 500, 292, "\#fc842c" \] } \] } \[/block\]

## Contact Lifecycle

Contacts could have different outcomes: 1. **Successful**: contacts sent at least 3 bidirectional messages if it's a chat or starts using another media. 2. **Failed** 2.1 **Dissuaded**: this represents the number of contacts who requested a contact but were dissuaded after waiting a specified amount of time. 2.2 **Abandoned**: this represents the number of contacts that started a contact and left after waiting at least 10 seconds. 2.3 **Cancelled**: this represents the number of contacts who requested a contact but closed it before 10 seconds had passed. 2.4 **Other**

* **no\_interaction**: successfully established contacts, but without the minimum number of bidirectional messages
  * **unfinalized**: when a contact can't be characterized as successful, abandoned, cancelled, no\_interaction or dissuaded, it is counted as unfinalized. That may happen due to technical problems: network errors, page closed before the client software send the event, browser crashes, etc.

