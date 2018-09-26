---
title: Penetration Testing
excerpt: ''
---

# Penetration Testing

\[block:callout\] { "type": "danger", "body": "**Running penetration tests without our authorization is strictly prohibited and will be considered a cyber attack and it will be reported to the authorities.**\nYou are responsible for any damages to Vivocha or to Vivocha customers that are caused by your penetration testing activities." } \[/block\] Penetration Tests can be executed by our enterprise customers on request.

In order to get the authorisation you must submit your request to support@vivocha.com **three weeks prior to your desired date**, specifying the following information:

* Start date and time
* End date and time
* Company Name that will perform the tests
* Your Contact at the Company \(person in charge of the test in such company\)
* Phone and Email address
* Scanning IP addresses \(Source\)
* Total Bandwidth \(Please provide expected Gbps\)

We will forward this data to our provider that will let us know if we can do it within three working days.

Testing is **not authorized** until our provider validates the information and sends an authorization email to the requesting party containing an authorization number.

We will provide a dedicated production environment unconnected to the other customers' accounts in which you can. \[block:callout\] { "type": "warning", "body": "Additional charges may apply to setup the penetration tests dedicated environment." } \[/block\]

\[block:callout\] { "type": "warning", "body": "You **cannot** run tests on instances other than those provided or outside the scheduled days." } \[/block\]

\[block:callout\] { "type": "info", "body": "Any discoveries of vulnerabilities or other issues must be conveyed to us at the end of the working day during the execution of the tests.\n\nAny discoveries of vulnerabilities or other issues that are the direct result of AWS \(our provider\) will be forwarded to them by Vivocha.\n\nThe full report of the penetration test must be conveyed to us within 24 hours of completion of the testing." } \[/block\] **You cannot perform any kind of DoS or DDoS attack.**

**The testing results will be considered confidential information.**

Below the policy of our provider: \[block:callout\] { "type": "info", "body": "AWS's policy regarding the use of security assessment tools and services allows significant flexibility for performing security assessments of your AWS assets while protecting other AWS customers and ensuring quality-of-service across AWS.\n\nAWS understands there are a variety of public, private, commercial, and/or open-source tools and services to choose from for the purposes of performing a security assessment of your AWS assets.\n\nThe term \"security assessment\" refers to all activity engaged in for the purposes of determining the efficacy or existence of security controls amongst your AWS assets, eg. port-scanning, vulnerability scanning/checks, penetration testing, exploitation, web application scanning, as well as any injection, forgery, or fuzzing activity, either performed remotely against your AWS assets, amongst/between your AWS assets, or locally within the virtualized assets themselves.\n\nYou are NOT limited in your selection of tools or services to perform a security assessment of your AWS assets. However, you ARE prohibited from utilizing any tools or services in a manner that perform Denial-of-Service \(DoS\) attacks, or simulations of such, to or from ANY AWS asset, yours or otherwise. Prohibited activities include, but may not be limited to:\n _Protocol flooding \(eg. SYN flooding, IMCP flooding, UDP flooding\)\n_ Resource request flooding \(eg. HTTP request flooding, Login request flooding, API request flooding\)\n\nA security tool that solely performs a remote query of your AWS asset to determine a software name and version, such as \"banner grabbing,\" for the purpose of comparison to a list of versions known to be vulnerable to DoS, is NOT in violation of this policy.\n\nAdditionally, a security tool or service that solely crashes a running process on your AWS asset, temporary or otherwise, as necessary for remote or local exploitation as part of the security assessment, is NOT in violation of this policy. However, this tool may NOT engage in protocol flooding or resource request flooding, as mentioned above.\nA security tool or service that creates, determines the existence of, or demonstrates a DoS condition in ANY other manner, actual or simulated, is expressly forbidden.\n\nSome tools or services include actual DoS capabilities as described, either silently/inherently if used inappropriately or as an explicit test/check or feature of the tool or service. Any security tool or service that has such a DoS capability, must have the explicit ability to DISABLE, DISARM, or otherwise render HARMLESS, that DoS capability. Otherwise, that tool or service may NOT be employed for ANY facet of the security assessment.\n\nIt is the sole responsibility of the AWS customer to ensure the tools and services employed for performing a security assessment are properly configured and successfully operate in a manner that does not perform DoS attacks or simulations of such. It is the sole responsibility of the AWS customer to independently validate the tool or service employed does not perform DoS attacks, or simulations of such, PRIOR to security assessment of any AWS assets. This AWS customer responsibility includes ensuring contracted third-parties perform security assessments in a manner that does not violate this policy.\n\nFurthermore, you are responsible for any damages to AWS or other AWS customers that are caused by your penetration testing activities.", "title": "AWS's Policy Regarding the Use of Security Assessment Tools and Services" } \[/block\]

