# Partial Payment

This app facilitates users to buy products and pay on installments or partial payments.

## Installation

* This app can be downloaded from our site and installed using the default joomla installer.

* Once installed, the app can be configured under J2store-Apps.

* Click Enable to enable the app.
* Click Open to Open and configure the settings for the app.

## Setting up plans/installments for partial payments:

* Click on the Plans tab (Refer the screenshot attached).

* Click on the New button to create a new plan.

* Give the plan a name,description and set up a plan schedule(the installments the payment is to be paid within).

* Click Save.

* Click Back to Apps to set up partial payments.

**Relevant Screenshot**

![](./assets/images/app_partialpaymentplan.png)


## Configuration

### Basic Settings


* ** Enable partial payment**

     Three options are available as follows:

    * **No**-Disable the partial payment mode.

    * **Yes-optional partial payment**-This allows partial payment mode as an option against normal full payment method.

  * **Yes-required partial payment**-This makes partial payment as the only option.


* **Select by default**

   Choose if the default payment mode is partial or full.

* **Partial payment type**

  Select if you wish to set up a fixed amount as the default amount to be paid or a plan or a % of the total amount.

* **Amount/Plan**

    * This option depends on the value chosen on the previous parameter.

    *  If you wish to collect a % of the total amount or a fixed amount the amount has to be specified here.

    * If plan is chosen as the partial payment mode,the plan that has been created should be selected here.

* **Order Status**

 Scheduled order status for the future payments must be specified here.

* **Cron URL**
 The Cron URL should be mentioned here.

**Relevant Screenshot**


  ![](./assets/images/app_partialpaymentbasicsettings.png)


### Mail Settings

* **Send email on enable pay**

  Choose Yes to send emails to the users when the payment due date approaches.

* **Notify payment pending on**

 Send reminder mails to customers through the days specified here after the payment date.

* Click Save.

**Relevant Screenshot**

 ![](./assets/images/app_partialpaymentmailsettings.png)
