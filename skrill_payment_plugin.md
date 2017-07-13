# Skrill Payment Plugin

#### Introduction
The Skrill Payment Plugin for J2store to pay online transaction amount for a product.

#### Requirements
* PHP 5.2 or higher
* Joomla 2.5 or above
* J2Store 2.7.3 or above

#### Installation
1. Use Joomla installer to install the plugin
2. At the backend, go to **Extension -> Plugin Manager** and open the **Skrill**(type=j2store)
3. Enable plugin
4. Enable plugin params

#### Params
**1. Payment Option Title:**
If required, enter Option Title. This text will be displayed while listing the payment option.

**2. Image or Logo:**
If required, Select image or logo . This image will be displayed while listing the payment option and before pay order.

**3. Merchant ID:**
Please enter the merchant ID associated with **Skrill** account.

**4. Merchant Email:**
Please enter the merchant email associated with **Skrill** account.

**5. Secret Word:**
Please enter the secret word associated with **Skrill** account.

**6. Use PaySkrill Sandbox:**
This option is used to test **Skrill** payments.

**7. Test Merchant ID:**
Please enter the Test Merchant ID associated with **Skrill** account.

**8. Test Merchant Email:**
Please enter the Test Merchant Email associated with **Skrill** account.

**9. Test Secret Word:**
Please enter the test secret word associated with **Skrill** account.

**10. Thankyou page article ID:**
Please enter article id for displaying Thankyou page.

**11. Display text on selection:**
The text entered here is displayed when a customer selects this payment method. You can enter a language constant as a value here, if you are using a multi-lingual site and 	then write a language override. Refer the tips below

***Tip*** 

**	ONLY FOR MULTI-LINGUAL SITES**

For example, enter a language constant: 

	J2STORE_TEXT_TO_DISPLAY_ON_SELECTION. 

Now, you can go to **Joomla Admin -> Language Manager -> Overrides** and create overrides for the language constant in all languages. 

**12. Display Text before payment:**

The text entered here is  displayed to the customer at the order summary screen before he makes the payment. 
	
You can enter a language constant as a value here, if you are using a multi-lingual site and then write a language override. Refer the *Display text on selection param.* 

**13. Display Text on error in payment:**

The text entered here is displayed to the customer when there is an error in the payment process.

You can enter a language constant as a value here if you are using a multi-lingual site and then write a language override. Refer the *Display text on selection param.*

**14. Debug:**

This option is used to enable/disable log file.

**15. Payment Button Text:**

The text of the payment button. The button will be displayed at the final checkout step. 

#### Support 

Still have questions? You can reach us in support@j2store.org 

Thank you for using our extension.