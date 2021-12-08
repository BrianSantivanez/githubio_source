---
title: "denySharingAccess"
description: "This method will deny another SoftLayer customer account's previously given access to provision CloudLayer Computing Ins... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Virtual"
classes:
    - "SoftLayer_Virtual_Guest_Block_Device_Template_Group"
aliases:
    - "/reference/services/softlayer_virtual_guest_block_device_template_group/denySharingAccess"
---
# [SoftLayer_Virtual_Guest_Block_Device_Template_Group](/reference/services/SoftLayer_Virtual_Guest_Block_Device_Template_Group)::denySharingAccess


Deny another SoftLayer customer account's previously given access to provision CloudLayer Computing Instances from an image template group. Template access should only be removed from the parent template group object, not the child. 


## Overview 
This method will deny another SoftLayer customer account's previously given access to provision CloudLayer Computing Instances from an image template group. Template access should only be removed from the parent template group object, not the child. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|accountId| integer| The account id that you wish to deny sharing an image template group with.|


### Required Headers
* authenticate
* SoftLayer_Virtual_Guest_Block_Device_Template_GroupInitParameters


### Return Values
* boolean




