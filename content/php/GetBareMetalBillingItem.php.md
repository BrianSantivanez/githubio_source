---
title: "GetBareMetalBillingItem.php"
description: "GetBareMetalBillingItem.php"
date: "2017-11-23"
classes: 
    - "SoftLayer_Account"
    - "SoftLayer_Billing_Item"
tags:
    - "billing"
---


```php
<?php
/**
* Retrieve the billing items for the Bare Metals in the account.
*
* This script makes a single call to the getHardware() method in the
* SoftLayer_Account API service and uses a object mask to get the
* billing items and items for each Bare Metal server in the account.
*
* Important manual pages
* http://sldn.softlayer.com/reference/services/SoftLayer_Account
* http://sldn.softlayer.com/reference/datatypes/SoftLayer_Account
* http://sldn.softlayer.com/reference/datatypes/SoftLayer_Billing_Item
*
* License: http:'sldn.softlayer.com/article/License
* Author: SoftLayer Technologies, Inc. <sldn@softlayer.com>
**/
require_once ('C:/scripst/getdetails/SoftLayer/SoapClient.class.php');

# Your SoftLayer API key and username.
$apiUsername = 'set me';
$apiKey = 'set me';

# Declaring the service
$accountService = Softlayer_SoapClient::getClient('SoftLayer_Account', null, $apiUsername, $apiKey);

# Declaring the object mask to get information about the items
$objectMask = 'mask[id, hostname, domain, datacenter[longName], billingItem[item]]';
$accountService->setObjectMask($objectMask);

try {
    # Retrieving the bare metal servers billing items for the account.
    $servers = $accountService->getHardware();
    print_r($servers);
} catch (Exception $e) {
    die('Unable to retrieve the bare metal servers. ' . $e->getMessage());
}

?>

```
