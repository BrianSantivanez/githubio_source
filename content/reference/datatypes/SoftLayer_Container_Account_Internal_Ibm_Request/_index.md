---
title: "SoftLayer_Container_Account_Internal_Ibm_Request"
description: "Contains data required to both request a new IaaS account for active IBM employees and review pending requests. Fields u... "
layout: "datatype"
tags:
    - "datatype"
    - "sldn"
    - "Container"
classes:
    - "SoftLayer_Container_Account_Internal_Ibm_Request"
---

# SoftLayer_Container_Account_Internal_Ibm_Request
<div id='service-datatype'>
    <ul id='sldn-reference-tabs'>
        <li id='datatype'> <a href='/reference/datatypes/SoftLayer_Container_Account_Internal_Ibm_Request' >Datatype</a></li>
    </ul>
</div>

## Description 


Contains data required to both request a new IaaS account for active IBM employees and review pending requests. Fields used exclusively in the review process are scrubbed of user input. 


### associatedMethods

*  [SoftLayer_Account_Internal_Ibm::requestAccount](/reference/services/SoftLayer_Account_Internal_Ibm/requestAccount )
*  [SoftLayer_Account_Internal_Ibm::getAccountTypes](/reference/services/SoftLayer_Account_Internal_Ibm/getAccountTypes )





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
[accountType]: #accounttype
#### [accountType]
Purpose of the internal IBM account chosen from the list of available  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[address1]: #address1
#### [address1]
If not provided, will attempt to retrieve from BluePages  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[address2]: #address2
#### [address2]
If no address provided, will attempt to retrieve from BluePages  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[city]: #city
#### [city]
If not provided, will attempt to retrieve from BluePages  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[companyName]: #companyname
#### [companyName]
Name of the company displayed on the IaaS account  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[country]: #country
#### [country]
If not provided, will attempt to retrieve from BluePages  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[deniedFlag]: #deniedflag
#### [deniedFlag]
True if the request has been denied by either the IaaS team or the  
<span class="type-label">Type: </span>**boolean**  



</div>
<div class="prop-row">

-----
[departmentCode]: #departmentcode
#### [departmentCode]
Department within the division which will be changed during cost recovery.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[departmentCountry]: #departmentcountry
#### [departmentCountry]
Country assigned to the department for cost recovery.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[divisionCode]: #divisioncode
#### [divisionCode]
Division code used for cost recovery.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[emailAddress]: #emailaddress
#### [emailAddress]
Account owner's IBM email address. Must be a discoverable email  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[firstName]: #firstname
#### [firstName]
Applicant's first name, as provided by IBM BluePages API.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[lastName]: #lastname
#### [lastName]
Applicant's last name, as provided by IBM BluePages API.  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[managerApprovalStatus]: #managerapprovalstatus
#### [managerApprovalStatus]
APPROVED if the request has been approved by the first-line manager,  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[multiTenantFlag]: #multitenantflag
#### [multiTenantFlag]
True for accounts intended to be multi-tenant and false otherwise  
<span class="type-label">Type: </span>**boolean**  



</div>
<div class="prop-row">

-----
[officePhone]: #officephone
#### [officePhone]
Account owner's primary phone number. If no phone number is available  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[paasAccountId]: #paasaccountid
#### [paasAccountId]
Bluemix PaaS 32 digit hexadecimal account id being automatically linked  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[postalCode]: #postalcode
#### [postalCode]
If not provided, will attempt to retrieve from BluePages  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[purpose]: #purpose
#### [purpose]
Stated purpose of the new account this request would create  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[securitySubjectMatterExpertEmail]: #securitysubjectmatterexpertemail
#### [securitySubjectMatterExpertEmail]
Division's security SME's email address, if available  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[securitySubjectMatterExpertName]: #securitysubjectmatterexpertname
#### [securitySubjectMatterExpertName]
Division's security SME's name, if available  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[securitySubjectMatterExpertPhone]: #securitysubjectmatterexpertphone
#### [securitySubjectMatterExpertPhone]
Division's security SME's phone, if available  
<span class="type-label">Type: </span>**string**  



</div>
<div class="prop-row">

-----
[state]: #state
#### [state]
If required for chosen country and not provided, will attempt  
<span class="type-label">Type: </span>**string**  



</div>
</div>
<!-- LOCAL PROPERTY END -->

</div>


