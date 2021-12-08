---
title: "createCancelServiceTicket"
description: "A cancel service request creates a sales ticket. The hardware ID parameter is required to determine which server is to b... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Ticket"
classes:
    - "SoftLayer_Ticket"
aliases:
    - "/reference/services/softlayer_ticket/createCancelServiceTicket"
---
# [SoftLayer_Ticket](/reference/services/SoftLayer_Ticket)::createCancelServiceTicket


Create a sales cancel service ticket.


## Overview 
A cancel service request creates a sales ticket. The hardware ID parameter is required to determine which server is to be cancelled. 

The reason parameter could be from the list below: 
* "No longer needed"
* "Business closing down"
* "Server / Upgrade Costs"
* "Migrating to larger server"
* "Migrating to smaller server"
* "Migrating to a different SoftLayer datacenter"
* "Network performance / latency"
* "Support response / timing"
* "Sales process / upgrades"
* "Moving to competitor"


The content parameter describes further the reason for cancelling service. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|attachmentId| integer| The internal identifier of the server or CloudLayer Computing Instance to cancel.|
|reason| string| Cancellation reason.|
|content| string| Cancellation content for ticket. A brief description explaining the cancellation reason.|
|attachmentType| string| <ul type="xsd:string"> <li title="HARDWARE">HARDWARE</li> <li title="VIRTUAL_GUEST">VIRTUAL_GUEST</li> </ul>|


### Required Headers
* authenticate


### Optional Headers
* SoftLayer_TicketObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Ticket'>SoftLayer_Ticket </a>



### Error Handling

* SoftLayer_Exception 

> Throws the exception "Attachment id must be provided." when attachment id parameter is not provided. 

* SoftLayer_Exception 

> Throws the exception "Cancellation reason must be provided." when reason parameter is not provided. 

* SoftLayer_Exception 

> Throws the exception "Cancellation content description must be provided." when content parameter is not provided. 

* SoftLayer_Exception 

> Throws the exception "You do not have permission to this service." when a portal user does not have permission to cancel service. 



