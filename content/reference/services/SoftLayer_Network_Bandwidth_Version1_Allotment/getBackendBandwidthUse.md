---
title: "getBackendBandwidthUse"
description: "This method recurses through all servers on a Bandwidth Pool between the given start and end dates to retrieve public ba... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Bandwidth_Version1_Allotment"
aliases:
    - "/reference/services/softlayer_network_bandwidth_version1_allotment/getBackendBandwidthUse"
---
# [SoftLayer_Network_Bandwidth_Version1_Allotment](/reference/services/SoftLayer_Network_Bandwidth_Version1_Allotment)::getBackendBandwidthUse


return a collection of private usage objects that contain hourly incoming and outgoing network traffic amounts for a customer date period. 


## Overview 
This method recurses through all servers on a Bandwidth Pool between the given start and end dates to retrieve public bandwidth data. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|startDate| dateTime| Start date formatted as: 'MM/DD/YY'.|
|endDate| dateTime| End date formatted as: 'MM/DD/YY'.|


### Required Headers
* authenticate
* SoftLayer_Network_Bandwidth_Version1_AllotmentInitParameters


### Optional Headers
* SoftLayer_Network_Bandwidth_Version1_AllotmentObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Bandwidth_Version1_Usage_Detail'>SoftLayer_Network_Bandwidth_Version1_Usage_Detail[] </a>




