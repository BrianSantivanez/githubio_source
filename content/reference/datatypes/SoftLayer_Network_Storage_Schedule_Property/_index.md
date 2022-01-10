---
title: "SoftLayer_Network_Storage_Schedule_Property"
description: "Schedule properties provide attributes such as start date, end date, interval, and other properties to a storage schedul... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Storage_Schedule_Property"
---

# SoftLayer_Network_Storage_Schedule_Property
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Network_Storage_Schedule_Property' >Datatype</a></li>
    </ul>
</div>

## Description 


Schedule properties provide attributes such as start date, end date, interval, and other properties to a storage schedule. 





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
The date a schedule property was created.  
<span class="type-label">Type: </span>**dateTime**  



</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
A schedule property's internal identifier.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[modifyDate]: #modifydate
#### [modifyDate]
The date a schedule property was last modified.  
<span class="type-label">Type: </span>**dateTime**  



</div>
<div class="prop-row">

-----
[typeId]: #typeid
#### [typeId]
An identifier for the type of a property.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[value]: #value
#### [value]
The value of a property.  
<span class="type-label">Type: </span>**string**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[schedule]: #schedule
#### [schedule]
The associated schedule for a property.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Storage_Schedule'>SoftLayer_Network_Storage_Schedule </a>**  



</div>
<div class="prop-row">

-----
[type]: #type
#### [type]
The type provides a standardized definition for a property.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Storage_Schedule_Property_Type'>SoftLayer_Network_Storage_Schedule_Property_Type </a>**  



</div>

## Count
</div>


