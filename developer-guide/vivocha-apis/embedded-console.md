---
title: Embedded console
excerpt: ''
---

# Embedded console

The embedded console feature allows you to manage Vivocha contacts inside third-party systems like CTIs.

In particular, the embedded console, is a reduced Agent Console specific for managing a single contact \(all the features not related to the contact managed are disabled, i.e. new contact notifications, report tools, media managing etc.\).

## Requirements

To use this feature you first need to activate external routing for new incoming contacts. To do that, you must subscribe to \(at least\) the "new" contact event using the [Subscribe API](http://docs.vivocha.com/display/VVCJ/Subscribe+to+CTI+Events), passing an additional query parameter, `external_routing=1`, that will disable the notification of incoming contact to any open Vivocha Console.

After you received the new event and the CTI has assigned the contact to the agent, call the [Routing token](http://docs.vivocha.com/display/VVCJ/Routing+Token) web service:

```text
https://<world>.vivocha.com/a/<account>/api/_/contact/routingToken/?cid=<contactid>&user=<agentid>
```

The response will contain the embedded console url, that you need to forward to the third-party agent interface.

## Simple integration

The Url can be opened directly in a new window/iframe in the agent's browser. The token url will automatically login the agent and will render the embedded version of the agent console for the specified contact.

### Example:

```markup
<iframe src="https://www.vivocha.com/a/<account>/token/2ef4689020385757ed4b3e816555aa5c"></iframe>
```

The Iframe will contain a Vivocha Console dedicated to the single contact: \[block:image\] { "images": \[ { "image": \[ "[https://files.readme.io/3a8bc9a-Screen\_Shot\_2015-11-11\_at\_16.06.17.png](https://files.readme.io/3a8bc9a-Screen_Shot_2015-11-11_at_16.06.17.png)", "Screen Shot 2015-11-11 at 16.06.17.png", 1561, 680, "\#ebf2f2" \], "border": true, "sizing": "full" } \] } \[/block\]

## Integration using the Embedded Console SDK

The best approach to integrate the Vivocha Embedded Console inside your Agent Desktop application, is to include the [Vivocha Embedded Console SDK](https://m1.vivocha.com/a/_/api/doc/#VivochaEmbeddedConsoleManager) and use the method `vivocha.openConsole` to inject the iframe in the page \(reference [here](https://m1.vivocha.com/a/voxdem1/api/doc/VivochaEmbeddedConsoleManager.html#.openConsole)\).

This method returns a promise that is resolved to a [VivochaEmbeddedConsole](https://m1.vivocha.com/a/_/api/doc/VivochaEmbeddedConsole.html) object from which you can attach to the contact events, interact with the console interface, manage the apps and more.

## Sample application

You can find a sample application that implements the Embedded Console flow using the **Embedded Console SDK** on GitHub at this url: [https://github.com/vivocha/sample-ec](https://github.com/vivocha/sample-ec).

