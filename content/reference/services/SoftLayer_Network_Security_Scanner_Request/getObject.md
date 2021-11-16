---
title: "getObject"
description: "getObject retrieves the SoftLayer_Network_Security_Scanner_Request object whose ID number corresponds to the ID number o... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Security_Scanner_Request"
aliases:
    - "/reference/services/softlayer_network_security_scanner_request/getObject"
---
# [SoftLayer_Network_Security_Scanner_Request](/reference/services/SoftLayer_Network_Security_Scanner_Request)::getObject


Retrieve a SoftLayer_Network_Security_Scanner_Request record.


## Overview 
getObject retrieves the SoftLayer_Network_Security_Scanner_Request object whose ID number corresponds to the ID number of the init parameter passed to the SoftLayer_Network_Security_Scanner_Request service. You can only retrieve requests and reports that are assigned to your SoftLayer account. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* SoftLayer_Network_Security_Scanner_RequestInitParameters
* authenticate


### Optional Headers
* SoftLayer_Network_Security_Scanner_RequestObjectMask
* SoftLayer_Network_Security_Scanner_RequestObjectFilter
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Security_Scanner_Request'>SoftLayer_Network_Security_Scanner_Request </a>



### Error Handling

* SoftLayer_Exception_ObjectNotFound 

> Throws the error "Unable to find object with id of {id}." when the object for the supplied hardwareId is not found. 

* SoftLayer_Exception_Network_Security_Scanner_Request_OpenRequestFound 

> Throws the error "Only one vulnerability scan may be started at a time." when a trying to create a new request before a previous one for the selected hardware item is finished. 

* SoftLayer_Exception_Network_Security_Scanner_Request_ReportNotFound 

> Throws the error "The selected vulnerability report could not be found." when the report file could not be located. 



