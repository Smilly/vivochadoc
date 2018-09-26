---
title: Mobile SDK Release Notes
excerpt: This page contains the changelogs for the Vivocha SDK releases.
---

# Mobile SDK Release Notes

\[block:parameters\] { "data": { "h-0": "Platforms", "0-0": "[iOS SDK](mobile-sdk-release-notes.md#section-ios-sdk)", "1-0": "[Android SDK](mobile-sdk-release-notes.md#section-android-sdk)", "2-0": "[Cordova Plugin](mobile-sdk-release-notes.md#section-cordova-plugin)" }, "rows": 3, "cols": 3 } \[/block\]

\[block:api-header\] { "title": "iOS SDK" } \[/block\]

## v2.4.3

* Fixed UI misplacements during videochat
* Fixed an issue on media upgrade/downgrade during a call
* Fixed chat baloon width for Arabic text
* Forced LTR on the navigation bar as in the Android SDK

## v2.4.2

* Fixed the "Done" button misplacement in the attachment preview.

## v2.4.1

* Fixed an issue that prevented the speaker to be activated during a Video chat

\[block:api-header\] { "title": "Android SDK" } \[/block\]

## v2.4.4

* Fixed UI misplacements during videochat
* Fixed an issue that prevented taking attachment pictures during video call
* Fixed an issue on media upgrade/downgrade during a call
* Local view during videocall is now rounded as in the iOS SDK

## v2.4.3

* Fixed an issue that caused the underlying Activity to be visibile in the initial phases of a Video chat on some Android devices

## v2.4.2

* Fixed an issue that prevented the speaker to be activated during a Video chat

\[block:api-header\] { "title": "Cordova Plugin" } \[/block\]

## v2.0.10 - July 3rd, 2018

* Fixed UI misplacements during videochat
* Fixed an issue on media upgrade/downgrade during a call
* Fixed chat baloon width for arabic text
* iOS: Forced LTR on the navigation bar as the Android SDK
* Android: Fixed an issue that prevented taking attachment pictures during video call
* Android: Local view during videocall is now rounded as the iOS SDK
* Updated iOS SDK to version 2.4.3
* Updated Android SDK to version 2.4.4

## v2.0.9 - June 7th, 2018

* Fixed an issue that caused the underlying Activity to be visibile in the initial phases of a Video chat on some Android devices
* Updated Android SDK to version 2.4.3

## v2.0.8 - May 28th, 2018

* Fixed an issue that prevented the speaker to be activated during a Video chat
* Updated iOS \(2.4.1\) and Android \(2.4.2\) SDKs

## v2.0.7 - May 16th, 2018

* Fix the script for symlinks inside the iOS SDK folder \(fix for case insensitive file systems\)

## v2.0.6 - May 15th, 2018

* Fix the script for symlinks inside the iOS SDK folder

## v2.0.5 - April 26th, 2018

* Updated Android SDK to version 2.4.1 \(x86 native libraries for Media\)
* Added a new script to ensure needed symlinks inside the iOS SDK folder

## v2.0.4 - April 23rd, 2018

* Updated iOS and Android SDKs to version 2.4.0

## v2.0.2 - April 17th, 2018

* Removed references to the Current symlink in the iOS config on plugin.xml

## v2.0.1 - April 10th, 2018

* Fix compilation issue with Xcode 9.3

## v2.0.0 - March 7th, 2018

* Ionic support. To install:  

```text
ionic cordova plugin add "path_to_vivocha" --link
npm install "path_to_vivocha/ionic-vivocha" --save
```

## v1.3.28 - February 8th, 2018

* Fixed an issue that prevented the iOS device token to be sent to Vivocha in the correct form

## v1.3.27 - January 19th, 2018

* Fixed an issue parsing a boolean in the SetSideButton method on iOS

## v1.3.26 - January 12th, 2018

* Fixed an issue parsing some theme keys on Android

## v1.3.25 - January 8th, 2018

* Fix iPhoneX spacing in every orientation.
* Fix iPhoneX sidetab on the notch side.
* Fix application crash when the contact is not available anymore but the message queue is still running \(Android\).
* Fix application layout for RTL orientation \(Android\).

**Notes:** The iPhone X layout patches are not testable on the iPhoneX simulator, due to the missing differentation between simulator devices.

## v1.3.24 - November 2nd, 2017

* Fix version number that wasn't properly updated on plugin.xml \(v1.3.23 was still showing 1.3.22\).

## v1.3.23 - October 17th, 2017

* Fix sidetab badge not visible on the right on Android devices.
* Fix events propagation from native code to JavaScript when the event body contain entities or special characters \(e.g. quotes\).
* Fix method setBlockSideButton \(iOS\).
* Fix center position of custom logo in the chatviewcontroller.
* Fix minor glitches introduced by iOS 11:
  * Fix the "UI calls on non-main thread queues".
  * Fix attachment sorting issue on resume \(if you close and reopen the app with a valid chat\).
  * Fix missing title when the attachemnt is outgoing.

**Notes:** as written on plugin.xml notes, to allow the storage of a picture taken during a chat on iOS 11 you have to add the following description in your file Info.plist: `NSPhotoLibraryAddUsageDescription`

## v1.3.22 - September 19th, 2017

* Fix application crash on getTheme \(iOS\).
* Fix application crash when sendBtnTextColor = null on iOS.
* Removed default descriptions for the Info.plist file from the plugin install scripts to avoid the override of the 

  already used ones.

**Notes:** as soon as we removed the injection of the descriptions from our starting scripts, from this version, you have to add the following descriptions manually:

```markup
<key>NSMicrophoneUsageDescription</key>
<key>NSCameraUsageDescription</key>
<key>NSPhotoLibraryUsageDescription</key>
```

## v1.3.21 - September 11th, 2017

* Fix application crash on terminateHidingView \(iOS\).
* New internal FileProvider class to avoid AndroidManifest merge errors with other FileProviders.
* Fix NullPointerException on getContext calls \(Android\).

## v1.3.20 - June 30th, 2017

* Fix theme baloon corner radius default value.

## v1.3.19 - June 30th, 2017

* Fix setTheme and getTheme correct priority \(remote, local, default\). Now you don't need to pass all the values.

## v1.3.18 - June 28th, 2017

* Fix exception on getAgent when the agent has not yet joined the contact \(Android\).

## v1.3.17 - June 28th, 2017

* Fix exception on getAgent when the agent has not yet joined the contact \(iOS\).

## v1.3.16 - June 27th, 2017

* Fix attachment on Android 7 \(SDK Android 2.3.3\).
* Methods setDataCollection and storeSurvey now accepts also an array of DataCollection inputs \(previous version allowed

  to pass only one\).

* Add event _vivocha.receivedAgentPresence_ that notifies the Cordova application about the presence of an agent after

  the contact begins. 

**Notes:** This fix requires that you add a tag on your AndroidManifest. If you update the plugin using the cordova CLI this is automatically done by our install scripts, otherwise you have to add the following tag inside your `application` tag:

```markup
<provider
  android:name="android.support.v4.content.FileProvider"
  android:authorities="com.vivocha.sdk.provider.${applicationId}"
  android:exported="false"
  android:grantUriPermissions="true">
  <meta-data
    android:name="android.support.FILE_PROVIDER_PATHS"
    android:resource="@xml/vivocha_provider_paths"
  />
</provider>
```

## v1.3.15 - May 30th, 2017

* Fix dissuasion popup caused by a race condition on chat close when the chat window was not available yet.

## v1.3.14 - May 25th, 2017

* Fix the tag format expected by the server on _createContactWithDataCollection_.

## v1.3.13 - April 11th, 2017

* Fix language detection on the iOS SDK.
* Fix 2 lines lines layout for text field in the chatview.

**Notes:** the language detection works as following: 1. We try to find a local translation for the language returned by the device \(or for the language specified using the `overrideLanguage` method\). 2. If no translations are found, the first part of the language is used \(e.g._**en-US**_will be used as_**en**_\) to start a new search. 3. If still no translations are found, it will be \(e.g. in case of _**en**_, having _**en-GB**_ and _**en-US**_, _**en-GB**_ will be the one chosen\). 4. If no translations are found after all the steps, it will be used the default language \(_**en**_\).

## v1.3.12 - March 30th, 2017

* Add the storeSurvey method to push a survey to the Vivocha servers once the contact is closed.

**Notes:** to enable this feature you need to enable the survey editing the service from the Vivocha foundry. On the app side, you have to call the `storeSurvey` method once you receive the `vivocha.contactTerminated` event passing the contact id and the DataCollection object.

* The `storeSurvey(id, data_collection)` method update the contact data on the Vivocha servers with a DataCollection

  object.

  * _id_ {string} the contact id.
  * _data\_collection_ {object} is a DataCollection JSON object.

```javascript
document.addEventListener('vivocha.contactTerminated', function (data) {
  console.log('vivocha.contactTerminated', data);

  var val = prompt('How do you rate the chat?');
  if (val) {
    var notes = prompt('Do you want to submit additional notes?');
    vivochaPlugin.storeSurvey(
      data.contactId,
      {
        "name": "survey_anchored",
        "desc": "Survey",
        "data": [
          {
            "name": "rating",
            "type": "rating",
            "desc": "rating",
            "value": val
          },
          {
            "name": "note",
            "type": "text",
            "desc": "note",
            "value": notes || "-"
          }
        ]
      },
      function (res) {
        console.debug('vivochaPlugin.storeSurvey', res);
      },
      function (err) {
        console.error('vivochaPlugin.storeSurvey error', err);
      }
    );
  }
})
```

**Notes 2:** for security reasons, you can set the survey only once per contact. For the same reasons is not possible to push a survey data collection after 5 minutes from the end of the contact.

## v1.3.11 - March 22nd, 2017

* Add mapping to localization methods from SDK to Cordova.
* Fix overrideLanguage and addLocalization methods.

**Notes:**

* The `overrideLanguage()` method forces the SDK UI to use a different langage from the one configured in the device.
* The `addLocalization(lang, translation)` method allow to ovverride the strings:
  * _lang_ {string} the language of the translation object \(e.g. "en", "fr"\).
  * _translation_ {object} is a JSON object thit the following format:.

    ```javascript
    { "translation_key" : "translation" }
    ```

Example:

```javascript
vivochaPlugin.addLocalization("fr", {
  "button_close": "Fermer",
  "button_back": "Retour",
  "button_send": "Envoyer"
}, function(res) {
  console.log('vivochaPlugin.addLocalization', res);
}, function(err) {
  console.log('vivochaPlugin.addLocalization', err);
})
```

As you can se from the example above, you can specify only the strings that you want to override. For the others it will be used the default value in the curren language. If not present it will be used the english string. You can find the list of the available keys [here](https://github.com/Smilly/vivochadoc/tree/b817a1941984576e8436f7d5995548bf11c2df0a/Developer%20Guide/Mobile%20Services/strings_keys.txt).

## v1.3.10 - March 15th, 2017

* Fix crash on call of start/stop/start flow when the contact is on background.
* Add the following values on setTheme to change the theme colors in the loading spinner area:
  * _chatLoaderBackgroundColor_
  * _chatLoaderSpinnerColor_
  * _chatLoaderTextColor_

**Notes:** all the new parameters get an hex color value.

## v1.3.9 - March 1st, 2017

* Fix agent availability event after a stop and a new start.
* Fix crash when a Vivocha stop occurred when the app was moving to background \(Android\).

## v1.3.8 - February 7th, 2017

* Fix the behaviour differences between the iOS and Andoird setChatHeaderImage implementation.

**Notes:** from this version both platforms support a Base64 string image as parameter of setChatHeaderImage. This image will override the Vivocha logo on the chat view.

## v1.3.7 - January 26th, 2017

* Fix NullPointerException on agentUnavailable event \(Android\).
* Fix typo on agentUnavailable event \(iOS\).
* Fix behaviour differences on agentUnavailable event between iOS and Android.

## v1.3.6 - January 20th, 2017

* Improved detection of hidden Windows in order to find the best window add the Vivocha UI from the showChatView method.

  This behaviour was detected on WorkLight framework \(iOS\).

* Fix alignement on error message with the iOS counterpart.

## v1.3.5 - January 17th, 2017

* Fix message event propagation if the activity is on Background \(Android\).
* Fix received message outgoing status.
* Fix the behaviour differences between the iOS and Andoird setDataCollection implementation.
* Allow data collection to be set when a contact is in progress.

## v1.3.4 - December 12th, 2016

* Rename DDLog to \_\_VVCDDLog to avoid compatibility issues with IBM \(Mobile First\) \(iOS\).
* Remove volley as stand alone aar because now volley is part of vivocha code to avoid compatibility issues with IBM \(Mobile First\) \(Android\). Update plugin.xml to use the new library.

## v1.3.3 - December 7th, 2016

* Add agent data checks to availability events.
* Allow to call setDataCollection multiple times on Android as it was on iOS.
* Fix deletion of data collection passing a null value.

## v1.3.2 - November 29th, 2016

* Fix regression introduced by v1.3.1 on volley library and JavaScript events propagation.
* Fix regression on contact\_color param.
* Fix propagation of messages from visitor/agent on _**vivocha.textMessageSent**_ and _**vivocha.receivedTextMessage**_

  events.

* Fix propagation of _**vivocha.createNewContactDidSucceed**_ and _**vivocha.createNewContactDidFail**_ events.
* Fix propagation of _**vivocha.contactTerminated**_ and _**vivocha.contactTerminatedByOtherPeer**_ events.
* Fix return values on getTheme to Hex \(iOS\).
* Fix request permissions for camera \(Android &gt; 23\).
* Fix sideTab hiding state.
* Fix propagation of _**onAgentPresence**_ events.

## v1.3.1

* Fix vivocha.agentAvailable event \(Android\).
* Fix missing managing of the following events \(Android\):
  * _**vivocha.createNewContactDidSucceed**_
  * _**vivocha.createNewContactDidFail**_
  * _**vivocha.textMessageSent**_
  * _**vivocha.contactTerminated**_
  * _**vivocha.contactTerminatedByOtherPeer**_
  * _**vivocha.sdkStarted**_
  * _**vivocha.sdkStopped**_
  * _**vivocha.stop**_
* Fix sideButton text \(iOS\).

## v1.3.0

* First stable release.

