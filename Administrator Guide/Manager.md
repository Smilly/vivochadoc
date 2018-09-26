---
title: "Manager"
excerpt: "A smart tool that lets you create, edit, delete Vivocha resources"
---
Vivocha Manager is a web administration tool that allows users to create, edit, delete Resources such as Accounts, Subscription plans, Security profiles etc.
Each user can read a list of Resources and do different operations (Create, Read, Update, Delete) on Resource Items, according to the security profile associated to the user account.

* [Login and access](#section-login-and-access "Login and access")
* [Resources and Resource Items](#section-resources-and-resource-items "Resources and Resource Items")
* [Edit a Resource Item](#section-edit-a-resource-item "Edit a Resource Item")
* [Create a Resource Item](#section-create-a-resource-item "Create a Resource Item")
* [Toolbars](#section-toolbars "Toolbars")
* [Special editors](#section-special-editors "Special Editors")
* [Common operations](#section-common-operations "Common operations")

## Login and access
Manager is accessible at [MANAGER-URL-HERE](MANAGER-URL-HERE "Manager address") after the user successfully logs in at [LOGIN-URL-HERE](LOGIN-URL-HERE "Login page").

## Resources and Resource Items
A **Resource** is a definition of objects with the same structure. 
Example of Resources are: *Account*, *User*, *Profile* etc. 
A **Resource Item** is a single item of a specific Resource.
Example of Resource Items (reading resource *Account*) are: *Vivocha*, *Eptica*, *Genertel*, etc.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/gWmNxEwhQdintQZ87q3U_Schermata%202016-06-22%20alle%2011.23.16.png",
        "Schermata 2016-06-22 alle 11.23.16.png",
        "2808",
        "2258",
        "#40596e",
        ""
      ],
      "caption": "Manager's home page showing the list of available resources",
      "sizing": "smart"
    }
  ]
}
[/block]
The Manager's home page displays a menu and a grid of cards, one for each **readable** Resource by the logged user. When a Resource is selected (clicking on a card or on a menu item) a query is performed on database and a list of Resource Items is displayed to user.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/U3WuTy4Sou0YN4lGxNFW_Schermata%202016-06-22%20alle%2011.23.23.png",
        "Schermata 2016-06-22 alle 11.23.23.png",
        "2808",
        "2258",
        "#364d5d",
        ""
      ],
      "caption": "List of Resource Items for the Resource Account"
    }
  ]
}
[/block]
In the Resource Items list view the user can search for a specific item (the search is performed by item's **id**), sort the items list, create or delete an item.

**NOTE**
- the :fa-search: button triggers a search query and is disabled by default if no text is inserted in the search field (query can be performed also pressing ENTER) 
- :fa-plus-circle: and :fa-trash-o: buttons can be hidden if not allowed by user's account security profile

**IMPORTANT** 
the delete operation is irreversible.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/szwQWjSYSGynLxg2v74G_Schermata%202016-06-22%20alle%2015.09.00.png",
        "Schermata 2016-06-22 alle 15.09.00.png",
        "3354",
        "2322",
        "#364d5d",
        ""
      ],
      "caption": "Resource Items can be filtered with the top search bar and sorted by specific properties"
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/EtiW7awSg2fhHpo7DKRQ_Schermata%202016-06-22%20alle%2017.11.37.png",
        "Schermata 2016-06-22 alle 17.11.37.png",
        "3354",
        "2322",
        "#61738b",
        ""
      ],
      "caption": "The delete operation requires a confirmation in order to proceed"
    }
  ]
}
[/block]
## Edit a Resource Item

* [Default values](#section-default-values "Default values")
* [Going deep](#section-going-deep "Going deep")
* [Save changes](#section-save-changes "Save a Resource Item")

Clicking on a Resource Item, the editor will show the list of editable properties of the selected item. Each property has a name (example: *id*, *world*, *country*, etc), a description and one of the following types: **string**, **number**, **date**, **select**, **object**, **array**. According to the type, a different UI component (the **property editor**) is displayed on the right.

### Default values

Some properties can have a default value, that is displayed under the description.
Properties with :fa-ellipsis-v: button on the right allow users to quickly set value to property's default value. When a property is not required and has a default value, the default is used automatically, otherwise the user must set the desired value.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/oBG5kR9fQmSMe1unlQgj_Schermata%202016-06-22%20alle%2011.57.37.png",
        "Schermata 2016-06-22 alle 11.57.37.png",
        "2808",
        "2258",
        "#475f73",
        ""
      ],
      "caption": "Editing a Resource Item",
      "sizing": "smart",
      "border": false
    }
  ]
}
[/block]
### Going deep
A Resource Item can have multiple levels of depth. Properties of type **object** and **array** have a :fa-chevron-right: icon meaning that clicking on the property the editor will go into the selected property. Going deep, a "breadcrumbs" toolbar will appear, showing a button for each level of depth: clicking on a button the editor shows the list of editable properties for the selected level. On each level is possible to simply go back by clicking on the :fa-arrow-left: button.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/RvA0SuZTyY6N7Klg5wKA_Schermata%202016-06-22%20alle%2017.44.36.png",
        "Schermata 2016-06-22 alle 17.44.36.png",
        "3692",
        "2322",
        "#475f74",
        ""
      ],
      "caption": "Editor's breadcrumbs: clicking on \"BILLING\" the editor returns on BILLING's level"
    }
  ]
}
[/block]
### Save changes

A Resource Item can be saved on server clicking on the :fa-floppy-o: button.
**NOTE**
The :fa-floppy-o: button is displayed only in the first level of depth.

The edited Item must pass the Editor's validation before being stored on the server: all required properties must be provided and the required formats must be respected.
In case of error a popup message is shown on top right corner and the wrong property is highlighted with a :fa-exclamation-circle: icon.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/fxtWbvMSQXyVWVzMCQex_Schermata%202016-06-22%20alle%2012.29.21.png",
        "Schermata 2016-06-22 alle 12.29.21.png",
        "2808",
        "2258",
        "#475f72",
        ""
      ],
      "caption": "Errors on saving: items must pass the editor validation"
    }
  ]
}
[/block]
## Create a Resource Item
From the Resource Items list, according to account's security profile, users can create new items by clicking on the :fa-plus-circle: button on the right and then choose if start from an empty item or from a template, if there are templates available for the select Resource.

**NOTE**
When creating a new Resource Item, depending on the Resource, the editor may show editable properties that aren't shown on item update: this is because some properties are required and editable only on creation.
Example (for Resource Account): *owner_email*, *owner_password*.

**IMPORTANT**
New items are initially stored into the browser; nothing is saved on server until the user clicks on the :fa-floppy-o: button.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5eVwcyhJQQaAG29mwNh1_Schermata%202016-06-22%20alle%2011.27.38.png",
        "Schermata 2016-06-22 alle 11.27.38.png",
        "2808",
        "2258",
        "#61738b",
        ""
      ],
      "caption": "New Account creation"
    }
  ]
}
[/block]
## Toolbars
In addition to breadcrumb's toolbar, the editor has a special toolbar that allow user to do extra actions according to the type of property that is currently edited:
* JSON: opens a json editor with the value of the **current property** *(type object)*
* UNDO / REDO: cancel or repeat actions *(type object)*
* ADD ITEM: insert new items *(type array)*
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/5NP8rEnRmOIyP2juQa3w_Schermata%202016-06-22%20alle%2012.08.28.png",
        "Schermata 2016-06-22 alle 12.08.28.png",
        "2808",
        "2258",
        "#475f73",
        ""
      ],
      "caption": "The editor toolbar when editing an object"
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/2vR47nUrQtC1Rh1m8MKk_Schermata%202016-06-22%20alle%2012.12.25.png",
        "Schermata 2016-06-22 alle 12.12.25.png",
        "2808",
        "2258",
        "#465e73",
        ""
      ],
      "caption": "The editor toolbar when editing an array"
    }
  ]
}
[/block]
** NOTE **
The JSON editor is shown in readonly mode. Edit mode can be activated clicking on **EDIT**.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/qkq2EPl6S6uZFdJAxRXE_Schermata%202016-06-22%20alle%2012.26.51.png",
        "Schermata 2016-06-22 alle 12.26.51.png",
        "2808",
        "2258",
        "#8b8e91",
        ""
      ],
      "caption": "JSON Editor view"
    }
  ]
}
[/block]
## Special editors

### "oneOf" properties
Some properties can be edited in different ways, using different property editors. This properties are called **oneOf** properties.
Example: the name of a Plan, can be saved as string or as object.
When the editor loads **oneOf** properties, the user has to select how to edit it. If the loaded property already has a value, the editor automatically detects the property editor.
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/W94k5UrLQ865kA2EUEx7_Schermata%202016-06-22%20alle%2018.59.13.png",
        "Schermata 2016-06-22 alle 18.59.13.png",
        "3570",
        "2322",
        "#475f74",
        ""
      ],
      "caption": "Select the desired property editor"
    }
  ]
}
[/block]

[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/PCoidgQsReWICNf3NEgq_Schermata%202016-06-22%20alle%2018.59.41.png",
        "Schermata 2016-06-22 alle 18.59.41.png",
        "3570",
        "2322",
        "#475f74",
        ""
      ],
      "caption": "The \"string\" property editor was selected"
    }
  ]
}
[/block]
**NOTE**
- For oneOf properties the property editor can always be changed. By clicking on :fa-times-circle: button, the selected editor is reset to initial state.
- Sometimes a property value can be set as NULL.

## Common Operations
* [Create a Template](#section-create-a-template "Create a Template")


### Create a Template ### 
Templates are special resources that currently cannot be created from the Resource Items list.
In order to create a new Template Resource Item, user must select the target Resource, create a new Item and fill the desired values.
When the editing is done, clicking on the :fa-floppy-o: the editor will ask if save as new Template or as new Resource Item for the selected Resource.

Steps:
1. Select a Resource from the Manager home
2. Create a new Resource Item ( :fa-plus-circle: button ) and insert the desired values
3. Click on :fa-floppy-o: button
4. Select **SAVE AS TEMPLATE**
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/UKYM98nToqUwkmaNowtn_Schermata%202016-06-22%20alle%2012.43.18.png",
        "Schermata 2016-06-22 alle 12.43.18.png",
        "2808",
        "2258",
        "#72762d",
        ""
      ],
      "caption": "Saving new Resource Item as Template"
    }
  ]
}
[/block]