---
title: "SoftLayer_Virtual_ReservedCapacityGroup"
description: "This data type presents the structure for a virtual reserved capacity group."
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Virtual"
classes:
    - "SoftLayer_Virtual_ReservedCapacityGroup"
---

# SoftLayer_Virtual_ReservedCapacityGroup
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Virtual_ReservedCapacityGroup' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Virtual_ReservedCapacityGroup' >Datatype</a></li>
    </ul>
</div>

## Description 


This data type presents the structure for a virtual reserved capacity group. 





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
[accountId]: #accountid
#### [accountId]
The unique ID of the account that created the reserved capacity group.   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[backendRouterId]: #backendrouterid
#### [backendRouterId]
The reserved capacity group's backend router's associated unique ID.   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[createDate]: #createdate
#### [createDate]
The date that the reserved capacity group was created.   
<span class="type-label">Type: </span>**dateTime**  



</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
The reserved capacity group's associated unique ID.   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[modifyDate]: #modifydate
#### [modifyDate]
The date that the reserved capacity group was last modified.   
<span class="type-label">Type: </span>**dateTime**  



</div>
<div class="prop-row">

-----
[name]: #name
#### [name]
The reserved capacity group's name.   
<span class="type-label">Type: </span>**string**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[account]: #account
#### [account]
The account that the reserved capacity group is implemented on.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Account'>SoftLayer_Account </a>**  



</div>
<div class="prop-row">

-----
[availableInstances]: #availableinstances
#### [availableInstances]
The instances available for guest provisions on this reserved capacity group.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Virtual_ReservedCapacityGroup_Instance'>SoftLayer_Virtual_ReservedCapacityGroup_Instance[] </a>**  



</div>
<div class="prop-row">

-----
[backendRouter]: #backendrouter
#### [backendRouter]
The router the reserved capacity group is implemented on.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Hardware_Router_Backend'>SoftLayer_Hardware_Router_Backend </a>**  



</div>
<div class="prop-row">

-----
[instances]: #instances
#### [instances]
The guest instances that are members of this reserved capacity group.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Virtual_ReservedCapacityGroup_Instance'>SoftLayer_Virtual_ReservedCapacityGroup_Instance[] </a>**  



</div>
<div class="prop-row">

-----
[instancesCount]: #instancescount
#### [instancesCount]
The number of instances that are members of this reserved capacity group.  
<span class="type-label">Type: </span>**unsigned integer**  



</div>
<div class="prop-row">

-----
[occupiedInstances]: #occupiedinstances
#### [occupiedInstances]
The instances already occupied by a guest on this reserved capacity group.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Virtual_ReservedCapacityGroup_Instance'>SoftLayer_Virtual_ReservedCapacityGroup_Instance[] </a>**  



</div>

## Count
<div class="prop-row">

-----
[availableInstanceCount]: #availableinstancecount
#### [availableInstanceCount]
A count of the instances available for guest provisions on this reserved capacity group.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[instanceCount]: #instancecount
#### [instanceCount]
A count of the guest instances that are members of this reserved capacity group.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[occupiedInstanceCount]: #occupiedinstancecount
#### [occupiedInstanceCount]
A count of the instances already occupied by a guest on this reserved capacity group.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
</div>


