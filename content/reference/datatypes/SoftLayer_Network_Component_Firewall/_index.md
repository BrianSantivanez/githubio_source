---
title: "SoftLayer_Network_Component_Firewall"
description: "The SoftLayer_Network_Component_Firewall data type contains general information relating to a single SoftLayer network c... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Network"
classes:
    - "SoftLayer_Network_Component_Firewall"
---

# SoftLayer_Network_Component_Firewall
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
    <li id='service'> <a href='/reference/services/SoftLayer_Network_Component_Firewall' >Service</a></li>    <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Network_Component_Firewall' >Datatype</a></li>
    </ul>
</div>

## Description 


The SoftLayer_Network_Component_Firewall data type contains general information relating to a single SoftLayer network component firewall. This is the object which ties the running rules to a specific downstream server. Use the [[SoftLayer Network Firewall Template]] service to pull SoftLayer recommended rule set templates. Use the [[SoftLayer Network Firewall Update Request]] service to submit a firewall update request. 

### External Links


* [Firewall at Wikipedia](http://en.wikipedia.org/wiki/Firewall_(networking))




### seeAlso

* [SoftLayer_Network_Firewall_Template](/reference/services/SoftLayer_Network_Firewall_Template )


* [SoftLayer_Network_Firewall_Update_Request](/reference/services/SoftLayer_Network_Firewall_Update_Request )




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
[guestNetworkComponentId]: #guestnetworkcomponentid
#### [guestNetworkComponentId]
Unique ID for the network component of the switch interface that this network component firewall is attached to.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[id]: #id
#### [id]
Unique ID for the network component firewall.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[networkComponentId]: #networkcomponentid
#### [networkComponentId]
Unique ID for the network component of the switch interface that this network component firewall is attached to.  
<span class="type-label">Type: </span>**integer**  



</div>
<div class="prop-row">

-----
[status]: #status
#### [status]
Current status of the network component firewall. Status "no_edit" means this host is not protected by a hardware firewall. Status "allow_edit" means this host is protected by a hardware firewall and processing firewall rules. Status "bypass" means this host is provisioned behind a hardware firewall, but bypassing the firewall rules.   
<span class="type-label">Type: </span>**string**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

<div id="relationalProperties"  class="prop-content" >

## Relational
<div class="prop-row">

-----
[applyServerRuleSubnets]: #applyserverrulesubnets
#### [applyServerRuleSubnets]
The additional subnets linked to this network component firewall, that inherit rules from the host that the context slot is attached to.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Subnet'>SoftLayer_Network_Subnet[] </a>**  



</div>
<div class="prop-row">

-----
[billingItem]: #billingitem
#### [billingItem]
The billing item for a Hardware Firewall (Dedicated).  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Billing_Item'>SoftLayer_Billing_Item </a>**  



</div>
<div class="prop-row">

-----
[guestNetworkComponent]: #guestnetworkcomponent
#### [guestNetworkComponent]
The network component of the guest virtual server that this network component firewall belongs to.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Virtual_Guest_Network_Component'>SoftLayer_Virtual_Guest_Network_Component </a>**  



</div>
<div class="prop-row">

-----
[networkComponent]: #networkcomponent
#### [networkComponent]
The network component of the switch interface that this network component firewall belongs to.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Component'>SoftLayer_Network_Component </a>**  



</div>
<div class="prop-row">

-----
[networkFirewallUpdateRequest]: #networkfirewallupdaterequest
#### [networkFirewallUpdateRequest]
The update requests made for this firewall.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Firewall_Update_Request'>SoftLayer_Network_Firewall_Update_Request[] </a>**  



</div>
<div class="prop-row">

-----
[rules]: #rules
#### [rules]
The currently running rule set of this network component firewall.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Component_Firewall_Rule'>SoftLayer_Network_Component_Firewall_Rule[] </a>**  



</div>
<div class="prop-row">

-----
[subnets]: #subnets
#### [subnets]
The additional subnets linked to this network component firewall.  
<span class="type-label">Type: </span>**<a href='/reference/datatypes/SoftLayer_Network_Subnet'>SoftLayer_Network_Subnet[] </a>**  



</div>

## Count
<div class="prop-row">

-----
[applyServerRuleSubnetCount]: #applyserverrulesubnetcount
#### [applyServerRuleSubnetCount]
A count of the additional subnets linked to this network component firewall, that inherit rules from the host that the context slot is attached to.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[networkFirewallUpdateRequestCount]: #networkfirewallupdaterequestcount
#### [networkFirewallUpdateRequestCount]
A count of the update requests made for this firewall.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[ruleCount]: #rulecount
#### [ruleCount]
A count of the currently running rule set of this network component firewall.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
<div class="prop-row">

-----
[subnetCount]: #subnetcount
#### [subnetCount]
A count of the additional subnets linked to this network component firewall.   
<span class="type-label">Type: </span>**unsigned long**  



</div>
</div>


