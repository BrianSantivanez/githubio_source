---
title: "getBillingItemSnapshotsWithExternalAccountId"
description: "This service returns the snapshots of billing items recorded periodically given an account ID owned by the brand those billing items belong to. Retrieving billing item snapshots is more performant than retrieving billing items directly and performs less relational joins improving retrieval efficiency. 

The downside is, they are not real time, and do not share relational parity with the original billing item. "
date: "2018-02-12"
tags:
    - "method"
    - "sldn"
    - "Brand"
classes:
    - "SoftLayer_Brand"
type: "reference"
layout: "method"
mainService : "SoftLayer_Brand"
---
