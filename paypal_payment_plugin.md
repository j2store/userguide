# Paypal Payment Plugin

The plugin integrates PayPal Website Payment Standard method with your J2Store shopping cart. You need either a PayPal account in order to take payments

>Are you looking to troubleshoot your PayPal integration? We have answered most of the common problems. So read carefully

* [Requirements](#requirements)
* [Installation Instructions](#installation)
* [Parameters](#parameters)
* [Enabling IPN notification](#enable-ipn)
   * [Still having problems receiving IPN or intermittently not receiving the IPN?](#still-ipn-problems)
* [Troubleshooting Paypal Related Issues](#troubleshooting)
	* [Orders not confirmed. Status shows as incomplete or new](#orders_not_confirmed)
	* [Order status Failed](#order_status_failed)
	* [Currency is wrong. Paypal payment screen shows USD while my currency is different](#currency_is_wrong)
	* [Paypal duplicate invoice ID and how to solve it ](#paypal_duplicate)
		* [Solution 1: Set the Invoice Prefix](#invoice_prefix)
		* [Solution 2: Change settings in Paypal](#change_settings)
    * [Things don't appear to be working at the moment. Please try again later](#things-don't-appear-to-be-working-at-the-moment)
    * [Admin tools PRO exception](#admin-tools-pro)
    * [[Why]The payment HTML form not works](#payment-form-not-works)

## Introduction
Paypal standard plugin for J2Store allows you to accept payments via Paypal Payment Gateway. This uses the Paypal's Website Standard Payment. Customer will be redirected to Paypal to make payment securely 

<a name="requirements"></a>
## Requirements 
* PHP 5.2 or higher 
* Joomla 2.5.x 
* J2Store 2.0 or above 
<a name="installation"></a>

## Installation Instructions 
1. Use the Joomla installer to install the plugin. 
2. In the backend, go to Extensions->Plugin Manager and open the Paypal Payments 
plugin. (type=**j2store**). 
3. Enable the plugin 
4. Enter the parameters (read the explanation about each parameter given below) 
5. Save and close it. 

Now you can see the Paypal Payments as an option during the Check out process. 
<a name="parameters"></a>

## Parameters 
**Paypal Merchant Email Address**

This is your original paypal email/merchant email address, which you have used in Paypal. 

**API Username**

Enter the API username associated with your PayPal live account.

**API Password**

Enter the API password associated with your PayPal live account.

**API Signature**

Enter the API signature associated with your PayPal live account.

> Not sure where to find your API signature? Read the documentation below
https://developer.paypal.com/docs/classic/api/apiCredentials/#create-an-api-signature

**Choose the callback url to be used for IPN notifications**

The URL selected here will be set as dynamic IPN url instead of the URL which you have configured in your PayPal account.

 * **Default url :** The default url is the normal query string url used for IPN Notifications. This will work for 99% of the users. If it does not work in some cases, you could try any one of the following alternative urls.
   ```
   http(s)://www.example.com/index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=payment_paypal&paction=process
   ```

 * **Alternative - 1 :** It is the alternative callback url that uses the callback view.
   ```
   http(s)://www.example.com/index.php?option=com_j2store&view=callback&method=payment_paypal&paction=process
   ```

 * **Alternative - 2 :** It is the **Proxy** of default url. Sometimes, the PayPal IPN server truncates the query strings. It happens very rarely and you can check the IPN history in your PayPal account to see if PayPal is truncating. Login to your PayPal account and then go to:  to view the IPN history.  If it does truncates the query strings, you can use this url
   ```
   http(s)://www.example.com/plugins/j2store/payment_paypal/payment_paypal/tmpl/notify.php
   ```
> If you are using any **firewall** like **Admin Tools PRO**, you might have to add exception to IPN url you have selected to use. **PayPal does a server-to-server remote post. Most firewalls will block remote post requests.**

**Surcharge Percentage**

You can collect a percent of the total order value as surcharge / fee for using the Paypal option from your customers using this option.  You can enter a value here (for example: 2 ).  If you enter 2 here, then 2 % of the total order value will be added as a handling cost to the order.

This is optional parameter.

>NOTE: DO NOT enter any symbol like % here.

Leave empty if you dont want to charge.

**Surcharge Fixed**:

You can collect a  fixed surcharge / fee for using the Paypal option from your customers in addition to the order value.  You can enter a value here (for example: 2 ).  If you enter 2 here, then 2 will be added as a handling cost to the order.

Leave empty if you dont want to charge.

This is an optional parameter.

**Use SSL to post back to Paypal?**

If you are using SSL certificate (https), enable this with a **Yes**. If you dont know what SSL is, better leave it as **No** 

**Use Paypal Sandbox**

Paypal offers a testing suite called Sandbox. Before going live, you can test your store using the Paypal's sandbox feature. Read more about Paypal Sandbox at developer.paypal.com.

>IN LIVE SITE, THIS SHOULD BE SET TO NO. 

**Paypal Sandbox Merchant Email**

Your paypal sandbox email. 

**Sandbox API Username**

Enter API username associated with your PayPal sandbox account.

**Sandbox API Password**

Enter API password associated with your PayPal sandbox account.

**Sandbox API Signature**

Enter API signature associated with your PayPal sandbox account.

**Article ID for Thanks you message**

You can create an article to say thanks, provide some information or instructions to the customers, who purchased in your online store. Enter the Article ID here. This will show, 
when customers return from the paypal. 

**Geozone**

By selecting a geozone here, you can restrict this payment method to only customers of that geo-region. Choose All geozones to show this method to all customers.

**PayPal Callback Text**

What the button on the PayPal site reads after the user has completed his transaction. Leave empty for the default 'Return to the merchant website' text. 

This is an optional parameter.

** Custom Header Image **

The URL to your logo so. This image will be displayed on the top of PayPal's checkout page instead of your merchant name. 

>WARNING! It must be an HTTPS URL, otherwise your clients will 
receive warnings about insecure content. 

This is an optional parameter.

**Header Background Colour**

The hex-code of your PayPal checkout page's header, e.g. FFFFFF for white (note: place no # in front the hex value) 

This is an optional setting.

**Header Background Colour**

The hex-code of your PayPal checkout page's header, e.g. FFFFFF for white (note: place no # in front the hex value) 

This is an optional setting.

**Header Border Color** 

The hex-code of your PayPal checkout page's header border, e.g. FFFFFF for white (note: place no # in front the hex value) 

This is an optional setting.

**Logo Image for display in Paypal**

The URL of the 150x50-pixel image displayed as your logo in the upper left corner of PayPal’s pages. Default: your business name (if you have a Business account) or your email address (if you have Premier account). If this is not working, try using the Custom Header Image param above. 

This is an optional setting.

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

<a name="enable-ipn"></a>
## How to enable IPN Notification in your PayPal account.

Login to your Paypal account

Click Profile on the My Account tab.

Click Instant Payment Notification Preferences in the Selling Preferences column.

Click Choose IPN Settings to specify your listener's URL and activate the listener.

In the Listener's url enter the following url

```php
http://<YOUR_DOMAIN>/index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=payment_paypal&paction=process&tmpl=component
```
If you access your website using an httpS protocol (SSL certified), you may want to use  below url

```php
https://<YOUR_DOMAIN>/index.php?option=com_j2store&view=checkout&task=confirmPayment&orderpayment_type=payment_paypal&paction=process&tmpl=component
```
 >> Do not copy paste the above urls. You need to change your domain name and the http protocol

<a name="still-ipn-problems"></a>
### Still having problems receiving IPN or intermittently not receiving the IPN?

Since J2Store 3.2.21, we have introduced a fail-safe method to collate PayPal Transactions. There could be a hundreds of reasons why PayPal did not sent the IPN or why your site did not receive the IPN.

The listener in the plugin is always active and ready to listen. If Paypal sends IPN, it will listen and process. That is it's job.

Since there could be many reasons why IPN has not reached or sent, we included a collation method as a fail-safe since J2Store 3.2.21
So even if the IPN did not arrive, the plugin can now query the PayPal server and collate the transactions (triggered via a cron job)
>NOTE: It is purely optional to implement this fail-safe mechanism. This is not a necessary step. If you are too anxious and doubt that your site is not receiving the IPN, you can implement this. 

##### How do I implement this fail-safe method ?

 In the event of IPN not reaching your site, you can make sure that the transactions at your site and PayPal could be collated using a cron job
 
- Make sure you have J2Store 3.2.21
- Login to your hosting cPanel and set up a cron job
- The cron job command should be: (You can set this to run at 15 minutes intervals)
 
**Non-ssl**
```curl 
 wget -O /dev/null "http://<YOUR_DOMAIN_NAME>/index.php?option=com_j2store&view=cron&command=paypalcollation&cron_secret=XXXXX" > /dev/null
 ```
 
** SSL ** 
```curl 
 wget --no-check-certificate -O /dev/null "https://<YOUR_DOMAIN_NAME>/index.php?option=com_j2store&view=cron&command=paypalcollation&cron_secret=XXXXXX" > /dev/null
```
 
>**NOTE:** Replace <YOUR_DOMAIN_NAME> with your domain name   
> Replace XXXXXX with your cron secret key, which you can find at Joomla Administration -> J2Store -> Set up -> Configuration -> Store

<a name="troubleshooting"></a>
## Troubleshooting Paypal Related Issues

There could be many reasons why your Paypal Plugin is not working. This guide lists most common reasons and solutions for them.
<a name="orders_not_confirmed"></a>
### 1. Orders not confirmed. Status shows as incomplete or new

It means you are not getting the Instant Payment Notification (IPN) from Paypal.

The IPN may not reach your site, if :

1. The Site is offline
2. The Site is in local server / local host / live in your local machine
3. You have created a menu for the Checkout and set its access level to Registered or Special or Something other than public. 
4. You have a firewall installed either in your site or by your host
5. You have disabled IPN in your Paypal account. 

#### Solutions to above issues :

1. Go to Joomla admin - Global configuration. Set **Site Offline** to No
2. Host your site
3. Set the Checkout menu access level to Public
4. If you have a firewall like Admin Tools, then you can add Exceptions. Please consult with your firewall provider or with your host.
    ``` 
        If you are using the Admin Tools PRO version, you will have to exclude the [IPN urls mentioned above](#enable-ipn)
        
        If your site or your hosting server has a firewall (you can check with your host), then you may have to whitelist the Paypal's server IPs
        
        Here you can get a list of IPs used by the Paypal servers
        https://ppmts.custhelp.com/app/answers/detail/a_id/92
        
        Paypal makes a remote post (IPN) to your site when a payment is made to inform us that payment has been made and you can mark the order complete. Firewalls normally block remote posts. So we may have to whitelist the IPs allowing them to do the remote post.
    ```

5. See the [IPN topic above](#enable-ipn) 

<a name="order_status_failed"></a>
### 2. Order status Failed

**Solution - 1**

Are you using your Primary Paypal Email as your merchant email? If your order status says failed, then chances are that you are using a secondary email of your Paypal account.

Paypal allows you to add multiple emails in an account to accept payments. With the Paypal plugin for J2Store, make sure you are using your primary Paypal account email. You can check which is your primary email by signing into your Paypal account and then going to Profile -> Add / Edit emails page.

![Paypal Primary Email](./assets/images/paypal_primary_email1.png)

**Solution-2**

Go to Global configuration -> Server tab -> Database setting
Are you using the MySQL PDO driver ?

If yes, please take a backup of the site and choose the MySQLi driver.

The PDO driver of Joomla has a bug. Instead of returning a boolean value on table update as mandated by the interface, it would return a record set, causing issues.

<a name="currency_is_wrong"></a>
## 3. Currency is wrong. Paypal payment screen shows USD while my currency is different

Paypal supports multiple currencies. However, it does not support all currencies of the world. Please ensure that your currency is supported by checking this page: https://www.paypal.com/multicurrency

If your currency is not supported, Paypal will automatically assume the currency as USD.

A workaround to this problem : Allow customers to shop in your currency and convert it to USD when they are redirected to paypal for payment.

Here is a step by step guide to set up auto conversion of your currency to USD.

Let us assume, your store is located in India and your currency is INR. But Paypal does not support INR.

Here is how you can overcome the issue.

####Step 1: Enable Auto currency update
![currency_auto_update](./assets/images/Selection_048.png)
Go to Joomla admin - j2store - set up - > configuration -> Store tab
Set your Default Currency as INR
Set Auto update currency to YES

####Step 2: Create multiple currencies
Go to Joomla admin - j2store - set up - currencies

You might have already created the INR currency. Open it and make sure its value is set to 1
        
**Now, create a new currency**     


![currency_creation](./assets/images/Selection_050.png)   

- Currency Name: USD   
- Currency Code: USD
- Currency Symbol: $
- Decimal places: 2
- Decimal Separator: .
- Thousands separator: ,
- Value: 0.061 (You can enter any value less than 1. Once saved, J2Store will automatically contact Yahoo Financial services and update the correct exchange value )
- Status: Published

Save now.   

![currency_management](./assets/images/Selection_049.png)    


You are all set now. Prices in your store will now display in INR. When the customer is redirected to paypal, he will be asked to pay in USD. 
J2Store will automatically do the currency conversion depending on the prevailing exchange rate.
<a name="paypal_duplicate"></a>

## 4. Paypal duplicate invoice ID and how to solve it
Paypal by default does not allow duplicate invoices. When you try to pay for a duplicate invoice id, Paypal will produce the following error:

>**The transaction was refused as a result of a duplicate invoice ID supplied. Attempt with a new invoice ID**

If this were to happen, one of the reasons could be that the configuration in Paypal is set to not accept duplicate invoices. You may receive orders from various places and if the invoice numbers are the same, Paypal recognises there is an invoice duplication.

There are two ways, by which you can fix this.
<a name="invoice_prefix"></a>

#### Solution 1: Set the Invoice Prefix

Please follow the steps:

1. From your J2Store Dashboard, go to - Set Up -> Configuration -> Order

>Note: This step is for V3. If you are using v2, then go to Set Up -> Store Profiles -> your store profile

2. Set the Invoice Prefix in the textbox provided, for e.g., INV-2015- or INV/2015/

3. Save & Close.

<a name="change_settings"></a>

#### Solution 2: Change settings in Paypal

Please try the following:

1. Log-in to your Paypal account
2. Click Profile
3. Under Selling Preferences, click Payment Receiving Preferences
4. Under Block Accidental Payments choose "No, allow multiple payments per invoice ID".
5. Save.

<a name="things-don't-appear-to-be-working-at-the-moment"></a>
## Things don't appear to be working at the moment. Please try again later

Paypal has recently rolled out their cool " New Checkout! "

With this Paypal also seems to impose certain new technical restrictions  

- Specified Character length for address fields, Product name and Product options. Length varies based on fields and is specified on their integration guide.
- Number of product options sent to paypal are limited to 7 options.

This could be due to the recent technical restrictions imposed by paypal: (refer below image)  

![paypal-technical-restriction](./assets/images/paypal-docs-arrtibutes-restriction.png)

#### How to fix it ?

We have updated the paypal plugin with fixes for these new technical restrictions. Please make sure you update your paypal plugin to latest (v.3.4)
With this update if you have used more than 7 options then the first 7 options are passed to paypal and others are ignored. Similarly if the product option character length is larger than allowed by paypal, those values are trimmed (cut off). This will make sure you do not get any errors and customers will continue to see checkout screen without any issues.

**NOTE:** Please take a backup before updating the plugin and test after installing.

### Here is another possible reason (this might also cause this error)

You might have enabled the Encrypted Website Payments. Try the following steps to solve this.

1. Log in to your PayPal account.
2. Click Profile.
3. From the Selling Preferences column, click Website Payment Preferences.
4. In the Encrypted Website Payments section, select Off.
5. Click Save.

Also check if your PayPal account is approved to receive payments.

<a name="admin-tools-pro"></a>
## Admin tools PRO exception

All firewalls including the Admin Tools PRO would normally block any server-to-server remote POST requests. PayPal sends the IPN callback notification as a remote POST request immediately after the customer makes the payment.

In order to allow this request to pass through your firewall, you need to add an exception

Here is a screenshot of the WAF Exception in Admin Tools PRO
![](./assets/images/admin-tool-pro-exception.png)

## Why the paypal payment form not works ?

It seems due to the param "Block non-encrypted Website Payments" has been enabled inside your paypal account settings.

Disabling this param will solve this problem.

**Block non-encrypted Website Payments** = disable