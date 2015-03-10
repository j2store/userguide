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

This is an optional parameter.

>NOTE: DO NOT enter any symbol like % here. Leave empty if you dont want to charge.

**Surcharge Fixed**

You can collect a fixed surcharge / fee from your customers in addition to the order value. You can enter a value here (for example: 2 ). If you enter 2 here, then 2 will be added as a
handling cost to the order. Leave empty if you dont want to charge.

This is an optional parameter.

**Currency Code**

Currency code provided by DIBS refer:
http://www.dibs.se/toolbox/currency_codes/ eg: 208 for DKK

**Use DIBS Sandbox**

For testing purposes, set this parameter to **Yes**.

>Important: IT SHOULD BE SET TO "**NO**" IN LIVE SYSTEMS.

**Thanks Message Joomla Article ID**

You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Display text on selection**

The text entered here will be displayed when customer selects this payment method.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. 

Refer the tips below

>Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON_SELECTION.

Now you can go to Joomla admin-> Language Manager->Overrides and create overrides for the language constant in all your languages.

**Display text before payment**

The text entered here will be displayed to the customer at the order summary screen before he makes the payment.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order**

The text entered here will be displayed to the customer after he makes the payment.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment**

The text entered here will be displayed to the customer when there is an error in the payment process.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment**

The text entered here will be displayed to the customer when he cancels the payment at the gateway (NOT in your site).

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.















