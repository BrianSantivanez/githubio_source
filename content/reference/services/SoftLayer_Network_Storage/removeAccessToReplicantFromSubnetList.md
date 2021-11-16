---
title: "removeAccessToReplicantFromSubnetList"
description: "This method is used to modify the access control list for this Storage volume's replica.  The SoftLayer_Network_Subnet o... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage"
aliases:
    - "/reference/services/softlayer_network_storage/removeAccessToReplicantFromSubnetList"
---
# [SoftLayer_Network_Storage](/reference/services/SoftLayer_Network_Storage)::removeAccessToReplicantFromSubnetList


Remove access to this volume's replica from multiple SoftLayer_Network_Subnet objects.


## Overview 
This method is used to modify the access control list for this Storage volume's replica.  The SoftLayer_Network_Subnet objects which have been allowed access to this storage volume's replica will be listed in the allowedReplicationSubnets property of this storage volume. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|subnetObjectTemplates| <a href='/reference/datatypes/SoftLayer_Network_Subnet'>SoftLayer_Network_Subnet[] </a>| |


### Required Headers
* authenticate
* SoftLayer_Network_StorageInitParameters


### Return Values
* boolean




