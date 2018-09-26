---
title: Data Collection
excerpt: ''
---

# Data Collection

[Data Collection general settings](data-collection.md#section--data-collection-general-settings-) [Data Collection fields](data-collection.md#section--data-collection-fields-) [   Field advanced options](data-collection.md#section--field-advanced-options-) [      Translations](data-collection.md#section--translations-) [      Settings](data-collection.md#section--settings-) [Form Data Collection](data-collection.md#section--form-data-collection-) [Bot Data Collection](data-collection.md#section--bot-data-collection-) [Dialog Data Collection](data-collection.md#section--dialog-data-collection-) [   General prompts](data-collection.md#section-general-prompts) [   Field-oriented prompts](data-collection.md#section-field-oriented-prompts) [   Prompts templating and available variables](data-collection.md#section-prompts-templating-and-available-variables) [Customer Satisfaction Survey](data-collection.md#section--customer-satisfaction-survey-) [Data Collection advanced settings](data-collection.md#section--data-collection-advanced-settings-)

  
 \[block:callout\] { "type": "info", "body": "[➡ Read more about the \"How to use Data Collection and Surveys in a Campaign\" in our documentation](doc:vcb-web-engagement-widgets#section--data-collection-survey-)" } \[/block\] The Data Collection allows you to obtain information that will help agents handle customers' requests. Data can be asked directly to the user, through a form with fields to fill manually or automatically by fetching the information from the page the user is visiting in that moment in case these are available. To Users can be also asked to provide the same data in a more conversational way by simulating an interaction directly with an agent.

It's possible to access the general settings by clicking the Add New button to create a new data collection or simply on one of the objects already set in the account and represented by a box reporting information such as the name, the icon corresponding to the type, and a series of icons indicating the configured fields, and the button  :fa-ellipsis-v:  that give access to the commands to edit its settings and delete it. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/7234492-Screen\_Shot\_2018-08-20\_at\_15.18.25.png](https://files.readme.io/7234492-Screen_Shot_2018-08-20_at_15.18.25.png)", "Screen Shot 2018-08-20 at 15.18.25.png", 1436, 826, "\#c4c4c4" \], "border": true, "sizing": "80" } \] } \[/block\]

## **Data Collection general settings**

A Data Collection must have an identifier, a title and at least a field in order to be used.

Vivocha 6 supports three different types of Data Collection:

* Form
* Dialog 
* Bot 

You are asked to select one of the supported types from the drop-down list. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/4480fea-Screen\_Shot\_2018-08-23\_at\_12.35.43.png](https://files.readme.io/4480fea-Screen_Shot_2018-08-23_at_12.35.43.png)", "Screen Shot 2018-08-23 at 12.35.43.png", 1054, 408, "\#f7f7f7" \], "border": true, "sizing": "80" } \] } \[/block\] You can assign a different title to the Data Collection for each of the supported languages in the Campaign by clicking the  :fa-angle-down:  button to expand the drop-down list. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/de513f6-Screen\_Shot\_2018-08-20\_at\_16.21.08.png](https://files.readme.io/de513f6-Screen_Shot_2018-08-20_at_16.21.08.png)", "Screen Shot 2018-08-20 at 16.21.08.png", 1092, 676, "\#f5f5f5" \], "sizing": "80", "border": true } \] } \[/block\] To save the changes you click the  **:fa-save:  Save** button.

## **Data Collection fields**

To add fields to the Data Collection click on the Add Field button in the general info panel; the Data Collection fields section opens allowing to set the main properties of the field, which are:

* the **field id** that identify the field.
* the **field type:** selectable from a drop-down list showing all available types \(i.e: firstname, lastname, phone number, email, date, string, text area, ecc... \) so the system is able to use the correct format to apply to the field.
* the **field name** which is the text appearing in the label of the field. 
* a checkbox to state whether the field is **mandatory** or it is not.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/7259f05-Screen_Shot_2018-08-21_at_12.16.07.png",
    "Screen Shot 2018-08-21 at 12.16.07.png",
    1045,
    768,
    "#fafafa"
  ],
  "sizing": "80",
  "border": true
  ```

    }

  \]

  }

  \[/block\]

  Moving the mouse on the right side of each field two buttons apper commands that allow 

*  :fa-trash: : to eliminate the field 
*  :fa-cog: : to access the panel of the advanced options where it's possible to configure all its own properties.

The **Field Name** can be set for each supported language by clicking the  :fa-globe:  and opening the translation panel for that field \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e59d334-Screen\_Shot\_2018-08-21\_at\_12.19.13.png](https://files.readme.io/e59d334-Screen_Shot_2018-08-21_at_12.19.13.png)", "Screen Shot 2018-08-21 at 12.19.13.png", 846, 542, "\#d1d1d1" \], "sizing": "80", "border": true } \] } \[/block\] The interface of the details section where to configure all the field's properties is different depending the data collection type you are configuring.

### **Field advanced options**

When you access to the field detail section, in the top card you have reported the general info of the field: the **field identifier** and the **field type** with the drop-down list of the all available types that can be assigned \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/e3d621d-dc-field\_settings\_2.png](https://files.readme.io/e3d621d-dc-field_settings_2.png)", "dc-field settings\_2.png", 891, 338, "\#f7f7f7" \], "border": true, "sizing": "80" } \] } \[/block\] The second card has two tabs:

#### **Translations**

in Translations you have the **label** assigned to the field in the general settings section, as well as the **Placeholder** of the field, the translation for each language in use in the Data Collection.

You can modify the languages translations for this field by clicking the  :fa-angle-down:  icon on the right to expand the card. Depending on the field type, if available you could also configure a set of languages translation for the placeholder.

To apply the changes carried out to the translations click on the "Save" button \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/4365639-Screen\_Shot\_2018-08-21\_at\_16.14.32.png](https://files.readme.io/4365639-Screen_Shot_2018-08-21_at_16.14.32.png)", "Screen Shot 2018-08-21 at 16.14.32.png", 1085, 746, "\#f6f6f5" \], "border": true, "sizing": "80" } \] } \[/block\]

#### **Settings**

in this tab you set some properties for the validation and the automatic filling of the field

**Field properties**

Four checkbox to set if:

* the field is **visible/hidden** to the customer.
* the field is **required** in the Data Collection and needs to be always provided \(this checkbox is disabled by default if the field is hidden to the customer\)
* the field is **visible/hidden** to the agent.
* the field is **editable** by the agent 

The way these properties are set determine also the behaviour of the form and how it is presented to the user set and \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/93b92c7-dc-field-settings-3.png](https://files.readme.io/93b92c7-dc-field-settings-3.png)", "dc-field-settings-3.png", 1868, 916, "\#f8f8f8" \], "border": true, "sizing": "80" } \] } \[/block\]

**Validation**

data entered in the field can be valideted:

* by defining a **regular expression** that constrains the data input.
* by setting the **minimum and maximum length** of it.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/ee202fb-dc-fields-validation.png",
    "dc-fields-validation.png",
    895,
    323,
    "#fcfcfc"
  ],
  "border": true,
  "sizing": "80"
  ```

    }

  \]

  }

  \[/block\]

  **Automatic Filling**

  You can set a field in order that data can be filled automatically and passed directly to the data collection form. A data field can be auto-filled in two ways:

With a **constant** value of the type of the field \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/77994f6-dc-auto-filling-constant.png](https://files.readme.io/77994f6-dc-auto-filling-constant.png)", "dc-auto-filling-constant.png", 1097, 278, "\#fafafa" \], "border": true, "sizing": "80" } \] } \[/block\] Using a **Data Capture Variable** that can be selected from a dropdown list containing a collection of both "built-in variables" and, at the bottom, the **custom variables** that, when available, fetches the data directly from the page.

Custom data capture variables can be defined [Custom Variables](doc:vcb-custom-variables) section of the Library. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/1322dd8-dc-auto-filling-variable-2.png](https://files.readme.io/1322dd8-dc-auto-filling-variable-2.png)", "dc-auto-filling-variable-2.png", 1095, 377, "\#f8f7f7" \], "border": true, "sizing": "80" } \] } \[/block\] To apply all the changes carried out so far to the field just click on the  **:fa-save: Save Field** button

## **Form Data Collection**

Data collection forms are the common method to gather information from users, and it represents the standard when you are using the web Channel;

A data collection form can be filled manually by the user, or if these information are available in the page they can be directly fetched and pre-fill the form without showing it to the user. It's also possible to present a pre-filled data collection to give the opportunity to change some of the information automatically fetched.

Multiple solutions are granted and you can chose the more suitable one based on the specific scenario. It's in fact possible to configure the properties of the fields in order to make them mandatory or not, define the filling methods and make them visible or hidden to the agents and to the users who can be authorized to modify them or not. \[block:callout\] { "type": "info", "body": "in case of a satisfaction survey data collection, information can be collected when a contact has already ended." } \[/block\]

## **Bot Data Collection**

You can implement an alternative way to collect data using a Bot and associate it with a data collection. To do that you may use an existing Bot developed through the NLP \(Natural Language Processing\) platforms that we support, such as Watson, Dialog Flow or you can also create one from scratch using our Bot SDK APIs.

[➡ Read about the "Bot external services" in our documentation](doc:vcb-external-services#section-bot-agents)

It's important to point out that this is different scenario from having an agent, even though a bot agent or virtual assistant, that interact a user in a already on-going contact. This approach actually allow to carry out the the gathering of data from the user before a contact is really on going and before the connection with an agent on the other side, whether a human agent or virtual like a Bot agent, is really established. In some cases it may be more suitable that initial phase of collecting data would take place before and only then make the contact to start.

In this way it's possible to develop bots that are dedicated to collect data without they necessarily have to be able to carry out also more complex transactional activities.

When selecting Bot as type of the data collection a further setting field is shown and it needs to be configured: the Bot Agent that will be associated to the data collection. It is the external service to the platform thinked, built and trained to collect data from the user. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/916a1d3-Screen\_Shot\_2018-08-28\_at\_12.48.32.png](https://files.readme.io/916a1d3-Screen_Shot_2018-08-28_at_12.48.32.png)", "Screen Shot 2018-08-28 at 12.48.32.png", 1047, 489, "\#f9f9f9" \], "border": true, "sizing": "80" } \] } \[/block\] Bots developed through our Bot SDK or built and trained using a bot / NLP platform are seen in Vivocha as Bot agents that can be registered and integrated within the platform specifying few settings in the External Services section at Library. \[block:callout\] { "type": "warning", "body": "Clearly the data collection fields configured in the data collection must be congruent with the type of information that the Bot is able to collect: they must named with the same ids of the fields set inside the Bot to make referement to these same information" } \[/block\] Furthermore, if developed and trained in the correct way, nothing prevents the same bot to be suitable to execute more complex activities aside the collecting of data.

## **Dialog Data Collection**

The third data collection type supported is the Dialog Data Collector \(DDC\) is a conversational tool to collect data from the user. It essentially consists in a dynamically generated bot based on the configuration of a data collection without to implement any NLP technology interpreting natural language, or that uses artificial intelligence to perform the interaction with the user.

In such way the same information requested through the fields in a form manually filled by the user or, if are available, fetched from the page by using the custom variables, can be obtained through an dialogue style interface that simulates the interaction with the user.

Also in this case the dialog window for gathering the data from the user starts before the contact is really on going and before the connection with the virtual agent on the other side is really established.

Considering a data collection with the following fields: name, last name, email and phone number, where the first three fields are mandatory while the phone it's not \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/f875ae8-Screen\_Shot\_2018-08-23\_at\_16.51.49.png](https://files.readme.io/f875ae8-Screen_Shot_2018-08-23_at_16.51.49.png)", "Screen Shot 2018-08-23 at 16.51.49.png", 1037, 572, "\#fbfbfb" \], "sizing": "80", "border": true } \] } \[/block\] In place of a form and its the fields to fill, the data collector ask for the same data but through a dialog modality as if there was a bot or a real agent actually interacting with the user

While in a form the data collection fields will appear as shown on the left side in the image below, with the dialog style the request to get the same information are presented in the way on the right. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/7db94e8-Screen\_Shot\_2018-08-29\_at\_10.53.28.png](https://files.readme.io/7db94e8-Screen_Shot_2018-08-29_at_10.53.28.png)", "Screen Shot 2018-08-29 at 10.53.28.png", 1920, 1191, "\#dbe5ef" \], "sizing": "full" } \] } \[/block\] Fields that are not mandatory can also be skipped by simply selecting SKIP to continue to the next information.

Even if any kind of language interpretation is not used, the data collecting process through the dialog mode has its own validation rules of the entered data so for example, in case of an email address is not recognized as a valid one, you are asked to re-enter this data. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/f1e06f6-Screen\_Shot\_2018-08-29\_at\_18.01.32.png](https://files.readme.io/f1e06f6-Screen_Shot_2018-08-29_at_18.01.32.png)", "Screen Shot 2018-08-29 at 18.01.32.png", 1822, 1136, "\#e1e9f1" \], "sizing": "80" } \] } \[/block\] Furthermore at the end the data collected are shown in order it is possible to verify them; in case they were not entered properly, you can select those need to be provided again until they are approved. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/fe60f5f-Screen\_Shot\_2018-08-29\_at\_18.05.05.png](https://files.readme.io/fe60f5f-Screen_Shot_2018-08-29_at_18.05.05.png)", "Screen Shot 2018-08-29 at 18.05.05.png", 1803, 988, "\#c1d2e3" \], "sizing": "80" } \] } \[/block\] Beside supporting the features of a normal form-based data collection definition, like data types, validation default values, considering its conversational nature and in order to make this type of interaction as similar as possible to that you could have with a real agent, when configuring the fields of the data collection and defining the information you want to obtain from the user, you can also configure further dialog options as well as multiple different messages to display in place of the name of the field as it would appear in case of form data collection.

These customized messages and questions to send to the user are named **Prompts** and in a dialog type data collection they can be added in addition to the name given to the field label that would appear if the data collection would be a form.

They are of two categories: **general** and **field-oriented**: general prompts are the ones that can be configured by clicking on the button **Edit Dialog Options** at the bottom of the fields list. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/69ec774-Screen\_Shot\_2018-09-03\_at\_12.51.03.png](https://files.readme.io/69ec774-Screen_Shot_2018-09-03_at_12.51.03.png)", "Screen Shot 2018-09-03 at 12.51.03.png", 1038, 600, "\#fbfbfa" \], "border": true, "sizing": "80" } \] } \[/block\]

### General prompts

They can have different meanings and purposes depending on the different contexts in which are used in the interaction

* **Welcome messages:** a list of welcome messages or greeting
* **End of conversation messages:** a list of data collection ended/farewell messages or greeting

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/0903412-Screen_Shot_2018-09-03_at_18.30.35.png",
    "Screen Shot 2018-09-03 at 18.30.35.png",
    1059,
    805,
    "#f9f9f9"
  ],
  "sizing": "80",
  "border": true
  ```

    }

  \]

  }

  \[/block\]

* **Data Collection final messages:** messages to show when data collection is complete
* **Data Confirmation and recap messages:** a list of messages sent to the user to present a recap of collected data and to require a confirmation about it

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/0b1ecaf-Screen_Shot_2018-09-04_at_13.04.36.png",
    "Screen Shot 2018-09-04 at 13.04.36.png",
    1073,
    668,
    "#fafafa"
  ],
  "sizing": "80",
  "border": true
  ```

    }

  \]

  }

  \[/block\]

* **Wrong field chosen:** messages to propose to users to edit a collected info in case they want change something
* **Data collection complete messages:** messages to show when data collection is complete

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/9b6f7b3-Screen_Shot_2018-09-04_at_14.44.28.png",
    "Screen Shot 2018-09-04 at 14.44.28.png",
    1043,
    747,
    "#faf9f9"
  ],
  "border": true,
  "sizing": "80"
  ```

    }

  \]

  }

  \[/block\]

* **Error messages:** messages to send to the users in case of error or unexpected behaviour.

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/8316e0d-Screen_Shot_2018-09-04_at_14.55.28.png",
    "Screen Shot 2018-09-04 at 14.55.28.png",
    1035,
    627,
    "#fafafa"
  ],
  "border": true,
  "sizing": "80"
  ```

    }

  \]

  }

  \[/block\]

  **Field-oriented Prompts**

Differently from general prompts, these are related to a data field; going into the advanced options of the fields in place of the panel Translations there is a similar section that allows to set as many phrases as you want that could be proposed to the user when you ask for this data.

Some prompts can be multiple, instead of a single message. When multiple, they are shown to the user picking one by a random policy. When a prompt is not configured, a default message is presented to the user, infering it using the field type and associated labels.

* **Prompt messages:** a list of messages used to ask the user for the required data
* **Validation messages:** a list of messages sent to the usr when the data does't pass the configured validation rule

  \[block:image\]

  {

  "images": \[

    {

  ```text
  "image": [
    "https://files.readme.io/02f45a7-Screen_Shot_2018-08-31_at_17.51.49.png",
    "Screen Shot 2018-08-31 at 17.51.49.png",
    1086,
    801,
    "#fafafa"
  ],
  "border": true,
  "sizing": "80"
  ```

    }

  \]

  }

  \[/block\]

  **Prompts templating and available variables**

  Some prompts can be expressed through a template, in that case, at runtime, the DDC will try to complete the template using the available vars in the context of the conversation state.

Templates are expressed through the _moustache style_ and only variable names can be used \(no expressions or calculations\)

Examples:

* `The required number must be greater than {{min}} and less than {{max}}`
* `Thank you {{firstname}}, how old are you?`

The bot engine will try to resolve variables surrounded by `{{` and `}}` using the real value depending from the its context and state.

Currently, templates can be used only in the following **prompts**:

| Context | prompts |
| :--- | :--- |
| **DataCollection / general** | welcome |
|  | end of conversation |
|  | data collection completed |
|  | data recap message |
|  | data confirmation message |
|  | choose wrong field message |
|  |  |
| **DataCollection Field** | prompt |
|  | validation |

Moreover, you can use templates also in the **Message meta-fields** ;\)

**Available variables**

The variables that can be referenced at any time in templates are the following:

* fields' ids \(es. `firstname`, `lastname`, `city`, ecc...\)
* any property passed through the BotRequest `data` property
* the following **field** properties \(if configured\):
  * `label`
  * `min`
  * `max`
  * `minLength`
  * `maxLength`
* properties related to current **user's chat message**:
  * `userMsgBody`
  * `userMsgPayload`
* \(NOT YET IMPLEMENTED\) properties related to **settings**:
  * `botName`

Given a template, if even only one variable can not be resolved \(due to a typo or to a not yet available value\), the prompt containing the template is leaved as it is.

**Example**:

* DDC is asking for an email address, and the configured validation error prompt is: `I'm sorry {{firstname}}, you've entered a not valid email address ({{email}}), please check it.`
* User sends a not valid email
* validation occurs, address is not valid, DDC tries to compile the template but `email` variable is not yet filled \(because eneted value is not valid\), the prompt sent to user is the template itself.

**TIP**: In the previous example, to send the intended validation error message, the prompt containing the right template should be like the following: `I'm sorry {{firstname}}, you've entered a not valid email address ({{userMsgBody}}), please check it.`

## **Customer Satisfaction Survey**

Customer satisfaction surveys \(CSAT\) are used at the end of a contact to gauge how happy or unhappy the customer was with an experience with a product or service, or with a specific interaction with the customer service team.

These surveys can be used to segment customers based on satisfaction scores, measure relative customer satisfaction scores over time, or find insights for customer experience improvements.

CSAT are no more than post-contact data collections and therefore they can be presented to customers in the three different supported types, form, bot and dialog and you can configure the fields od the data collection to compose a questionnaire that collect the info you need. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/bdd9323-Screen\_Shot\_2018-09-05\_at\_12.21.24.png](https://files.readme.io/bdd9323-Screen_Shot_2018-09-05_at_12.21.24.png)", "Screen Shot 2018-09-05 at 12.21.24.png", 1020, 804, "\#fbfbfb" \], "border": true, "sizing": "80" } \] } \[/block\] Fields of a specific type named **Rating** can be added to the data collection to assign a score to possible questions to ask at the end of the interaction, defining in its settings a minimum and a maximum value and a rating style. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/220f33c-Screen\_Shot\_2018-09-05\_at\_12.18.38.png](https://files.readme.io/220f33c-Screen_Shot_2018-09-05_at_12.18.38.png)", "Screen Shot 2018-09-05 at 12.18.38.png", 1054, 329, "\#f7f7f6" \], "sizing": "80", "border": true } \] } \[/block\] In order to add a survey to a Campaign you must associate the so configured data collection to the single engagement widgets for which you want to collect info at the end of contacts.

[➡ Read more about the "How to use Data Collection and Surveys in a Campaign" in our documentation](doc:vcb-web-engagement-widgets#section--data-collection-survey-)

## **Data collection advanced settings**

The data collection functionalities have been empowered thanks the introduction of new options that allows for example to merge more separated data collection and make possible to add new fields dynamically and propose them depending on the channel, the interaction mode and the type of info that you want to collect.

Initially you might want to ask the user to provide only a certain set of information, and in case specific conditions and events are verified, to request for further data.

Distinct set of data could be requested in two or more different data collection depending on the scenario and they can be sequentially presented to the user.

The data collections can also be of diffrent type, so the first information are provided by filling a form while others can be asked in a conversational way by a Dialog or Bot type data collection.

In case two ore more data collections presented sequentially are of the same type they can be merged toghether and also the sequence of the fields and the order in which data are collected can be changed to improve the user experience.

In data collection configuration we have introduced the possibility to insert particular meta-data; these are of three types:

**message:** it shows a message in the form, or in the dialog window, for example to provide an explanation without the necessity to collect any data.

**break:** in a form-type data collection it allows to split the field in more pages introducing a separation with the introduction of a next button.

**section:** it allows to group set of data fields in different sections and merge them in case of two or more data collections proposed sequentially, if in each data collection there are sections having the same section ID's

Sections act as markers to delimitate distinct groups of fields; a section inserted in a data collection indicates that all the fields inserted after it, are part of the section itself until another one is defined by a further section meta-field.

If for example you want to have all the fields that collect personal information, such as the firstname, lastname , date of birth, etc... Under a distinct and separated section you have to insert a section type meta-data on the top of these fields that you could name "personalSection".

As mentioned above, it's possible to propose the user more data collections in a dynamic way depending on the scenarios and the events that may occur and in case it comes out that further data needs be collected.

This necessity comes out when within an engagement widget there are different configurations that make appear a media option rather than another depending on the scenarios and the events that may occur and when the needs to collect further data needs might come out.

These advanced settings are configurable in the section [**Proposed media**](doc:vcb-web-engagement-widgets#section--proposed-media-) of the single engagement widget ...

Think about the media **weblead** for example: if configured it can be an available option to request assistance or it could be proposed to the user in case there are not available agents, \(the weblead is a method of engagement that is always available since it's not depend from the agents' availability\), and therefore in order to be re-contacted later you could ask the user to provide the email address only in this case, in addition to the other fields that possibly have been collected from the data collection before to start a real contact.

If after the gathering of the personal info through the first data collection, in case of a weblead a second one is shown to ask the user to provide also his email address, if this field is under a section with the same id "personalSection" as well as the fields collected in the first data collection, it is appended just next the last field of this section and before eventual other fields that are external to it.

The image below shows how the email field under the personal section of the weblead data collection is appended after the last field of the personal section of the User info data collection, before eventual further fields that are not grouped in this section. \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/420008c-Screen\_Shot\_2018-09-11\_at\_18.18.35.png](https://files.readme.io/420008c-Screen_Shot_2018-09-11_at_18.18.35.png)", "Screen Shot 2018-09-11 at 18.18.35.png", 1900, 1408, "\#f6f6f7" \], "sizing": "full", "border": false } \] } \[/block\]

