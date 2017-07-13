# Afterpay

This plugin integrates Afterpay payment API with J2Store Joomla eCommerce solution.

#### Requirements

* PHP 5.4 or higher
* Joomla 3.x
* J2Store 3.2.x or higher

#### Installation

1. Download the plugin from our site and install it using Joomla installer.
2. In the backend, go to J2store Dashboard -> Payment methods and enable plugin.

3. Open the plugin and enter the parameters (read the explanation about each parameter given below)

4. Save and close it.

#### Configuration

**Payment option title**

The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Plugin Display Image**

This image will be displayed while payment options are listed in the checkout page.

**Payment process type**

***Authorise:*** If the merchant would like to put the payment on hold, then choose authorise as the payment process type.

***Capture:*** Choose capture as the payment process type, when the merchant is ready to finalise the payment.

**Merchant Id**

Enter your valid merchant ID associated with your afterpay live account.

**Merchant secret key**

Enter valid secret key of your afterpay payment live account.
![afterpay-setting-1](./assets/images/afterpay_01.png)

**Sandbox mode**

If you are having test account with afterpay, you will have to choose sandox feature. Choose **YES** to enable sandbox feature.

**Test Merchant ID**

Enter valid merchant ID of your afterpay test account.

**Merchant secret key**

Enter valid secret key of your afterpay test account.

**Article ID for thank you message**

Create Joomla Article with content which says thank you message. Enter the article ID in the text box provided. Users will see this content when they successfully completes payment and redirect to the store.

**Geozone**

By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**Display text on selection**

The text entered here will be displayed when customer selects this payment method. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override.
For example, enter a language constant:

J2STORE_TEXT_TO_DISPLAY_ON_SELECTION.

Now you can go to Extensions -> Language ->Overrides and create overrides for the language constant in all your languages.

**Display text before payment**

The text entered here will be displayed to the customer at the order summary screen before he makes the payment. You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the Display text on selection parameter.
![afterpay-setting-2](./assets/images/afterpay_02.png)

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

Choose **YES** to enable the debug mode. If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. **DO NOT** select **YES** in the live site.
![afterpay-setting-3](./assets/images/afterpay_03.png)

#### Support

Still have questions? You can post in our support forum: http://j2store.org/forum/index.html

Thank you for using our extension.