---
title: "getStatus"
description: "Returns an array of SoftLayer_Container_Network_LoadBalancer_StatusEntry objects.  A SoftLayer_Container_Network_LoadBalancer_StatusEntry object has two variables, 'Label' and 'Value' 

Calling this function executes a command on the physical load balancer itself, and therefore should be called infrequently.  For a general idea of the load balancer service, use the 'peakConnections' variable on the Type 

Possible values for 'Label' are: 


* IP Address
* Port
* Server Status
* Load Status
* Current Connections
* Total Hits


Not all labels are guaranteed to be returned. "
date: "2018-02-12"
tags:
    - "method"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_LoadBalancer_Service"
type: "reference"
layout: "method"
mainService : "SoftLayer_Network_LoadBalancer_Service"
---
