---
title: "massHyperThreadingUpdate"
description: "You can launch hyper-threading update by selecting from your server list. It will bring your server offline for approxim... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware_Server"
aliases:
    - "/reference/services/softlayer_hardware_server/massHyperThreadingUpdate"
---
# [SoftLayer_Hardware_Server](/reference/services/SoftLayer_Hardware_Server)::massHyperThreadingUpdate


Runs firmware reflashes on the servers components.


## Overview 
You can launch hyper-threading update by selecting from your server list. It will bring your server offline for approximately 60 minutes while the updates are in progress. 

In the event of a hardware failure during this update our datacenter engineers will be notified of the problem automatically. They will then replace any failed components to bring your server back online. They will be in contact with you to ensure that impact on your server is minimal. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|hardwareIds| array of integers| List of hardware ids to update hyper-threading.|
|disableHyperthreading| boolean| Flag to determine whether to disable or enable hyper-threading.|


### Required Headers
* authenticate


### Return Values
* <a href='/reference/datatypes/SoftLayer_Container_Hardware_Server_Request'>SoftLayer_Container_Hardware_Server_Request[] </a>



### Error Handling

* SoftLayer_Exception_Public 

> Throws the exception 'You do not have permission to this service.' when a user does not have permission to Issue OS Reloads. 



