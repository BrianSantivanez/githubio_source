---
title: "deleteObject"
description: "Delete a domain's resource record. '''This cannot be undone.''' Be wary of running this method. If you remove a resource record in error you will need to re-create it by creating a new SoftLayer_Dns_Domain_ResourceRecord object. The serial number of the domain associated with this resource record is updated upon deletion. You may not delete SOA, NS, or PTR resource records. 

''deleteObject'' returns Boolean ''true'' on successful deletion or ''false'' if it was unable to remove a resource record. "
date: "2018-02-12"
tags:
    - "method"
    - "sldn"
    - "Dns"
classes:
    - "SoftLayer_Dns_Domain_ResourceRecord"
type: "reference"
layout: "method"
mainService : "SoftLayer_Dns_Domain_ResourceRecord"
---
