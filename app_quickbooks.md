# Quickbooks Online

This plugin integrates Quickbooks online, a business accounting software with J2Store Joomla eCommerce solution.

The app integrates only with the **QuickBooks Online edition**. If you have an offline edition, consider migrating to online and the migration is very smooth.

You should have following minimum requirements to use this app.

##### Minimum requirements

* PHP **OAuth** extension should be enabled. If you don't know what OAuth extension is, contact your hosting provider and ask them to enable it for you.

* Cron job should be enabled. Otherwise the app will not work.

* You must have atleast J2Store version **3.2.21** to use this app.

##### Key features

**Orders**

As soon as an order is placed in your online store, it will be synchronized with your QuickBooks account.
You do not need to manually create any records in your accounting page. The order data including the itemized data will be sent to quickbooks.

**Customers**

The the customer data including their address and email will be synchronized with your quickbooks account. The app checks for duplicates before attempting to create the customers.

**Existing order and customer data**

Do you already have hundreds of orders and customers in your online store. No worries. The app has a synchronize option to send the existing order and customer data.

**Mark transactions as paid**

If you are accepting credit card payments, you would probably want to mark the invoices as paid immediately after they were created.
The app could do that automatically for you. You can choose an income account to create the payment-received transactions.

**Queues**

The transactions are queued before being sent to quickbooks. So there is no performance overload or delays when customers make orders. Even if the communication between quickbooks and your online store is interrupted, the transaction will be re-queued. You can also manage the transaction records in queue.

#### Installation

1. Download Quickbook from our site and install it using Joomla installer.

2. After installing the app, go to J2Store > Apps and enable the Quickbook for J2Store.

3. Once enabled, click on Open to configure the Quickbook app settings and to add the credentials keys.

#### How to launch a quickbook sandbox ?

1. Once logged in to Intuit Developer, select Sandbox from the  Docs & Tools landing page or from the dropdown arrow next to your name. 

2. The Manage Sandboxes page displays. To open a QuickBooks Online sandbox, click Go to company for the desired sandbox. Sign in with your developer credentials.

#### How to create a sandbox ?

Create a sandbox from your total allocation via the Manage Sandboxes page.

1. Once logged in to Intuit Developer, click either the Tools dropdown or the dropdown arrow next to your name from the menu on any page and choose Sandbox. 

2. The Manage Sandboxes page displays. Next, select the country and the click Add from the Manage Sandboxes page.

3. A US sandbox is provisioned automatically. You can have up to four additional sandboxes distributed as you like across the AU, CA, FR, IA, UK, and US development regions.

4. Once a sandbox is created, you cannot change its country designation.

5. A sandbox cannot be deleted. Once your allocation is exhausted, the Add button is disabled.

#### Where to find App token, consumer key, consumer secret ?

1. Sign in to your Intuit Developer account.

2. From the menu on any page, click My Apps.

3. Find the app you want keys for and click it. The app opens to the Development tab.

4. If you don't have any app, Click the Create new app button.

5. Click the Select APIs button.

6. Select APIs.

7. select one or both of the QuickBooks Online APIs: Accounting and/or Payments.

8. Your new app opens to its Dashboard tab.

9. Click the **Keys** tab. You see your token and keys listed.

#### Settings

**Sandbox/Test Mode**

Quickbooks offers sandbox feature for testing purpose. If you would like to use Sandbox account to test, set this option to **YES**.

**Change Payment status Paid ?**

If you want to change payment status to **PAID**, set this option to **YES**. If you are accepting credit card payments, the app could mark the invoices as paid immediately after they were created.

**Syncronize Order total is zero ? **

Choose **YES**, if you want to synchronize order total zero.

**Syncronize order status list**

Orders with status selected here are synchronized to Quickbook. For example, choose **Confirmed**. So the app will synchronize the order whose order has status confirmed.

**Debug**

Choose YES to enable debug mode. It will generate the log file in cache folder of joomla root. (./cache)
> Don't enable DEBUG mode in live site.

#### Production

**Company/RealmId :**

Enter company ID associated with your Quickbook's live account.

> The below details can be obtained from My Apps section in https://developer.intuit.com

**Consumer Key :**

Enter consumer key associated with your Quickbook's live account.

**Consumer Secret :**

Enter consumer secret key associated with your Quickbook's live account.

**Access Token :**

Enter Access token associated with your Quickbook's live account.

**Access Token Secret :**

Enter access token secret key associated with your Quickbook's live account.

**Quickbook production connection :** After entering all the required data such as company id, consumer key, consumer secret, Access Token, click on **connect to QuickBooks** to connect Quickbook production app.

#### Sandbox

**Sandbox Company/RealmId :**

Enter company ID associated with your Quickbook's sandbox account.

> The below details can be obtained from My Apps section in https://developer.intuit.com

**Sandbox Consumer Key :**

Enter consumer key associated with your Quickbook's sandbox account.

**Sandbox Consumer Secret :**

Enter consumer secret key associated with your Quickbook's sandbox account.

**Sandbox Access Token :**

Enter Access token associated with your Quickbook's sandbox account.

**Sandbox Access Token Secret :**

Enter access token secret key associated with your Quickbook's **live** account.

**Quickbook sandbox connection :** After entering all the required data such as company id, consumer key, consumer secret, Access Token, click on **connect to QuickBooks** to connect Quickbook sandbox app.

#### Synchronize

**Customer Syncronization**

Click on button named "Customer" to synchronize J2Store customer to Quickbook customer.

**Invoice synchronization**

Click on button named "Invoice" to synchronize J2Store invoice to Quickbook.