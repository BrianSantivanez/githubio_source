---
title: "restoreDefaults"
description: "This will completely reset the firewall to factory settings. If the firewall is not a FSA 10G appliance an error will oc... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Vlan_Firewall"
aliases:
    - "/reference/services/softlayer_network_vlan_firewall/restoreDefaults"
---
# [SoftLayer_Network_Vlan_Firewall](/reference/services/SoftLayer_Network_Vlan_Firewall)::restoreDefaults


Reset the FSA 10G firewall to factory settings.


## Overview 
This will completely reset the firewall to factory settings. If the firewall is not a FSA 10G appliance an error will occur. Note, this process is performed asynchronously. During the process all traffic will not be routed through the firewall. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |


### Required Headers
* authenticate
* SoftLayer_Network_Vlan_FirewallInitParameters


### Optional Headers
* SoftLayer_Network_Vlan_FirewallObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Provisioning_Version1_Transaction'>SoftLayer_Provisioning_Version1_Transaction </a>




