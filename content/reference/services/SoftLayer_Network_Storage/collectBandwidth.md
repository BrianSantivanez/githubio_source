---
title: "collectBandwidth"
description: "{{CloudLayerOnlyMethod}} 

collectBandwidth() Retrieve the bandwidth usage for the current billing cycle."
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage"
aliases:
    - "/reference/services/softlayer_network_storage/collectBandwidth"
---
# [SoftLayer_Network_Storage](/reference/services/SoftLayer_Network_Storage)::collectBandwidth


Retrieve the bandwidth usage for the current billing cycle.


## Overview 
{{CloudLayerOnlyMethod}} 

collectBandwidth() Retrieve the bandwidth usage for the current billing cycle. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|type| string| The bandwidth type to collect usage for (upload, download)|
|startDate| dateTime| The starting date of the range of data you wish to collect.|
|endDate| dateTime| The ending date of the range of data you wish to collect.|


### Required Headers
* authenticate
* SoftLayer_Network_StorageInitParameters


### Return Values
* unsigned long



### Error Handling

* SoftLayer_Exception 

> Throw the exception "The <nasType> Storage type is not supported for bandwidth used collection.  Please contact development." 



