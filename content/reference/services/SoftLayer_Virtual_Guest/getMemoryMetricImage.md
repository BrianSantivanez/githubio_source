---
title: "getMemoryMetricImage"
description: "Use this method when needing a memory usage image for a single guest.  It will gather the correct input parameters for t... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Virtual"
classes:
    - "SoftLayer_Virtual_Guest"
aliases:
    - "/reference/services/softlayer_virtual_guest/getMemoryMetricImage"
---
# [SoftLayer_Virtual_Guest](/reference/services/SoftLayer_Virtual_Guest)::getMemoryMetricImage


Retrieve a visual representation of the amount of memory used for the specified time frame for a computing instance. 


## Overview 
Use this method when needing a memory usage image for a single guest.  It will gather the correct input parameters for the generic graphing utility automatically based on the snapshot specified. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|snapshotRange| string| <ul type="xsd:string"> <li title="day">day</li> <li title="week">week</li> <li title="30day">30day</li> <li title="previous_calendar_month">previous_calendar_month</li> <li title="current_calendar_month">current_calendar_month</li> <li title="current_billing_cycle">current_billing_cycle</li> <li title="previous_billing_cycle">previous_billing_cycle</li> <li title="specified_day">specified_day</li> <li title="specified_range">specified_range</li> </ul>|
|dateSpecified| dateTime| Include this parameter when snapshot is 'specified_day' or 'specified_range'.  Needs to be formatted as: 'MM/DD/YYYY'|


### Required Headers
* authenticate
* SoftLayer_Virtual_GuestInitParameters


### Return Values
* <a href='/reference/datatypes/SoftLayer_Container_Bandwidth_GraphOutputs'>SoftLayer_Container_Bandwidth_GraphOutputs </a>




