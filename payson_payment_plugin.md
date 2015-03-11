# Payson Payment Plugin

This plugin integrates the Payson Payment gateway with J2Store.

#### Installation
Use the Joomla extensions installer to install the plugin.

#### Plugin Configuration

Go to Joomla admin → Plugin Manager and open the Payson plugin.

The plugin has following options: 

##### Payment option title
The value entered here will be used as the title for this payment method. Customer will see this value when he checks out. 

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