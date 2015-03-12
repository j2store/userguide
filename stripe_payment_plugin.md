# Stripe Payment Plugin

The plugin integrates Stripe payment gateway with J2Store. It works and compatible with the latest Stripe API : 2014-01-31 (latest)

#### Installation
You can install the plugin through the standard Joomla installer.

#### Configuration
##### Payment Option title
Enter a name that will be shown in the payment methods
selection during the checkout process. Default Stripe.

##### Live Secret API Key
Enter your live Stripe account's Secret API Key.

##### Live Publishable Key
Enter your live Stripe account's Publishable API Key.

##### Charge mode
Choose the charge mode. Sale - Captures the amount immediately.
Authorize - the charge issues an authorization (or pre-authorization), and will need to be captured later. Uncaptured charges expire in 7 days, Default is sale

##### Use Stripe Sandbox
This option allows you to test the plugin with Stripe in test mode instead of the live one.

>IMPORTANT: NEVER ever set this to yes when your shop is live.

##### Test Secret API Key
This is the test key to be used while testing the shop. You can find these keys under your account settings.

##### Test Publishable Key
Enter your test Stripe account's Publishable API Key here.

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
If you encounter any issues with the plugin, please contact the support team at ***support@j2store.org***.