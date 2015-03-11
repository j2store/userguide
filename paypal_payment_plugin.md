# Paypal Payment Plugin

The Paypal Plugin for J2Store enables you to receive payments via Paypal Payment Gateway. This integrates the Paypal's Website Standard Payment API. 

#### Requirements 
* PHP 5.2 or higher 
* Joomla 2.5.x 
* J2Store 2.0 or above 

#### Installation Instructions 
1. Use the Joomla installer to install the plugin. 
2. In the backend, go to Extensions->Plugin Manager and open the Paypal Payments 
plugin. (type=**j2store**). 
3. Enable the plugin 
4. Enter the parameters (read the explanation about each parameter given below) 
5. Save and close it. 

Now you can see the Paypal Payments as an option during the Check out process. 

#### Parameters 
**Paypal Merchant Email Address**

This is your original paypal email/merchant email address, which you have used in Paypal. 

**Surcharge Percentage**

You can collect a percent of the total order value as surcharge / fee for using the Paypal option from your customers using this option.  You can enter a value here (for example: 2 ).  If you enter 2 here, then 2 % of the total order value will be added as a handling cost to the order.

This is optional parameter.

>NOTE: DO NOT enter any symbol like % here.

Leave empty if you dont want to charge.

**Surcharge Fixed**:

You can collect a  fixed surcharge / fee for using the Paypal option from your customers in addition to the order value.  You can enter a value here (for example: 2 ).  If you enter 2 here, then 2 will be added as a handling cost to the order.

Leave empty if you dont want to charge.

This is an optional parameter.

**Use SSL to post back to Paypal?**

If you are using SSL certificate (https), enable this with a **Yes**. If you dont know what SSL is, better leave it as **No** 

**Use Paypal Sandbox**

Paypal offers a testing suite called Sandbox. Before going live, you can test your store using the Paypal's sandbox feature. Read more about Paypal Sandbox at developer.paypal.com.

>IN LIVE SITE, THIS SHOULD BE SET TO NO. 

**Paypal Sandbox Merchant Email**

Your paypal sandbox email. 

**Article ID for Thanks you message**

You can create an article to say thanks, provide some information or instructions to the customers, who purchased in your online store. Enter the Article ID here. This will show, 
when customers return from the paypal. 

**Geozone**

By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**PayPal Callback Text**

What the button on the PayPal site reads after the user has completed his transaction. Leave empty for the default 'Return to the merchant website' text. 

This is an optional parameter.

**Custom Header Image **

The URL to your logo so. This image will be displayed on the top of PayPal's checkout page instead of your merchant name. 

>WARNING! It must be an HTTPS URL, otherwise your clients will 
receive warnings about insecure content. 

This is an optional parameter.

**Header Background Colour**

The hex-code of your PayPal checkout page's header, e.g. FFFFFF for white (note: place no # in front the hex value) 

This is an optional setting.

**Header Background Colour**

The hex-code of your PayPal checkout page's header, e.g. FFFFFF for white (note: place no # in front the hex value) 

This is an optional setting.

**Header Border Color** 

The hex-code of your PayPal checkout page's header border, e.g. FFFFFF for white (note: place no # in front the hex value) 

This is an optional setting.

**Logo Image for display in Paypal**

The URL of the 150x50-pixel image displayed as your logo in the upper left corner of PayPal’s pages. Default: your business name (if you have a Business account) or your email address (if you have Premier account). If this is not working, try using the Custom Header Image param above. 

This is an optional setting.






