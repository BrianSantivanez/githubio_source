---
title: "CreatePortablePublicSubnet.php"
description: "CreatePortablePublicSubnet.php"
date: "2017-11-23"
classes: 
    - "SoftLayer_SoapClient"
    - "SoftLayer_Container_Product_Order_Network_Subnet"
    - "SoftLayer_Network_Subnet"
    - "SoftLayer_Product_Order"
tags:
    - "subnet"
---


```php
<?php
/**
 * Create Static Public Subnet.
 *
 * Important manual pages:
 * http://sldn.softlayer.com/reference/services/SoftLayer_Product_Order/placeOrder/
 * http://sldn.softlayer.com/reference/services/SoftLayer_Product_Order/verifyOrder/
 * http://sldn.softlayer.com/reference/datatypes/SoftLayer_Container_Product_Order_Network_Subnet
 *
 * @license <http://sldn.softlayer.com/wiki/index.php/License>
 * @author SoftLayer Technologies, Inc. <sldn@softlayer.com>
 */

require_once(dirname(__FILE__) . '/SoftLayer/SoapClient.class.php');

/**
 * Set your SoftLayer API username and key.
 */
$apiUsername = 'set me';
$apiKey = 'set me';

/**
 * Set the service to use
 */
$serviceName ='SoftLayer_Product_Order';

$priceId =  13980;

/**
 * The id of the VLAN that you want to route a portable subnet to.
 *
 * @var int
 */
$endPointVlanId = 331044;

/**
 * The number of subnets you want to order
 *
 * @var int;
 */
$quantity = 1;

// Build a SoftLayer_Container_Product_Order_Network_Subnet object containing
// the order you want to place. Subnets don't have a package, so set packageId
// to 0. Since this order is for one item with no sub-options you only have to
// set a single price id in this order.
$orderTemplate = new stdClass();
$orderTemplate->packageId           = 0;
$orderTemplate->prices              = array();
$orderTemplate->prices[0]           = new stdClass();
$orderTemplate->prices[0]->id       = $priceId;
$orderTemplate->endPointVlanId = $endPointVlanId;
$orderTemplate->quantity            = $quantity;


$orderTemplate->itemCategoryQuestionAnswers = array();

// the item category question answers
$itemCategoryQuestionAnswer = new stdClass();
$itemCategoryQuestionAnswer->categoryId = 313;
$itemCategoryQuestionAnswer->categoryCode = 'sov_sec_ip_addresses_pub';
$itemCategoryQuestionAnswer->questionId = 14;
$itemCategoryQuestionAnswer->answer = '1';  // TOTAL_IPS_IN_30_DAYS
$orderTemplate->itemCategoryQuestionAnswers[] = $itemCategoryQuestionAnswer;

$itemCategoryQuestionAnswer = new stdClass();
$itemCategoryQuestionAnswer->categoryId = 313;
$itemCategoryQuestionAnswer->categoryCode = 'sov_sec_ip_addresses_pub';
$itemCategoryQuestionAnswer->questionId = 15;
$itemCategoryQuestionAnswer->answer = '3';  // # TOTAL_IPS_IN_12_MONTHS
$orderTemplate->itemCategoryQuestionAnswers[] = $itemCategoryQuestionAnswer;

$itemCategoryQuestionAnswer = new stdClass();
$itemCategoryQuestionAnswer->categoryId = 313;
$itemCategoryQuestionAnswer->categoryCode = 'sov_sec_ip_addresses_pub';
$itemCategoryQuestionAnswer->questionId = 16;
$itemCategoryQuestionAnswer->answer = 'Reason for IPs';  // REASON_FOR_IPS
$orderTemplate->itemCategoryQuestionAnswers[] = $itemCategoryQuestionAnswer;

$itemCategoryQuestionAnswer = new stdClass();
$itemCategoryQuestionAnswer->categoryId = 313;
$itemCategoryQuestionAnswer->categoryCode = 'sov_sec_ip_addresses_pub';
$itemCategoryQuestionAnswer->questionId = 9;
$itemCategoryQuestionAnswer->answer = 'Contact Name';  // CONTACT_NAME
$orderTemplate->itemCategoryQuestionAnswers[] = $itemCategoryQuestionAnswer;

$itemCategoryQuestionAnswer = new stdClass();
$itemCategoryQuestionAnswer->categoryId = 313;
$itemCategoryQuestionAnswer->categoryCode = 'sov_sec_ip_addresses_pub';
$itemCategoryQuestionAnswer->questionId = 10;
$itemCategoryQuestionAnswer->answer = 'Contact Job Title';  // # CONTACT_JOB_TITLE
$orderTemplate->itemCategoryQuestionAnswers[] = $itemCategoryQuestionAnswer;

$itemCategoryQuestionAnswer = new stdClass();
$itemCategoryQuestionAnswer->categoryId = 313;
$itemCategoryQuestionAnswer->categoryCode = 'sov_sec_ip_addresses_pub';
$itemCategoryQuestionAnswer->questionId = 11;
$itemCategoryQuestionAnswer->answer = 'contact.email@email.com';  // # CONTACT_EMAIL
$orderTemplate->itemCategoryQuestionAnswers[] = $itemCategoryQuestionAnswer;

$itemCategoryQuestionAnswer = new stdClass();
$itemCategoryQuestionAnswer->categoryId = 313;
$itemCategoryQuestionAnswer->categoryCode = 'sov_sec_ip_addresses_pub';
$itemCategoryQuestionAnswer->questionId = 12;
$itemCategoryQuestionAnswer->answer = '77778727';  // # CONTACT_PHONE_NUMBER
$orderTemplate->itemCategoryQuestionAnswers[] = $itemCategoryQuestionAnswer;

$itemCategoryQuestionAnswer = new stdClass();
$itemCategoryQuestionAnswer->categoryId = 313;
$itemCategoryQuestionAnswer->categoryCode = 'sov_sec_ip_addresses_pub';
$itemCategoryQuestionAnswer->questionId = 13;
$itemCategoryQuestionAnswer->answer = true;   // CONTACT_VALIDATED - I agree that the contact information is current and valid.
$orderTemplate->itemCategoryQuestionAnswers[] = $itemCategoryQuestionAnswer;

/**
 * Create a client to the API service.
 */
$client = SoftLayer_SoapClient::getClient($serviceName, null, $apiUsername, $apiKey);


// Create a SoftLayer API client object to the SoftLayer_Product_Order service.
$client = SoftLayer_SoapClient::getClient
    (
        'SoftLayer_Product_Order',
        null,
        $apiUsername,
        $apiKey
    );

// Place the order for the new subnet.
try {
    // Re-declare the order template as a SOAP variable, so the SoftLayer
    // ordering system knows what type of order you're placing.
    $orderTemplate = new SoapVar
    (
        $orderTemplate,
        SOAP_ENC_OBJECT,
        'SoftLayer_Container_Product_Order_Network_Subnet',
        'http://api.service.softlayer.com/soap/v3/'
    );

    // verifyOrder() will check your order for errors. Replace this with a call
    // to placeOrder() when you're ready to order. Both calls return a receipt
    // object that you can use for your records.
    //
    // Once your order is placed it'll go through SoftLayer's approval and
    // provisioning process. When it's done you'll have a new
    // SoftLayer_Network_Subnet object ready to use.
    $receipt = $client->verifyOrder($orderTemplate);
    print_r($receipt);
} catch (Exception $e) {
    echo 'Unable to place subnet order: ' . $e->getMessage();
}

```
