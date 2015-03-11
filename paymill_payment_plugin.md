# Paymill Payment Plugin


This plugin integrates Paymill payment gateway with J2Store. 

#### Installation 

You can install the plugin through the standard Joomla installer. 

#### Configuration 

**Payment Option title**

Enter a name that will be shown in the payment methods 
selection during the checkout process. Default Paymill

**Live Private Key**

Enter your live account's Private API Key. 

**Live Public Key**

Enter your live account's Public API Key 

**Test mode**

This option allows you to test the plugin with Paymill in test mode instead of the live one. 

>IMPORTANT: NEVER ever set this to yes when your shop is live. 

**Test Private Key**

Enter your test Private API Key here. 

**Test Public Key**

This is the test public key to be used while testing the shop. You can find these keys under your account settings. 

**Article ID for Thank you message**

You can create an article with a thank you or instructions or information to the customer and enter its ID here. This will be displayed to the customer when he returns to the site after making payment.

**Display text on selection**

The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the tips below

>Tip - ONLY FOR MULTI-LINGUAL SITES

For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON_SELECTION.

Now you can go to Joomla admin-> Language Manager->Overrides and create overrides for the language constant in all your languages.

**Display text before payment**

The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text after payment/order**

The text entered here will be displayed to the customer after he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment**

The text entered here will be displayed to the customer when there is an error in the payment process.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on cancel payment**

The text entered here will be displayed to the customer when he cancels the payment at the gateway (NOT in your site).

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment Button Text**

The text of the payment button. The button will be displayed at the final checkout step.

#### Support

Still have questions? You can reach us in ***support@j2store.org*** or post in our support
forum: http://j2store.org/forum/index.html

Thank you for using our extension.











