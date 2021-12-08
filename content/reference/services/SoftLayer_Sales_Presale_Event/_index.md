---
title: "SoftLayer_Sales_Presale_Event"
description: "Presale events are related to datacenters or products that are not yet currently available, but will be in the near futu... "
date: "2018-02-12"
layout: "service"
tags:
    - "service"
    - "sldn"
    - "Sales"
classes:
    - "SoftLayer_Sales_Presale_Event"
---
# SoftLayer_Sales_Presale_Event
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Sales_Presale_Event' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Sales_Presale_Event' >Datatype</a></li>
    </ul>
</div>

## Description


Presale events are related to datacenters or products that are not yet currently available, but will be in the near future. For example, if a new datacenter is opening in a month, a presale event may be created that allows customers to purchase server space in advance. When a presale order is placed, the server configuration is saved, but not provisioned until the presale end date - the server will not be available during this waiting period. Also, when a presale order is placed, the customer is not charged up front, but only when the presale order is actually approved and provisioned on the presale end date. 

This server allows customer to view the currently-active presale events and their date ranges. This may allow a customer to plan early for purchasing a new product or server in a new datacenter. 



        
<div id="properties" class="content service-content">

## Methods

<div class="view-filters">
    <div class="clearfix">
        <div class="search-input-box">
            <input placeholder="Method Filter" onkeyup="titleSearch(inputId='edit-combine', divId='method-div', elementClass='method-row')" 
                type="text" id="edit-combine" value="" size="30" maxlength="128" class="form-text">
        </div>
    </div>
</div>

<div id="method-div">

<div class="method-row">

#### [getActiveFlag](/reference/services/SoftLayer_Sales_Presale_Event/getActiveFlag)
Retrieve a flag to indicate that the presale event is currently active. A presale event is active if the current time is between the start and end dates.

</div>

<div class="method-row">

#### [getAllObjects](/reference/services/SoftLayer_Sales_Presale_Event/getAllObjects)


</div>

<div class="method-row">

#### [getExpiredFlag](/reference/services/SoftLayer_Sales_Presale_Event/getExpiredFlag)
Retrieve a flag to indicate that the presale event is expired. A presale event is expired if the current time is after the end date.

</div>

<div class="method-row">

#### [getItem](/reference/services/SoftLayer_Sales_Presale_Event/getItem)
Retrieve the [SoftLayer_Product_Item]({{<ref "reference/datatypes/SoftLayer_Product_Item">}}) associated with the presale event.

</div>

<div class="method-row">

#### [getLocation](/reference/services/SoftLayer_Sales_Presale_Event/getLocation)
Retrieve the [SoftLayer_Location]({{<ref "reference/datatypes/SoftLayer_Location">}}) associated with the presale event.

</div>

<div class="method-row">

#### [getObject](/reference/services/SoftLayer_Sales_Presale_Event/getObject)
Retrieve a SoftLayer_Sales_Presale_Event record.

</div>

<div class="method-row">

#### [getOrders](/reference/services/SoftLayer_Sales_Presale_Event/getOrders)
Retrieve the orders ([SoftLayer_Billing_Order]({{<ref "reference/datatypes/SoftLayer_Billing_Order">}})) associated with this presale event that were created for the customer's account.

</div>
</div>

</div>

