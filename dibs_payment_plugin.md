# DIBS Payment Plugin

The DIBS Plugin enables you to receive payments via DIBS Payment Solution, a leading payment solution provider in Nordic countries. http://www.dibspayment.com/
>NOTE: The Plugin uses the Flexwin payment method . Please refer more about this integration method in http://tech.dibs.dk/integration_methods/flexwin/flexwin_introduction/

#### Requirements
* PHP 5.2 or higher
* Joomla 2.5.x
* J2Store 2.0.2 or above

#### Installation Instructions

1. Use the Joomla installer to install the plugin.
2. In the backend, go to Extensions->Plugin Manager and open the DIBS Payments plugin
(type = **j2store**).
3. Enable the plugin
4. Enter the parameters (read the explanation about each parameter given below)
5. Save and close it.

Now you can see the DIBS Payments as an option during the Check out process.

#### Configuration

The plugin has the following parameters need to be addressed:

**Payment option title**

The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**DIBS Merchant Name**

The Unique Merchant ID number provided by the DIBS

**Surcharge Percentage**

You can collect a percent of the total order value as surcharge / fee from your customers using this option. You can enter a value here. ( for example: 2 ) If you enter 2 here, then 2% of the total order value will be added as a handling cost to the order.

>NOTE: DO NOT enter any symbol like % here. Leave empty if you dont want to charge.








