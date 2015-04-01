# Troubleshooting Paypal Related Issues

There could be several reasons why your Paypal Plugin is not working. This guide lists most common reasons and solutions for them.

### 1. Order status Failed

Are you using your Primary Paypal Email as your merchant email? If your order status is failed, then chances are that you are using a secondary email of your Paypal account.

Paypal allows you to add multiple emails in an account to accept payments. With the Paypal plugin for J2Store, make sure you are using your primary Paypal account email. You can check which is your primary email by signing into your Paypal account and then going to Profile -> Add / Edit emails page.

![Paypal Primary Email](paypal_primary_email1.png)

### 2. Currency is wrong. Paypal payment screen shows USD while my currency is different

Paypal supports multiple currencies. However, it does not support all currencies of the world. Please ensure that your currency is supported by checking this page: https://www.paypal.com/multicurrency

If your currency is not supported, Paypal will automatically assume the currency as USD.

A workaround to this problem is : Allow customers to shop in your currency and convert it to USD when they are redirected to paypal for payment.

Here is a step by step guide to set up auto conversion of your currency to USD.

Let us assume, your store is located in India and your currency is INR. But Paypal does not support INR.

Here is how you can overcome the issue.

####Step 1: Enable Auto currency update
![currency_auto_update](Selection_048.png)
Go to Joomla admin - j2store - set up - > configuration -> Store tab
Set your Default Currency as INR
Set Auto update currency to YES

####Step 2: Create multiple currencies
Go to Joomla admin - j2store - set up - currencies

You might have already created the INR currency. Open it and make sure its value is set to 1

**Now, create a new currency**
![currency_creation](Selection_050.png)
Currency Name: USD
Currency Code: USD
Currency Symbol: $
Decimal places: 2
Decimal Separator: .
Thousands separator: ,
Value: 0.061 (You can enter any value less than 1. Once saved, J2Store will automatically contact Yahoo Financial services and update the correct exchange value )
Status: Published

Save now.
![currency_management](Selection_049.png)

You are all set now. Prices in your store will now display in INR. When the customer is redirected to paypal, he will be asked to pay in USD. 
J2Store will automatically do the currency conversion depending on the prevailing exchange rate.











