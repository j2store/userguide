# Shipstation

The new J2Store integration with Shipstation helps you to integrate your J2Store site with one of the best shipping solution, Shipstation. Now import your orders and manage shipping on the go with the help of this integration. With Shipstation, you need not worry about shipping your orders using different carriers, cause you can manage everything at a one stop place using this integration.

Shipstation is a multi-channel, multi-carrier shipping solution that simplifies the shipping process for online merchants. Shipstation can be integrated seamlessly with any shipping carrier and channel and your orders can be easily tracked and managed with just few clicks, regardless of the location.

Now conduct your business with more fluidity and transparency with the easy interfacing of shipstation.

>Note: Specifying the tracking id manually in the Shipstation settings and setting up notifications for Order shipped won't work because if the notifications are set up this way, the tracking numbers will not be synchronized with J2Store.

## Installation

The integration can be downloaded from our site and installed using the default joomla installer.

## Pre-requisites

A shipstation account is required to use the integration.You could create one at www.shipstation.com

<a name="apikeys"></a>
## Creating an account and generating API keys

To get the API keys for the integration, it is necessary to create an account with Shipstation.Following are  the steps to be done:

* Go to www.shipstation.com.

* Click on the Start your 30 day free trial button.

* A page appears asking you to create a new account. Furnish your details and click on the Lets go to shipping button.

* Before logging into your account, it is necessary to verify the email address by clicking on the link sent to your registered email address.

* Post verification, you can login to the account by clicking on the login button on the top right corner and keying in the credentials.

*  Click on the **settings** icon on  the right corner.

* There will be lot of tabs displayed on the left side. Click on the **Account** tab.

* Clicking on the Account tab will open up the options from which the **API settings** option has to be chosen.

* Click on the **Generate API keys** button. API keys will be generated.

The below screenshots are for reference:

**Creating an account with Shipstation**

![](./assets/images/shipstationaccountcreation.png)

**Generating API keys**

![](./assets/images/shipstationapikeys.png)


![](./assets/images/shipstationapikeys1.png)


![](./assets/images/shipstationapikeys2.png)


![](./assets/images/shipstationapikeys3.png)

## Webhook URL

After entering the API keys in the app, the next step would be to set up the webhook URL in the Shipstation account.

This has to be done in order to receive notifications of the changes that occur in shipstation. The notifications will come up in your J2Store site's backend.So this is more of a synchronization.

## Setting up webhook notifications

Webhook notifications can be set up by following the steps given below:

* The URL for webhook can be fetched from the app's settings.

 ![](./assets/images/shipstationwebhookurl.png)

* Now login to your Shipstation account.

* Go to Settings->Integrations->Integration partner->Webhook.

* Specify the URL in the field Webhook URL and save.

![](./assets/images/shipstationwebhookurlspec.png)

## App settings

The following are the parameters that have to be filled for the integration to  work:

* **API key**

   The shipstation API key has to be specified here. The procedure to generate the API keys has been mentioned **[here](#apikeys)**

* ** API Secret**

  The shipstation secret key has to be mentioned here.

* **Webhook URL**

    The webhook URL to be specified in the shipstation account's integrations part is provided here.

* ** Allowed Order status **

   The orders with the chosen status will be synchronized with Shipstation.
   For example if the status is chosen as Confirmed here, then all the orders whose status is confirmed will be synchronized with Shipstation.

* **Debug**

   This option has to be set to Yes if the activity of shipstation has to be logged.

   ![](./assets/images/shipstationappsettings.png)
