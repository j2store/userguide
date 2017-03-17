# Subscriptions and Memberships

If you would like to sell subscription-based products, you could do just that with our Subscriptions and Membership app. This app allows you to sell products and services with recurring payments.The following features are possible with Subscription Products app :

##### Features

**1. Billing schedules**

Create any type of billing schedules. You can have memberships for days, weeks, months and years. Example: 3 months, 6 months, 1 year

**2. Automatic renewals and payments**

It is very convenient for the customers to have their membership auto-renewed with automatic payments (Current supported in 3 payment gates : PayPal, Stripe, Mollie. More gateway support is coming up)

**3. Sign up Fees**

You can now collect one-time sign -up fees or set -up fees along with the subscription. If it is a recurring subscription, the customer will only billing for the membership plan cost in the next billing automatically.

**4. Variable subscription**

Allow your customers to choose a membership plan that suits their needs. So you can create one subscription product with multiple variants.

**5. Expiry management**

The app automatically manages the expiration of the membership. You can set the system to notify the customers before the expiry of their subscription.

**6. Subscriptions management**

Manage all the subscriptions in one place. You can cancel the subscription, view the relavant orders and more

**7. Multiple subscriptions**

Customers can purchase any number of subscriptions in the same order / transaction.

**8. Notification emails**

Send automatic emails to the customers when the subscription is created, when a renewal payment is processed or when a subscription is cancelled or expired. You can customise the email messages as well using language overrides.

##### Supported Payment Gateways

1. Paypal Standard for J2Store (Available on request)

2. Stripe (Available on request)

3. Mollie payment plugin

##### Known limitations

1. Subscription Products app does not support for guest checkout.

2. Variable subscription product type allows you to add only one option with multiple values.


### Requirements

1. PHP 5.4+

2. J2Store 3.2.20 or above

3. Joomla 3.4.x or above

### Installation

1. Download Subscription and Memberships package from our site and install it using Joomla installer.

2. After installing the app, go to J2Store > Apps and enable Subscription Products app.

3. Once enabled, open the app and configure the basic settings of the app.

### Basic configuration

There is nothing complex to configure this app. Open the app and navigate to **Expiry Control** tab.

**Notify expire day before**

Enter the number of days to send the remember mail to customer for notifying that their subscription will be going to end. For example, 2. So the mail will be sent before 2nd day to expire.

**Run expiry control for every**

Choose when the expiry control should run whenever the page loads. For example, choose 12 hours. So the expiry control will be running for every 12 hours whenever the page loads. This is applicable for cron.

**Cron key**

Enter the Cron key here to run cron.

Once finished configuring expiry control settings, just go to Article manager and create a new article.

### How to create subscription based products ?

Susbcription Products app allows you to create two types of subscription product.

1. Simple subscription

2. Variable subscription

Following are the step by step instructions to create subscription products.

- **[Creating simple subscription product](#simple-subscription)**
- **[Creating variable subscription product](#variable-subscription)**
- **[Pricing](#pricing)**
- **[Frontend Demo](#demo)**

<a name="simple-subscription"/>
#### Creating simple subscription product

1. Go to Article Manager > create new article > Move to J2Store cart tab

2. Choose **YES** to Treat as a Product and select **Simple Subscription** as Product Type and click **Save and Continue**.

![](./assets/images/subscription-simple.png)

1. Set **YES** to Visible in storefront and navigate to **Pricing** tab.

2. Pricing tab, where you could set your subscription product's price, customer group, expiry date, etc.

You can set images, shipping, filters to your subscription product.

<a name="variable-subscription"/>
#### Creating variable subscription product

The variable subscription product allows you to add only one option with multiple values.

For example, create premium subscription providing customers an option to choose subscription period.

Go to J2Store > Catalog > Options and create a option "Subscription period" and add the option values such as 3 months, 6 months.

![](./assets/images/subscription-option.png)

1. Go to Article Manager > create new article > Move to J2Store cart tab

2. Choose **YES** to Treat as a Product and select **Variable Subscription** as Product Type and click **Save and Continue**.

3. Set **YES** to Visible in storefront and navigate to **Variants** tab.

4. In variants tab, search and add Subscription period option and set values.
> It allows you to add one option with multiple variants. For example, Subscription period as option with following variants 3 months, 6 months, etc. See the screen shot below

![](./assets/images/subscription-variants.png)

5. Generate variants and set price, subscription time period, images, shipping, filters for each variants.

<a name="pricing"/>
#### Pricing

- **Subscription price :** Enter the price (for example, $29) of your subscription product and choose the duration/recurring period. For example, if your subscription product's duration period is 3 months, then choose **every 3rd month**.

- **Subscription length :** This will be listed based on the time period you selected. Choose 3 months. So the subscription will end at the  end of 3rd month.

  If you would like to give a life time price for your subscription product (i.e.) wants to collect $29 at the end of every 3 months for lifetime, choose **Never Expire** to Subscription length. So $29 for every 3rd month for lifetime.

- **Add / Remove user groups :** Users will be added and removed from the Joomla user groups when their subscription to the level is enabled or disabled.

- **Sign-up fee :** This app allows you to collect one time set up fee or sign up fee from your customers. Enter your sign up fee here. For example, $5 or $10.

- **Set Advanced Pricing :** If you want advanced pricing, click the 'Set Prices' button and it will open up a pop-up window to allow you to set an advanced price setting.

![](./assets/images/subscription-pricing.png)

<a name="demo"/>
#### Frontend Demo

![](./assets/images/subscription-frontend.png)

![](./assets/images/subscription-cart.png)

![](./assets/images/subscription-payment-checkout.png)

![](./assets/images/subscription-frontend-profile.png)

### Check the subscription details and status from backend

Go to J2Store > Apps and Open Subscription Products app and you can see subscription button on top of the page. Click on this button to view the customer's subscription details and status.

![](./assets/images/subscription-button.png)

![](./assets/images/subscription-detail.png)
