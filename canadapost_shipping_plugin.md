# Canadapost Shipping Plugin

This plugin integrates Canada Post Shipping Rate API with J2Store. It integrates the RESTful API of the Canada Post.

#### Requirements
* PHP 5.3+
* Joomla 2.5 / 3.x +
* J2Store 2.6.8 +
* cURL

#### Installation
You can install the plugin through the standard Joomla installer.

#### Configuration
Prior to configuring the plugin, you should have an active account with the CanadaPost and received API keys. Contact CanadaPost to register and get API keys.
1. Make sure that you have set the Default Weight Class to Kilogram (KG) or Pound (LB) in the J2Store admin –> Set up –> Store Profiles –> Your Store profile
2. Make sure that you entered your Postal Code / Zip correct in your Store Profile
3. Make sure that you have set the Dimensions and Weight fields in your products correctly
4. Make sure that you have set the Enable Shipping to YES in your products
5. Open the Canada Shipping Plugin and set the Following Parameters

**API Username**

Your CanadaPost username

**API Password**

Your CanadaPost password

**Customer Number**

The customer number provided by the CanadaPost.

**Handling cost**

You can enter an amount here (without any symbols or letters). It will be added as a handling cost in addition to the shipping cost.

**Show delivery time**

Set this to Yes, if you want to show the expected delivery time to the customers.

















