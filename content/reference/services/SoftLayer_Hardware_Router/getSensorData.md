---
title: "getSensorData"
description: "The '''getSensorData''' method retrieves a server's hardware state via its internal sensors. Remote sensor data is trans... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Hardware"
classes:
    - "SoftLayer_Hardware_Router"
aliases:
    - "/reference/services/softlayer_hardware_router/getSensorData"
---
# [SoftLayer_Hardware_Router](/reference/services/SoftLayer_Hardware_Router)::getSensorData


Retrieve a server's hardware state via its internal sensors


## Overview 
The '''getSensorData''' method retrieves a server's hardware state via its internal sensors. Remote sensor data is transmitted to the SoftLayer API by way of the server's remote management card. Sensor data measures various information, including system temperatures, voltages and other local server settings. Sensor data is cached for 30 second; calls made to this method for the same server within 30 seconds of each other will result in the same data being returned. To ensure that the data retrieved retrieves snapshot of varied data, make calls greater than 30 seconds apart. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_Hardware_RouterInitParameters


### Return Values
* <a href='/reference/datatypes/SoftLayer_Container_RemoteManagement_SensorReading'>SoftLayer_Container_RemoteManagement_SensorReading[] </a>



### Error Handling

* SoftLayer_Exception 

> "Unable to locate the management component for this server." 



