# Quickbooks Online

This plugin integrates Quickbooks online, a business accounting software with J2Store Joomla eCommerce solution.

The app integrates only with the **QuickBooks Online edition**. If you have an offline edition, consider migrating to online and the migration is very smooth.

You should have following minimum requirements to use this app.

##### Minimum requirements

* PHP **OAuth** extension should be enabled. If you don't know what OAuth extension is, contact your hosting provider and ask them to enable it for you.

* Cron job should be enabled. Otherwise the app will not work.

* You must have atleast J2Store version **3.2.21** to use this app.

* The **CRON JOB** has to be created in order to perform the synchronization of orders and customers with Quickbooks properly.
    
    Here is the sample cron url:
    ```
    https://www.example.com/?option=com_j2store&view=queues&task=processQueue&queue_key=<queue key>&queue_type=app_quickbook
    ```
    Queue key could be found under J2Store > Setup > Configuration > Store tab
    
    Replace www.example.com with your domain.

### Installation

1. Download Quickbooks Online package from our site. You will get two .zip files named:

    a. Quickbooks Online OAuth 1 - plg_j2store_app_quickbook.zip
    b. Quickbooks online OAuth 2 - plg_j2store_app_quickbook_oauth2.zip
    
    If you see **client ID** and **Client secret** keys on your quickbooks account dashboard, you will have to install package b (plg_j2store_app_quickbook_oauth2.zip).
    
    If you see **Consumer ID** and **Consument Secret** keys on your quickbooks account dashboard, you will have to install package 2 (plg_j2store_app_quickbook.zip)
    
2. Install the downloaded package through Joomla installer.

3. After installing, go to J2Store > Apps and activate Quickbook Online.

4. Once enabled, open the app and configure the basic settings.

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

#### Where to find Company ID in sandbox ?

##### Step-1 Create a sandbox

Create a sandbox from your total allocation via the Manage Sandboxes page.

1. Once logged in to Intuit Developer, click either the Tools dropdown or the dropdown arrow next to your name from the menu on any page and choose Sandbox.
![](./assets/images/qb-sandbox-menu.png)

2. The Manage Sandboxes page displays. Next, select the country and the click Add from the Manage Sandboxes page.
![](./assets/images/qb-create-sandbox.png)

3. A US sandbox is provisioned automatically. You can have up to four additional sandboxes distributed as you like across the AU, CA, FR, IA, UK, and US development regions.

5. Select the country from the dropdown and click **Add** button.

5. Once a sandbox is created, you cannot change its country designation.

##### Step-2 Launch a quickbook sandbox and identify your company ID

1. Once logged in to Intuit Developer, select Sandbox from the  Docs & Tools landing page or from the dropdown arrow next to your name.
![](./assets/images/qb-sandbox-menu.png)

2. The Manage Sandboxes page displays. To open a QuickBooks Online sandbox, click **Go to company** for the desired sandbox.
![](./assets/images/qb-launch-sandbox.png)

3. It redirects you to the sandbox company home page where you can use ```ctrl+Alt+/``` from your keyboard to see your company ID.

4. The popup window will show your company ID.
![](./assets/images/qb-company-id.png)

#### Where to find App token, consumer key, consumer secret ?

1. Go to https://developer.intuit.com and Sign in to your Intuit Developer account.

2. After signing in, from the menu on any page, click My Apps.
![](./assets/images/qb-myapp-menu.png)

3. The resulted page displays you the list of app that you have created already. Find the app you want keys for and click on it. The app opens to the Development tab.

4. If you don't have any app, Click the Create new app button.
![](./assets/images/qb-create-apps.png)

5. Click the Select APIs button.
![](./assets/images/qb-select-api-btn.png)

6. Popup window will be dispayed. Select one or both of the QuickBooks Online APIs: Accounting and/or Payments and click **Create app** button.
![](./assets/images/qb-select-api.png)

7. Your new app opens to its Dashboard tab.

8. Click the **Keys** tab on either Developement tab or Producttion tab. 
 
 Development keys—use only in the sandbox environment.

 Production keys—use only in the production environment
 
 You see your token and keys listed. Copy them and paste it in our Quickbooks online app's configuration.
![](./assets/images/qb-dev-keys.png)

#### Settings

**Sandbox/Test Mode**

Quickbooks offers sandbox feature for testing purpose. If you would like to use Sandbox account to test, set this option to **YES**.

**Change Payment status Paid ?**

If you want to change payment status to **PAID**, set this option to **YES**. If you are accepting credit card payments, the app could mark the invoices as paid immediately after they were created.

**Syncronize Order total is zero ? **

Our quickbooks allows to auto synchronize your zero price order with Quickbooks online. Choose **YES**, if you want to synchronize order total zero.

**Syncronize order status list**

Orders with status selected here are synchronized to Quickbook. For example, choose **Confirmed**. So the app will synchronize the order whose order has status confirmed.

**Debug**

Choose YES to enable debug mode. It will generate the log file in cache folder of joomla root. (./cache)
> Don't enable DEBUG mode in live site.
![](./assets/images/qb-settings.png)

#### Production

You will have fill all the required fields below to connect to your Quickbook production account.

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
![](./assets/images/qb-production.png)

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
![](./assets/images/qb-sandbox.png)

#### Synchronize

**Customer Syncronization**

Click on button named "Customer" to synchronize J2Store customer to Quickbook customer.

**Invoice synchronization**

Click on button named "Invoice" to synchronize J2Store invoice to Quickbook.