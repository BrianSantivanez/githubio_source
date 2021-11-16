---
title: "immediateFailoverToReplicant"
description: "Immediate Failover to a volume replicant.  During the time which the replicant is in use the local nas volume will not b... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Iscsi"
aliases:
    - "/reference/services/softlayer_network_storage_iscsi/immediateFailoverToReplicant"
---
# [SoftLayer_Network_Storage_Iscsi](/reference/services/SoftLayer_Network_Storage_Iscsi)::immediateFailoverToReplicant


Immediate Failover to a volume replicant.


## Overview 
Immediate Failover to a volume replicant.  During the time which the replicant is in use the local nas volume will not be available. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|replicantId| integer| Replicant ID to failover to|


### Required Headers
* authenticate
* SoftLayer_Network_Storage_IscsiInitParameters


### Return Values
* boolean




