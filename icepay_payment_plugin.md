# IcePay Payment Plugin

This plugin integrates the IcePay Payment gateway with J2Store shopping cart.

#### System Requirements
* Joomla 2.5 / Joomla 3.x
* J2Store 2.6.7 +

#### Installation
Go to Joomla admin – Extensions manager to install the plugin.

#### Setting up the plugin
Go to the Plugin manager and open IcePay plugin.

Enter the Merchant ID and the Secret. You can find the Merchant ID and secret in your IcePay dashboard → My Websites → Your website

Click Save.

Now you will see the payment Methods available for your IcePay account.

Choose the methods that you want to offer to your customers. You can choose all of them as well.

Save

#### Configuring IcePay
Login to your IcePay dashboard.

Go to My Websites → Your website → Configure URL tab

Copy paste the following url in Thank you page, Error URL and PostBack Url fields

http://yourdomain.com/index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=payment_icepay&paction=process

NOTE: replace <yourdomain.com> with your domain name.

#### Plugin Parameters

**Payment option title**

The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Merchant ID**

The merchant ID provided by IcePay 

**Secret**

A secret key provided by IcePay

**Payment Methods**

List of payment methods available for your IcePay account. Refer the Configuring IcePay account section for information.

**Article ID for Thanks Message**

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

**Payment Button Text**

The text of the payment button. The button will be displayed at the final checkout step.

#### Support

Still have questions? You can reach us in ***support@j2store.org*** or post in our support
forum: http://j2store.org/forum/index.html

Thank you for using our extension.