---
title: "SoftLayer_Network_Subnet_Registration"
description: "The subnet registration data type contains general information relating to a single subnet registration instance. These... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Subnet_Registration"
---

# SoftLayer_Network_Subnet_Registration
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Network_Subnet_Registration' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Network_Subnet_Registration' >Datatype</a></li>
    </ul>
</div>

## Description 


The subnet registration data type contains general information relating to a single subnet registration instance. These registration instances can be updated to reflect changes, and will record the changes in the [SoftLayer_Network_Subnet_Registration_Event]({{<ref "reference/datatypes/SoftLayer_Network_Subnet_Registration_Event">}}). 





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
The registration object's associated [SoftLayer_Account]({{<ref "reference/datatypes/SoftLayer_Account">}}) id   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[cidr]: #cidr
#### [cidr]
The CIDR prefix for the registered subnet   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[createDate]: #createdate
#### [createDate]
  
<span class="type-label">Type: </span>**dateTime**  



</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
Unique ID of the registration object   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[modifyDate]: #modifydate
#### [modifyDate]
  
<span class="type-label">Type: </span>**dateTime**  



</div>
<div class="prop-row">

-----
[networkHandle]: #networkhandle
#### [networkHandle]
The RIR-specific handle or name of the registered subnet. This field is read-only.   
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[networkIdentifier]: #networkidentifier
#### [networkIdentifier]
The base IP address of the registered subnet   
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[regionalInternetRegistryHandleId]: #regionalinternetregistryhandleid
#### [regionalInternetRegistryHandleId]
The registration object's associated [SoftLayer_Account_Rwhois_Handle]({{<ref "reference/datatypes/SoftLayer_Account_Rwhois_Handle">}}) id   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[regionalInternetRegistryId]: #regionalinternetregistryid
#### [regionalInternetRegistryId]
The registration object's associated [SoftLayer_Network_Regional_Internet_Registry]({{<ref "reference/datatypes/SoftLayer_Network_Regional_Internet_Registry">}}) id   
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[statusId]: #statusid
#### [statusId]
The registration object's associated [SoftLayer_Network_Subnet_Registration_Status]({{<ref "reference/datatypes/SoftLayer_Network_Subnet_Registration_Status">}}) id   
<span class="type-label">Type: </span>**integer**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[account]: #account
#### [account]
The account that this registration belongs to.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Account'>SoftLayer_Account </a>**  



</div>
<div class="prop-row">

-----
[detailReferences]: #detailreferences
#### [detailReferences]
The cross-reference records that tie the [SoftLayer_Account_Regional_Registry_Detail]({{<ref "reference/datatypes/SoftLayer_Account_Regional_Registry_Detail">}}) objects to the registration object.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Subnet_Registration_Details'>SoftLayer_Network_Subnet_Registration_Details[] </a>**  



</div>
<div class="prop-row">

-----
[events]: #events
#### [events]
The related registration events.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Subnet_Registration_Event'>SoftLayer_Network_Subnet_Registration_Event[] </a>**  



</div>
<div class="prop-row">

-----
[networkDetail]: #networkdetail
#### [networkDetail]
The "network" detail object.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Account_Regional_Registry_Detail'>SoftLayer_Account_Regional_Registry_Detail </a>**  



</div>
<div class="prop-row">

-----
[personDetail]: #persondetail
#### [personDetail]
The "person" detail object.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Account_Regional_Registry_Detail'>SoftLayer_Account_Regional_Registry_Detail </a>**  



</div>
<div class="prop-row">

-----
[regionalInternetRegistry]: #regionalinternetregistry
#### [regionalInternetRegistry]
The related Regional Internet Registry.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Regional_Internet_Registry'>SoftLayer_Network_Regional_Internet_Registry </a>**  



</div>
<div class="prop-row">

-----
[regionalInternetRegistryHandle]: #regionalinternetregistryhandle
#### [regionalInternetRegistryHandle]
The RIR handle that this registration object belongs to. This field may not be populated until the registration is complete.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Account_Rwhois_Handle'>SoftLayer_Account_Rwhois_Handle </a>**  



</div>
<div class="prop-row">

-----
[status]: #status
#### [status]
The status of this registration.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Subnet_Registration_Status'>SoftLayer_Network_Subnet_Registration_Status </a>**  



</div>
<div class="prop-row">

-----
[subnet]: #subnet
#### [subnet]
The subnet that this registration pertains to.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Subnet'>SoftLayer_Network_Subnet </a>**  



</div>

## Count
<div class="prop-row">

-----
[detailReferenceCount]: #detailreferencecount
#### [detailReferenceCount]
A count of the cross-reference records that tie the [SoftLayer_Account_Regional_Registry_Detail]({{<ref "reference/datatypes/SoftLayer_Account_Regional_Registry_Detail">}}) objects to the registration object.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[eventCount]: #eventcount
#### [eventCount]
A count of the related registration events.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
</div>


