#PayGate Payment

The plugin integrates Paygate payment with J2Store Joomla eCommerce solution. Paygate helps webshops and online merchants to accept credit card / alternative payments and also can process online payments quickly, securely and efficiently.

####System Requirements

1. PHP 5.4 or greater

2. Joomla 3.x

3. J2Store 3.2.x or greater

####Installation Instructions

1. Use the Joomla installer to install the plugin.

2. In the backend, go to J2store Dashboard -> Payment methods and enable plugin.

3. Open the plugin and enter the parameters (read the explanation about each parameter given below)

4. Save and close it.

####Configuration

**Payment option title**

The value entered here will be used as the title for the payment. Customer will see this value when he checks out.

**Plugin display image**

This image will be displayed while payment options are listed in the checkout page.

**PayGate ID**

Enter the ID associated with your PayGate payment account.

**PayGate encryption / secret key**

Enter the secret key of your PayGate payment account.

**Use PayGate test mode**

Choose **Yes** to use the PayGate payment in test mode.
![](assets/images/paygate_01.png)

**Test PayGate Id**

Enter the Test ID of your PayGate payment test account.

**PayGate encryption / secret key**

Enter the secret key of your PayGate payment account.

**Locale (language)**

Payment page form will be displayed in the language chosen here.

**Article ID for Thank You message**

You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

**Geozone**

By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**Display text on selection**

The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON_SELECTION.

Now you can go to Joomla admin-> Language Manager->Overrides and create overrides for the language constant in all your languages.

**Display text before payment**

The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.
![](assets/images/paygate_02.png)

**Display text on after payment**

The text entered here will be displayed when customer completes the payment.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text on error in payment**

The text entered here will be displayed to the customer when there is an error in the payment process.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Display text if customers cancels payment**

The text entered here will be displayed to the customer when he cancels the payment at the gateway (NOT in your site).

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.

**Payment button text**

Text entered here will be added as the name of the payment button.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.

**Debug**

Choose YES to enable the debug mode. If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. DO NOT select YES in the live site.
![](assets/images/paygate_03.png)

**Support**

Still have questions? You can post in our support forum: http://j2store.org/forum/index.html

Thank you for using our extension.