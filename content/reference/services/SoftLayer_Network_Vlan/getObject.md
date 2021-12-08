---
title: "getObject"
description: "getObject retrieves the SoftLayer_Network_Vlan object whose ID number corresponds to the ID number of the init parameter... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Vlan"
aliases:
    - "/reference/services/softlayer_network_vlan/getObject"
---
# [SoftLayer_Network_Vlan](/reference/services/SoftLayer_Network_Vlan)::getObject


Retrieve a SoftLayer_Network_Vlan record.


## Overview 
getObject retrieves the SoftLayer_Network_Vlan object whose ID number corresponds to the ID number of the init parameter passed to the SoftLayer_Network_Vlan service. You can only retrieve VLANs that are associated with your SoftLayer customer account. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* SoftLayer_Network_VlanInitParameters
* authenticate


### Optional Headers
* SoftLayer_Network_VlanObjectMask
* SoftLayer_Network_VlanObjectFilter
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Network_Vlan'>SoftLayer_Network_Vlan </a>



### Error Handling

* SoftLayer_Exception_ObjectNotFound 

> Throw the error "Unable to find object with id of {id}." if the given initialization parameter has an invalid id field. 

* SoftLayer_Exception_AccessDenied 

> Throw the error "Access Denied." if the given initialization parameter id field is not the account id of the user making the API call. 



