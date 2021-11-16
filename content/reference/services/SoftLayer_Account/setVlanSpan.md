---
title: "setVlanSpan"
description: "Set the flag that enables or disables automatic private network VLAN spanning for a SoftLayer customer account. Enabling... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Account"
classes:
    - "SoftLayer_Account"
aliases:
    - "/reference/services/softlayer_account/setVlanSpan"
---
# [SoftLayer_Account](/reference/services/SoftLayer_Account)::setVlanSpan


Set the flag that enables or disables automatic private network VLAN spanning for a SoftLayer customer account.


## Overview 
Set the flag that enables or disables automatic private network VLAN spanning for a SoftLayer customer account. Enabling VLAN spanning allows an account's servers to talk on the same broadcast domain even if they reside within different private vlans. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|enabled| boolean| Whether or not to enable private VLAN spanning on an account.|


### Required Headers
* authenticate


### Return Values
* boolean



### Error Handling

* SoftLayer_Exception_User_Permission 

> <<< EOT 

* SoftLayer_Exception_NotReady 

> <<< EOT 



