---
title: "reassignServers"
description: "This method will reassign a collection of SoftLayer hardware to a bandwidth allotment Bandwidth Pool."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Bandwidth_Version1_Allotment"
aliases:
    - "/reference/services/softlayer_network_bandwidth_version1_allotment/reassignServers"
---
# [SoftLayer_Network_Bandwidth_Version1_Allotment](/reference/services/SoftLayer_Network_Bandwidth_Version1_Allotment)::reassignServers


reassign a collection of servers to a different allotment.


## Overview 
This method will reassign a collection of SoftLayer hardware to a bandwidth allotment Bandwidth Pool. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|templateObjects| <a href='/reference/datatypes/SoftLayer_Hardware'>SoftLayer_Hardware[] </a>| A collection of servers to be reassigned to a new allotment|
|newAllotmentId| integer| The id of the allotment that the objects will be reassigned to|


### Required Headers
* authenticate


### Return Values
* boolean




