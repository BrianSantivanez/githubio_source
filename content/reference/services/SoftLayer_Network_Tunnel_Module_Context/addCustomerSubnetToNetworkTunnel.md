---
title: "addCustomerSubnetToNetworkTunnel"
description: "Associates a remote subnet to the network tunnel.  When a remote subnet is associated, a network tunnel will allow the c... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Tunnel_Module_Context"
aliases:
    - "/reference/services/softlayer_network_tunnel_module_context/addCustomerSubnetToNetworkTunnel"
---
# [SoftLayer_Network_Tunnel_Module_Context](/reference/services/SoftLayer_Network_Tunnel_Module_Context)::addCustomerSubnetToNetworkTunnel


Associate a remote subnet to a network tunnel


## Overview 
Associates a remote subnet to the network tunnel.  When a remote subnet is associated, a network tunnel will allow the customer (remote) network to communicate with the private and service subnets on the SoftLayer network which are on the other end of this network tunnel. 

NOTE:  A network tunnel's configurations must be applied to the network device in order for the association described above to take effect. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|subnetId| integer| The internal identifier of the customer (remote) subnet to add.|


### Required Headers
* authenticate
* SoftLayer_Network_Tunnel_Module_ContextInitParameters


### Return Values
* boolean


### Associated Methods

*  [SoftLayer_Network_Tunnel_Module_Context::addPrivateSubnetToNetworkTunnel](/reference/services/SoftLayer_Network_Tunnel_Module_Context/addPrivateSubnetToNetworkTunnel )
*  [SoftLayer_Network_Tunnel_Module_Context::addServiceSubnetToNetworkTunnel](/reference/services/SoftLayer_Network_Tunnel_Module_Context/addServiceSubnetToNetworkTunnel )
*  [SoftLayer_Network_Tunnel_Module_Context::removePrivateSubnetFromNetworkTunnel](/reference/services/SoftLayer_Network_Tunnel_Module_Context/removePrivateSubnetFromNetworkTunnel )
*  [SoftLayer_Network_Tunnel_Module_Context::removeCustomerSubnetFromNetworkTunnel](/reference/services/SoftLayer_Network_Tunnel_Module_Context/removeCustomerSubnetFromNetworkTunnel )
*  [SoftLayer_Network_Tunnel_Module_Context::removeServiceSubnetFromNetworkTunnel](/reference/services/SoftLayer_Network_Tunnel_Module_Context/removeServiceSubnetFromNetworkTunnel )
*  [SoftLayer_Network_Tunnel_Module_Context::applyConfigurationsToDevice](/reference/services/SoftLayer_Network_Tunnel_Module_Context/applyConfigurationsToDevice )
*  [SoftLayer_Network_Customer_Subnet::createObject](/reference/services/SoftLayer_Network_Customer_Subnet/createObject )




