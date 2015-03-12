# Tranzila Payment Plugin













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

##### Testing Information
You may use a dummy number which simulates a ***Visa card*** number – 4444333322221111.

The CVV should be any three digit number, for example - 333.

Another dummy number to simulate ***Isracard*** is 12312312.

Contact **Tranzilla** for more information on test credit cards.

##### Troubleshooting
When submitting an order, J2Store may return an error about

"**Credit cart could not be processed...**" 

This might not necessarily mean it isn't working. 

You can check it in two places:

1) In the **Tranzila** account go to Transactions >> Today >> All, and see if your order was registered. If so, it means it worked ok on your settings are correct. The fact that it didn't return "000" (Payment accepted) as a response. Perform some more test purchases. If the problem persists, contact the **Tranzila** Support.

2) If your order was not registered in your **Tranzila**, then it means wrong settings. Check your server IP and make sure your entered the IP correctly.

#### Support
If you encounter any issues with the plugin, please contact the support team at ***support@j2store.org***.

