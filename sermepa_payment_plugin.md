# Sermepa Payment Plugin

This plugin integrates the TPV RedSys / Servired / Sermepa  payment system used by Spanish banks. It supports banks including -  La Caixa, Banco Sabadell, Caixa Penedes, Caja Rural, Unnim, Deutsche Bank. 

Full list can be read from here: http://www.servired.es/espanol/miembros.htm

#### Configuration Parameters
##### Payment option title
The value entered here will be used as the title for this payment method. Customer will see this value when he checks out. 

##### Payment Page title
Title displayed in the payment page of TPV Redsys/servied / sermepa gateway. Add a Title, ex: “La Caixa”.

##### Commerce number (número de comercio)(FUC)
The merchant commerce number provided by your bank

##### Commerce signature (secret) key
A secret key provided by your bank / payment gateway

##### Terminal Number (número de terminal)
The terminal number provided by your bank / the payment gateway

##### Method of Encryption
Encryption standard. It would be either sha1-enhanced or sha.

SHA1-Enhanced will be used by most of the banks. Read your Bank welcome documentation. 

##### Use Sandbox/test mode
Enable this to test your integration with the TPV Redsys / Servired /Sermepa test system. Your bank will provide the test credentials.

First turn this on and test your integration. Once you are ready, contact with your Bank and once you are live, disable this.
















##### Display Text on Selection
The text entered here will be displayed when customer selects this payment method. 

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below.

>Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant: 

J2STORE_TEXT_TO_DISPLAY_ON_SELECTION 

Now you can go to Joomla admin-> Language Manager->Overrides and create overrides for the language constant in all your languages. 

##### Display Text before Payment
The text entered here will be displayed to the customer at the order summary screen before he makes the payment. 

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter. 

##### Display Text after Payment/Order
The text entered here will be displayed to the customer after he makes the payment. 

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

##### Display Text on Error in Payment
The text entered here will be displayed to the customer when there is an error in the payment process.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

##### Display Text on Cancel Payment
The text entered here will be displayed to the customer when he cancels the payment at the gateway (NOT in your site).

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

##### Payment Button Text
The text of the payment button. The button will be displayed at the final checkout step.

#### Support
If you encounter any issues with the plugin, please contact the support team at ***support@j2store.org***.