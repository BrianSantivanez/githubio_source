---
title: "getBackendBandwidthUsage"
description: "Use this method to return an array of private bandwidth utilization records between a given date range. 

This method re... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware_Server"
aliases:
    - "/reference/services/softlayer_hardware_server/getBackendBandwidthUsage"
---
# [SoftLayer_Hardware_Server](/reference/services/SoftLayer_Hardware_Server)::getBackendBandwidthUsage


Retrieves public bandwidth usage records.


## Overview 
Use this method to return an array of private bandwidth utilization records between a given date range. 

This method represents the NEW version of getFrontendBandwidthUse 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|startDate| dateTime| Date from which to begin retrieving bandwidth data (inclusive).|
|endDate| dateTime| Date at which to stop retrieving bandwidth data (inclusive).|


### Required Headers
* authenticate
* SoftLayer_Hardware_ServerInitParameters


### Return Values
* <a href='/reference/datatypes/SoftLayer_Metric_Tracking_Object_Data'>SoftLayer_Metric_Tracking_Object_Data[] </a>




