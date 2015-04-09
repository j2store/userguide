# Telecash Payment Plugin


This plugin integrates J2Store with the Telecash payment system.

#### Requirements 
* PHP 5.2 or higher 
* Joomla 2.5.x 
* J2Store 2.0 or above 

#### Installation Instructions 
1. Use the Joomla installer to install the plugin. 
2. In the backend, go to Extensions->Plugin Manager and open the Telecash
plugin. (type=**j2store**). 
3. Enable the plugin 
4. Enter the parameters (read the explanation about each parameter given below) 
5. Save and close it. 

#### Parameters

##### Store ID
Store ID provided by Telecash.

##### Shared Secret
Secret key provided by Telecash.

##### Transaction Type
Sale - Captures the amount immediately. 
Authorize - the charge issues an authorization (or pre-authorization), and will need to be captured later. Default is sale

##### Use Telecash Sandbox
Telecash offers a testing suite. Before going live, you can test your store using the sandbox feature.

>IN LIVE SITE, THIS SHOULD BE SET TO NO.

##### Joomla Article ID for custom thank you message
You can create an Article ID with a message enter its ID here to show it to the customer after completion of the purchase.

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
Still have questions? You can post your questions in our support forum: http://j2store.org/forum/index.html