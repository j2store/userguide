# Australia Post Shipping Plugin

This plugin integrates J2Store with Australia Post Shipping rate API.

### Requirements
* **PHP 5.2 or higher**
* **Joomla 2.5 or above**
* **J2Store 2.7.3 or above**

### Installation
You can install this shipping plugin, using joomla installer.

1. In the J2Store admin, go to **Extensions -> Extension Manager**
2. Click on the *Browse* button and select **Australia Post Shipping** (type=j2store) and click on *Upload & Install*
3. Enable the plugin
4. Configure the shipping plugin by entering the plugin parameters

The installation procedure is illustrated in the image below:
![](./assets/images/aus-ship-plg-install.png)
![](./assets/images/aus-ship-doc-1.png)
![](./assets/images/aus-post-ship-method-list.png)

### Parameters

##### Shipping Type
For this option, select **Domestic Shipping Service** or **International Shipping Service**

Check the image below and set up the shipping parameters as illustrated in the image.
![](./assets/images/aus-post-ship-config.png)

##### API Key
This is your Australia post API key. It will be given to you once you create an Australia Post account.

##### Handling Cost
If a handling cost is applicable for the shipping, you can enter the cost directly in this field. 

##### Show Delivery Time
If you want to show the Date/Time of delivery in checkout page, you can set this option to **Yes**

##### Minimum Subtotal required
If a minium quantity is required to avail this shipping method, you can set it here.

##### Maximum Subtotal required
If there is a limit in the quantity to use this method, set it here.

##### Tax Profile
If the shipping cost is also taxable, you can select a tax profile here.

##### Geozone
If you have limitations in applying this shipping method, you can select the areas that are eligible, by selecting the corresponding geozone here. 

##### Weight Unit
For using this shipping method, the weight unit must always be set to ***Kilograms*** only. No other unit is allowed.

##### Length Unit
The length unit for this shipping method must be set to ***Centimetre***. No other unit for length measurement is entertained.

##### Debug
If you enable this option, a log file will be maintained for error debugging. This debug file will be stored in cache folder. 

>**IMPORTANT**: Apart from the parameters set here, to use **Australia Post Shipping Plugin**, it is mandatory to set the default currency as **Australian Dollar - AUD** and the country of the store as **Australia**, in the store configuration setup. If it is not met, this plugin can not be used.

### Support
If you still have questions, you can reach us in **support@j2store.org**

Thankyou for using our extension.

