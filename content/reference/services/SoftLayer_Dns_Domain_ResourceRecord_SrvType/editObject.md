---
title: "editObject"
description: "editObject edits an existing SRV resource record. The ''host'' property of the templateObject parameter is scrubbed to r... "
layout: "method"
tags:
    - "method"
    - "sldn"
    - "Dns"
classes:
    - "SoftLayer_Dns_Domain_ResourceRecord_SrvType"
aliases:
    - "/reference/services/softlayer_dns_domain_resourcerecord_srvtype/editObject"
---
# [SoftLayer_Dns_Domain_ResourceRecord_SrvType](/reference/services/SoftLayer_Dns_Domain_ResourceRecord_SrvType)::editObject


Edit a domain's SRV record.


## Overview 
editObject edits an existing SRV resource record. The ''host'' property of the templateObject parameter is scrubbed to remove all non-alpha numeric characters except for "@", "_", ".", "*", and "-". The ''data'' property of the templateObject parameter is scrubbed to remove all non-alphanumeric characters for "." and "-". Editing an SRV record updates the serial number of the domain the record is associated with. 

''editObject'' returns Boolean ''true'' on a successful edit or ''false'' if it was unable to edit the resource record. 

-----

### Parameters 
|Name | Type | Description |
| --- | --- | --- |
|templateObject| <a href='/reference/datatypes/SoftLayer_Dns_Domain_ResourceRecord_SrvType'>SoftLayer_Dns_Domain_ResourceRecord_SrvType </a>| A skeleton SoftLayer_Dns_Domain_ResourceRecord_SrvType object with only the properties defined that you wish to change. Unchanged properties are left alone.|


### Required Headers
* authenticate
* SoftLayer_Dns_Domain_ResourceRecord_SrvTypeInitParameters


### Return Values
* boolean


### Associated Methods

*  [SoftLayer_Dns_Domain_ResourceRecord::editObject](/reference/services/SoftLayer_Dns_Domain_ResourceRecord/editObject )
*  [SoftLayer_Dns_Domain_ResourceRecord::editObjects](/reference/services/SoftLayer_Dns_Domain_ResourceRecord/editObjects )
*  [SoftLayer_Dns_Domain_ResourceRecord_SrvType::editObjects](/reference/services/SoftLayer_Dns_Domain_ResourceRecord_SrvType/editObjects )




