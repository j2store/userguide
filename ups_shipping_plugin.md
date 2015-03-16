# UPS Shipping Plugin

This plugin integrates UPS Shipping Rate API with J2Store.

### Requirements
* PHP 5.3+
* Joomla 2.5 / 3.x +
* J2Store 2.6.7 +

### Installation
You can install the plugin through the standard Joomla installer.

### Configuration
Prior to configuring the plugin, you should have an active account with the UPS and received API keys. Contact UPS to register and get API keys

#### Access Key
Enter the access key provided by the UPS.

#### Username
Your UPS username

#### Password
Your UPS password

#### Shipper Number
This is actually the shipping account number provided by the UPS.

#### Test mode
If you would like to test the API, set this to '**Yes**'. Otherwise, you can set this to **NO**.

#### Services
Choose the shipping services that you would like to provide to the customers.

>NOTE: Services depend on the customer's shipping address. Even if you chose many services here, UPS will show only the services that are available to the customer's shipping
destination at the checkout.

#### Pickup Type
Choose your Pickup type

#### Packaging
Choose your packaging option. Default: Package

#### Customer classification
Wholesale - If you are billing to a UPS account and have a
daily UPS pickup, Occasional - If you do not have a UPS account or you are billing to a UPS account but do not have a daily pickup, Retail - If you are shipping from a retail outlet (only
used when origin is US)

#### Weight Unit
Valid Units are: Kilogram (KGS), Pound (LBS).

>IMPORTANT: You must choose a weight unit here. Otherwise, the plugin will not work. If you are using more than one weight unit for your products, then the plugin willautomatically convert to the weight unit you are choosing here.

**Example**
Product A – Weight is 5 KG , Product B – Weight 7 Pounds.

You have set the Pound as the weight unit in the plugin params.
Then the Product A weight will be converted to pound, according to the values provided at the Weight Classes section (J2Store admin – set up – weight classes)

#### Show Weight Total
Set this to yes to show the total weight of the products in the
order to the customer during the checkout. The weight will appear next to the shipping method name

#### Length Unit
The length unit.

The plugin will not convert the length unit. Make sure that you are using the same length unit for all your products.

#### Tax Class
If you want to charge tax for shipping cost, choose a tax class here. Otherwise, leave this field empty / do not select any option.

#### Geozone
You can select a geozone and restrict the availability of this shipping method to the countries/zones in that geozone. Leave empty / un selected for making this shipping method available to customers from all regions.

#### Debug
If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory.

>Set this to NO in Live websites.

### Support
You can contact ***support@j2store.org*** if you have any questions.