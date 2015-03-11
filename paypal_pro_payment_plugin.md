# Paypal PRO Payment Plugin

This plugin integrates with Paypal Pro Payments using the Direct API.

#### Installation
You can use the standard Joomla installer for installing the plugin. Go to Extensions and choose the plugin package to install.

#### Configuration
Go to Joomla Administraton->Extensions->Plugin Manager Open the Paypal Pro plugin.

>TIP: Set the type filter to J2Store to quickly get to the plugin

##### Payment Option Title
Enter a title for this payment option. Customers can see this title while selecting the payment.

##### API User Name
The API username provided by Paypal. You can get this under the options in Profile settings.

##### API Password
The API password provided by Paypal. You can get this under the options in Profile settings.

##### API Signature
The unique signature provided by Paypal. You can get this under the options in Profile settings.

##### Card Types
Select the allowed card types for your store. Paypal has some regional differences. In USA< it accepts all card types, while in Canada only Visa and Mastercard are accepted. Check the regional differences here: https://developer.paypal.com/docs/classic/paypal-payments-pro/integration-guide/WPWebsitePaymentsPro/#id25a6cc16-bbc4-4070-a575-9fad358f2b95

##### Payment Action
Set the type of payment you wanted to take. The default and RECOMMENDED setting is **Sale**. This will enable you to get the payment instantly credited to your account.

**Authorisation**: An authorization payment action represents an agreement to pay and places the buyer’s funds on hold for up to three days. Choose this payment action if you need to ship the goods before capturing the payment or if there is some reason not to accept the payment immediately. After shipping, you have to login to your Paypal account and manually capture the payment.

##### Use Paypal Sandbox
Set this to yes if you want to test the integration with a Paypal Sandbox account. To create a sandbox account you need to sign up for it at http://developer.paypal.com

##### Geozone
By selecting a geozone here, you can restrict this payment method from showing to customers from only that geo-region. Choose All geozones to show this method to all customers




