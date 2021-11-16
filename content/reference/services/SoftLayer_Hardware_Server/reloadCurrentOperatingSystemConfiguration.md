---
title: "reloadCurrentOperatingSystemConfiguration"
description: "Reloads current operating system configuration. 

This service has a confirmation protocol for proceeding with the reloa... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware_Server"
aliases:
    - "/reference/services/softlayer_hardware_server/reloadCurrentOperatingSystemConfiguration"
---
# [SoftLayer_Hardware_Server](/reference/services/SoftLayer_Hardware_Server)::reloadCurrentOperatingSystemConfiguration


Reloads current operating system configuration.


## Overview 
Reloads current operating system configuration. 

This service has a confirmation protocol for proceeding with the reload. To proceed with the reload without confirmation, simply pass in 'FORCE' as the token parameter. To proceed with the reload with confirmation, simply call the service with no parameter. A token string will be returned by this service. The token will remain active for 10 minutes. Use this token as the parameter to confirm that a reload is to be performed for the server. 

As a precaution, we strongly  recommend backing up all data before reloading the operating system. The reload will format the primary disk and will reconfigure the server to the current specifications on record. 

The reload will take AT MINIMUM 66 minutes. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|token| string| The token returned by this service as a confirmation to proceed with the reload.|


### Required Headers
* authenticate
* SoftLayer_Hardware_ServerInitParameters


### Return Values
* string



### Error Handling

* SoftLayer_Exception_Public 

> Throws the exception 'You do not have permission to this service.' when a user does not have permission to Issue OS Reloads. 

* SoftLayer_Exception_Public 

> Throws the exception 'There is currently an outstanding transaction for this server.' when there is a current hardware update. 

* SoftLayer_Exception_Public 

> Throws the exception 'This server currently does not have an operating system.' when the server does not have an operating system in its current configuration. 

* SoftLayer_Exception_Public 

> Throws the exception 'Invalid token provided.' when an invalid token is provided. 



