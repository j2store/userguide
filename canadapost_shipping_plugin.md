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
2. Make sure that you entered your Postal Code/Zip correct in your Store Profile
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

**Test mode**

If you would like to test the API, set this to **Yes**. Otherwise, you can set this to **No**.

**Weight Unit**

Valid Units are: Kilogram (KG), Pound (LB).

>**IMPORTANT**
Make sure to set your default weight class to either KG or LB in your storeprofile. All your products should be using the same weight class

**Length Unit**

The length unit. The plugin will not convert the length unit. Make sure that you are using the same length unit for all your products.

**Tax Class**
If you want to charge tax for shipping cost, choose a tax class here. Otherwise, leave this field empty/donot select any option.

**Geozone**

You can select a geozone and restrict the availability of this shipping method to the countries/zones in that geozone. Leave empty/unselected for making this shipping method available to customers from all regions.

**Debug**

If you set this to **Yes**, then debug messages will be logged and saved in the cache folder in your Joomla root directory.
Set this to **No** in Live websites.

#### Support
You can contact ***support@j2store.org*** if you have any questions.













