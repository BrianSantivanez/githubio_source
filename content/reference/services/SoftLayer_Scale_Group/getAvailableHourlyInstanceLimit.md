---
title: "getAvailableHourlyInstanceLimit"
description: "This returns the number of hourly instances an account can add from this point. It is essentially the same as [SoftLayer... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Scale"
classes:
    - "SoftLayer_Scale_Group"
aliases:
    - "/reference/services/softlayer_scale_group/getAvailableHourlyInstanceLimit"
---
# [SoftLayer_Scale_Group](/reference/services/SoftLayer_Scale_Group)::getAvailableHourlyInstanceLimit


This returns the number of hourly instances an account can add from this point. 


## Overview 
This returns the number of hourly instances an account can add from this point. It is essentially the same as [SoftLayer_Account::hourlyInstanceLimit]({{<ref "reference/services/SoftLayer_Account/hourlyInstanceLimit">}}) minus existing hourly instances and ones spoken for as part of a scaling group (as determined by the group's maximum). This number can be used to help determine a maximum member count for a new group to ensure it won't go over the account limit. This can return a negative value if the current hourly instance count combined with the unused-but-possible count (based on other scale group maximums) is over the limit. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate


### Return Values
* integer




