---
title: "addAttachedVirtualGuest"
description: "Attach the given CloudLayer Computing Instance to a SoftLayer ticket. An attachment provides an easy way for SoftLayer's... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Ticket"
classes:
    - "SoftLayer_Ticket"
aliases:
    - "/reference/services/softlayer_ticket/addAttachedVirtualGuest"
---
# [SoftLayer_Ticket](/reference/services/SoftLayer_Ticket)::addAttachedVirtualGuest


Attach a CloudLayer Computing Instance to a ticket.


## Overview 
Attach the given CloudLayer Computing Instance to a SoftLayer ticket. An attachment provides an easy way for SoftLayer's employees to quickly look up your records in the case of specific issues. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|guestId| integer| The internal identifier of the virtual guest record to attach.|
|callCommit| boolean| call commit or not|


### Required Headers
* authenticate
* SoftLayer_TicketInitParameters


### Optional Headers
* SoftLayer_TicketObjectMask
* SoftLayer_ObjectMask

### Return Values
* <a href='/reference/datatypes/SoftLayer_Ticket_Attachment_Virtual_Guest'>SoftLayer_Ticket_Attachment_Virtual_Guest </a>


### Associated Methods

*  [SoftLayer_Ticket::removeAttachedVirtualGuest](/reference/services/SoftLayer_Ticket/removeAttachedVirtualGuest )



### Error Handling

* SoftLayer_Exception 

> Throw the exception "Unable to attach a null virtual guest to this ticket." if no virtual guest identifier is provided. 

* SoftLayer_Exception 

> Throw the exception "This virtual guest is already attached to this ticket." if the given virtual guest is already attached to this ticket. 

* SoftLayer_Exception 

> Throw the exception "You may not attach this virtual guest to this ticket." if the user making the API call does not have permission to use the given virtual guest. 

* SoftLayer_Exception 

> Throw the exception "Unable to attach virtual guest to this ticket." if the API is unable to attach the given virtual guest to this ticket. 



