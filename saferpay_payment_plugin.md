# Saferpay Payment Plugin

This plugin integrates the SaferPay payment gateway with J2Store.

#### Installation
Install using the standard Joomla installer. 

Then go to Joomla administration->J2Store → Set up → Payment → SaferPay → Edit paramters. 

Fill in the fields, save and enable the plugin.

#### Configuration Params

##### Payment Option Title
Enter a title here to show during the payment selection in checkout.

##### Account ID
The Account ID provided by the SaferPay.

You can get the Account ID from your SaferPay Merchant Backoffice. Go to My Saferpay → Saferpay Ecommerce → Accounts to find the account ID. Or Contact SaferPay support to know your Account ID.

##### Enable test mode
Set yes to test the plugin's integration with the SaferPay test server.

##### Joomla Article ID for custom thank you message
You can create an article with a custom messsage to show after the customer completes the purchase. Enter the Article ID here.

##### Display text on selection
The text entered here will be displayed when customer selects this payment method. 

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below.

>Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant: 
J2STORE_TEXT_TO_DISPLAY_ON_SELECTION

Now you can go to Joomla admin-> Language Manager->Overrides and create overrides for the language constant in all your languages. 

##### Display text before payment

The text entered here will be displayed to the customer at the order summary screen before he makes the payment. 

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

##### Display text after payment/order
The text entered here will be displayed to the customer after he makes the payment. 

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

##### Display text on error in payment
The text entered here will be displayed to the customer when there is an error in the payment process.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

##### Display text on cancel payment
The text entered here will be displayed to the customer when he cancels the payment at the gateway (NOT in your site).

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

##### Payment Button Text

The text of the payment button. The button will be displayed at the final checkout step.

#### Support
Still have questions? You can post your questions in our support forum: http://j2store.org/forum/index.html

Thank you for using our extension. 