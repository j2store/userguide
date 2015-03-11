# Barclays ePDQ Payment Plugin

This plugin integrates the Barclays ePDQ payment gateway with the J2Store shopping cart.

#### Requirements
* PHP 5.3 or higher
* Joomla 2.5.x/3.0x
* J2Store 2.7.3 + (Note the plugin will not work with earlier versions of J2Store)

#### Required ePDQ settings
Login to your ePDQ Barclayscard merchant account.
Go to Confgurations → Technical Information

#### Global Transaction Parameters
##### Default operation code

You have two default operation code, **Sale** and **Authorization**. The brief description of both is given below.

**Sale**

This will enable you to receive instant payment

**Authorization**

You have to capture this either manually or automatically.

For Sale, a successful payment will return Status code 9 and for a Successful Authorisation, the status code is 5. Both the cases will be treated as Success and Confrmed by the **ePDQ** plugin.

>NOTE: If you are selling digital goods, it is advised to use SALE as operation code

Check the image below for a clear understanding.

![EPDQ Plugin](epdq_plugin_1.png)

The following parameters for technical information in your **ePDQ** account should be set as instructed below.

##### Hashing method (Tab: Security)
This should be set to SHA-1, as the plugin will not function with other methods. Check the image on how to do this.

![Hashing Method](hashing_method.png)







