# Payflow PRO Payment Plugin

This plugin integrates the Payflow PRO gateway with J2Store. Accepted cards include Visa, MasterCard, Switch/Maestro, and Solo credit cards in the United States.

Payflow PRO is available only for merchants in US, Canada, Australia, New Zealand.

#### Requirements
* PHP 5.3 or higher
* Joomla 2.5.x
* J2Store 2.6.3

#### Installation Instructions
Use the Joomla installer to install the plugin like you do for other extensions.

#### Configuring the Plugin
Go to Joomla admin → Extensions → Plugin Manager → Paypal Payflow PRO.

**Payment option title**

The value entered here will be used as the title for this payment method. Customer will see this value when he checks out. Default: Payflow PRO

**Vendor/Merchant Login**

The Merchant Login with which you login to Paypal Manager

**User**

Your User ID. If you created a new user, then enter that user id here. If not, then this field should carry the same value as the Vendor/Merchant Login.

**Password**

Your password with which you login to Paypal manager

**Partner**
Your PayPal partner ID. By default, it will be PayPal.

**Transaction Type**

The type of transaction. If you choose SALE, then the payment will be captured immediately after a customer makes the payment. If you choose Authorization, then Payment will not be captured. You will have to capture it manually by going to Paypal Manager. Default value: Sale

**Use sandbox for testing**

Set this to YES, only if your account is in TEST mode. 

>IN LIVE SITE, THIS SHOULD BE SET TO NO.




















