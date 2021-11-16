---
title: "SoftLayer_Ticket_Update_Employee"
description: "The SoftLayer_Ticket_Update_Employee data type models an update to a ticket made by a SoftLayer employee."
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Ticket"
classes:
    - "SoftLayer_Ticket_Update_Employee"
---

# SoftLayer_Ticket_Update_Employee
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Ticket_Update_Employee' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Ticket_Update_Employee' >Datatype</a></li>
    </ul>
</div>

## Description 


The SoftLayer_Ticket_Update_Employee data type models an update to a ticket made by a SoftLayer employee. 



### seeAlso

* [SoftLayer_Ticket](/reference/services/SoftLayer_Ticket )


* [SoftLayer_Ticket_Update](/reference/datatypes/SoftLayer_Ticket_Update )


* [SoftLayer_Ticket_Update_Customer](/reference/datatypes/SoftLayer_Ticket_Update_Customer )




<!-- Filer BEGIN -->
<div class="view-filters">
        <div class="clearfix">
            <div class="search-input-box">
                <input placeholder="Datatype Filter" onkeyup="titleSearch(inputId='prop-input', divId='properties', elementClass='prop-row')" 
                    type="text" id="prop-input" value="" size="30" maxlength="128" class="form-text">
            </div>
        </div>
</div>
<!-- Filer END -->

<div id="properties" class="content">
<div id="localProperties" class="prop-content" >

## Local
<div class="prop-row">

-----
[createDate]: #createdate
#### [createDate]
The data a ticket update was created.  
<span class="type-label">Type: </span>**dateTime**  



</div>
<div class="prop-row">

-----
[editorId]: #editorid
#### [editorId]
The internal identifier of the SoftLayer portal or API user who created a ticket update. This is only used if a ticket update's ''editorType'' property is "USER".   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[editorType]: #editortype
#### [editorType]
The type user who created a ticket update. This is either "USER" for an update created by a SoftLayer portal or API user, "EMPLOYEE" for an update created by a SoftLayer employee, or "AUTO" if a ticket update was generated automatically by SoftLayer's backend systems.   
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[entry]: #entry
#### [entry]
The contents of a ticket update.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
A ticket update's internal identifier.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[responseRating]: #responserating
#### [responseRating]
A ticket update's response rating. Ticket updates posted by SoftLayer employees have the option of earning a rating from SoftLayer's customers. Ratings are based on a 1 - 5 scale, with one being a poor rating while 5 is a very high rating. This is only used if a ticket update's ''editorType'' property is "EMPLOYEE".   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[ticketId]: #ticketid
#### [ticketId]
The internal identifier of the ticket that a ticket update belongs to.  
<span class="type-label">Type: </span>**integer**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[changeOwnerActivity]: #changeowneractivity
#### [changeOwnerActivity]
  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[chat]: #chat
#### [chat]
The chat between the Customer and Agent  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Ticket_Chat_Liveperson'>SoftLayer_Ticket_Chat_Liveperson </a>**  



</div>
<div class="prop-row">

-----
[editor]: #editor
#### [editor]
A representation of the SoftLayer employee who created a ticket update.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_User_Employee'>SoftLayer_User_Employee </a>**  



</div>
<div class="prop-row">

-----
[fileAttachment]: #fileattachment
#### [fileAttachment]
The files attached to a ticket update.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Ticket_Attachment_File'>SoftLayer_Ticket_Attachment_File[] </a>**  



</div>
<div class="prop-row">

-----
[ticket]: #ticket
#### [ticket]
The ticket that a ticket update belongs to.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Ticket'>SoftLayer_Ticket </a>**  



</div>
<div class="prop-row">

-----
[type]: #type
#### [type]
The Type of update to this ticket  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Ticket_Update_Type'>SoftLayer_Ticket_Update_Type </a>**  



</div>

## Count
<div class="prop-row">

-----
[fileAttachmentCount]: #fileattachmentcount
#### [fileAttachmentCount]
A count of the files attached to a ticket update.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
</div>


