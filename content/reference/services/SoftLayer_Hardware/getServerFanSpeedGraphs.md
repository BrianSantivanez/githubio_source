---
title: "getServerFanSpeedGraphs"
description: "The '''getServerFanSpeedGraphs''' method retrieves the server's fan speeds and displays the speeds using tachometer grap... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware"
aliases:
    - "/reference/services/softlayer_hardware/getServerFanSpeedGraphs"
---
# [SoftLayer_Hardware](/reference/services/SoftLayer_Hardware)::getServerFanSpeedGraphs


Retrieve a server's fan speed graphs.


## Overview 
The '''getServerFanSpeedGraphs''' method retrieves the server's fan speeds and displays the speeds using tachometer graphs. data used to construct these graphs is retrieved from the server's remote management card. Each graph returned will have an associated title. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_HardwareInitParameters


### Return Values
* <a href='/reference/datatypes/SoftLayer_Container_RemoteManagement_Graphs_SensorSpeed'>SoftLayer_Container_RemoteManagement_Graphs_SensorSpeed[] </a>



### Error Handling

* SoftLayer_Exception 

> "Method has not been implemented for this object type." 



