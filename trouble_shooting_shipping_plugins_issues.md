#Troubleshooting shipping methods

* [Introduction](#introduction)
* [Common Issues](#common_issues)
	* [Enable Shipping](#enable_shipping)
	* [Geozone](#geozone)
* [Issues specific to Standard Shipping methods](#issues-standard-shipping)
	* [Set Rates](#set_rates)
* [Issues specific to USPS, FedEx, UPS, CanadaPost, Australia Post](#specific-plugins)
	* [Weight and Dimensions](#weight_dimension)
	* [API credentials](#api_credentials)
	* [Currency](#currency)
	* [UPS accepted measurements](#ups_measurements)
* [Debug Mode](#debug_mode)

<a name="introduction" />
##Introduction
You have installed the shipping plugin but it doesn't show up during the checkout. Here are a list of reasons that might be preventing the plugin from fetching shipping cost real-time from the APIs of the Shipping carrier.

<a name="common_issues"></a>
##Common Issues

There are certain common issues that prevents the shipping methods from showing up in the checkout.

<a name="enable_shipping"></a>

###Enable Shipping

Well. This might sound trivial. But some of us often forget to turn on the Enable shipping switch while creating the product. Make sure that Enable shipping is set to YES.
By default, Enable Shipping is set to NO. So this should be your first check.

<a name="geozone"></a>

###Geozone

All the plugins come with a geozone filter setting.

In **Standard shipping methods**, all the shipping rates are geozone specific. So you MUST configure the geozones correct before you set up the shipping cost.
![shipping geozone setting](./assets/images/shipping_geozone.jpg)

Geozones are nothing but a group of countries / zones.
For example, shipping cost to a group of countries will be same. So those countries could be grouped to form a geozone.

Based on the shipping address provided by the customer, the system will look up for a shipping method and the rate and display it to the customer.

> **NOTE**
> If you ship your goods to the entire world and use shipping plugins like USPS, FedEx or UPS, you will have a param called: All geozones. Choosing this will allow the plugin to work for all shipping locations. Check the screenshot below

![shipping geozone setting](./assets/images/shipping_geozone_setting.png)
<a name="issues-standard-shipping" />
##Issues specific to standard shipping methods

J2Store comes with seven standard shipping methods built-in. The following are some of the common issues.

<a name="set_rates" />
###Set Rates
After creating a shipping method (by going to J2Store admin -> Set up -> Shipping -> Standard Shipping Methods), you can see a link named Set Rates. Click on it to set the shipping rates for the chosen shipping type.

<a name="specific-plugins" />
## Issues specific to plugins like USPS, FedEx, UPS, CanadaPost, Australia Post

Shipping carriers have different limitations in the methods offered by them. For example, UPS only accepts Pound / Inch, Kilogram / Centimetre as the weight / dimension combination. A change in this would result in an error and no methods will be shown. 

The following are common issues which affect the display of shipping methods.

<a name="weight_dimension"></a>

###Weight and Dimensions

All the shipping carriers use the weight and the dimension of your product (Length, Width & Height) of your products ) to calculate the shipping cost (besides using the destination address). So make sure that you enter the Weight and the dimension of your product.

You should select the weight and the length measurement unit from the drop down list.

![shipping dimension](./assets/images/weight_and_dimensions.png)

Also make sure that you choose the correct measurement units in the plugin settings as well. If the measurement units used in the products does not match with the settings in the plugin, then J2Store will attempt to convert the values to the measurement unit set in the plugin.

<a name="api_credentials"></a>

###API credentials

All shipping carriers have a web service and provide credentials to access their Rate API. Some of the carriers like USPS offer TEST accounts as well.  Make sure you enter these credentials correctly in the Plugin. Some of the carriers provide Customer number (like Canada Post ) and a few other parameters as well. Refer the documentation PDF that come with each plugin for more information.

<a name="currency"></a>

### Currency
In USPS shipping plugin, if the shipping server is queried, the server will return the list of options and their corresponding rates in US $. The shipping plugin may not show the rates if USD is not present in your list of currencies and you have configured a currency other than the US $, like CAD or AUD. To avoid this issue, you must have USD as a currency  in your list of currencies. This will solve the issue.

<a name="ups_measurements" />
### UPS accepted measurements
Only KG (Kilogram) and LB (Pound) are supported by UPS as the weight measurement units.  Similarly, only IN (Inch) and CM (Centimetres) are supported as length measurement units.

And there is more.  If you use Pound (LB) as the weight measurement, then the length measurement should be Inch (IN). Similar if KG is used, then CM should be the measurement. A wrong combination will result in an error.

<a name="debug_mode"></a>
## Debug Mode

In your plugin settings, set the Debug mode to YES. This will allow the plugin to log the responses sent by the APIs of the shipping carriers.

The log is stored in the /cache folder of your Joomla Root. You can use your Hosting CPanel's file manager or an FTP program like FileZilla to access the log file. The log should give you a lot of information.

VERY IMPORTANT: Debug mode SHOULD NOT be enabled in LIVE / PRODUCTION sites.

![debug mode](./assets/images/debug_mode.png)

Still not working, please create a private ticket or email us the log file. We will help you troubleshoot.