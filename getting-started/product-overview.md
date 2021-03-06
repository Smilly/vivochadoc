---
title: Product overview
excerpt: This page will help you get started with the Vivocha Platform
---

# Product overview

{% hint style="info" %}
**If you currently run a previous major version of the Platform, please refer to relative documentation sites:**  
[Vivocha 5.0](http://docs.vivocha.com/v5.0/docs) - your domain is mX.vivocha.com  
[Vivocha 5.2](http://docs.vivocha.com/v5.2/docs) - your domain is nX.vivocha.com
{% endhint %}

Vivocha is **multi-channel online customer engagement and cloud-based service**, tailored to businesses looking to engage with customers online using the most effective communication channel at the right time and with the right agent. Vivocha enables businesses to seamlessly communicate with prospects and customers directly on the website, using any combination of VoIP \(audio and video\), chat, callbacks, and collaboration tools like assisted browsing and form and document sharing.

To get started with Vivocha you will first need an account. To create an account you can send an email at [sales@vivocha.com](mailto:sales@vivocha.com).

Before being able to use the Vivocha chat on your website you will have to paste the Vivocha Activation Code \(VAC\) onto any and all pages of your website where you would like to use the Vivocha widgets. You will find this code in your account's settings. It will look something like this, except that instead of "ACCOUNTID" there will be the name of your Vivocha account: 

```javascript
<script type="text/javascript">
(function(){
  window.vvc_ready_handlers = [];
  window.vivocha = { ready: function(cb) { window.vvc_ready_handlers.push(cb); }}
  var t = document.createElement("script");
  t.type="text/javascript"; t.async=true;
  t.src="//www.vivocha.com/a/ACCOUNTID/api/vivocha.js";
  var n=document.getElementsByTagName("script")[0];
  n.parentNode.insertBefore(t,n);
})();
</script>
```

When your account has been created and you have pasted the VAC into the necessary pages you will have a service automatically created. By logging on to your Vivocha Console the service will be activated and the visitors on your website will be able to communicate directly with you.

Test your service: after logging in to your Vivocha account @ [https://www.vivocha.com/login](https://www.vivocha.com/login) with your UserID and Password you will be on your Vivocha Console and ready to receive a chat, just wait for a customer to visit your page and ask for help!

