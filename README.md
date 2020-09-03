# PyCon TW 2020 Talk: Network Automation with Python Supplements

This repository provides demonstration supplement to the PyCon TW 2020 talk: Network Automation with Python. 
https://tw.pycon.org/2020/en-us/conference/talk/1153041030333858139/

The examples are done via the free sandbox environment provided by https://developer.cisco.com/site/sandbox/, thank you Cisco DevNet! Please feel free to sign up and follow along with the examples provided. 

![Cisco DevNet Screenshot](/images/Cisco_DevNet_Screenshot.png)

## NX-OS Device API Example

The NX-oS Device API Example is done with the Multi-IOS Cisco Test Network Sandbox, https://devnetsandbox.cisco.com/RM/Diagram/Index/037f3542-f1bb-4b70-a0e7-d87f0fa8b75f, with 8 node datacenter setup. This lab is free but requires reservation on the DevNet lab page. 

![Multi-IOS-Test-Network](/images/Multi-IOS-Test-Network.png)

```
(venv) [developer@devbox user]$ssh cisco@172.16.30.58
Warning: Permanently added '172.16.30.58' (RSA) to the list of known hosts.
User Access Verification
Password:

Cisco NX-OS Software
Copyright (c) 2002-2018, Cisco Systems, Inc. All rights reserved.
Nexus 9000v software ("Nexus 9000v Software") and related documentation,

dist4# confi t
Enter configuration commands, one per line. End with CNTL/Z.
dist4(config)# feature nxapi
dist4(config)# nxapi http port 80
dist4(config)# end
dist4# copy run start
[########################################] 100%
Copy complete, now saving to disk (please wait)...
Copy complete.
dist4#
```

## Ansible Example

The Ansible example is based on the same remote lab. 

## Meraki Controller Example

The Meraki controller example is based on the always-on Meraki lab, but it can also be done with the Meraki reservation labs. 

![Meraki_Lab](/images/Meraki_Lab.png)

[Meraki Dashboard API Reference](https://documentation.meraki.com/zGeneral_Administration/Other_Topics/The_Cisco_Meraki_Dashboard_API)

Steps: 

1. Select Organization and network. 
2. Enable API access. 
3. Generate API key. 
4. Use the API key to retrieve organization ID. 
5. Use API endpoint to retrieve information, for example, a list of inventories. 

- Click image below for YouTube video

[![Meraki Video Demo](/images/Meraki_Video.png)](https://youtu.be/_GLoWyHFTnE)



