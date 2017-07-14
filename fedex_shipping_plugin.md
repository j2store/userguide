# FedEx Shipping Plugin

This plugin integrates J2Store with FedEx Shipping rate API.

### Requirements
* **PHP 5.2 or higher**
* **Joomla 2.5 or above**
* **J2Store 2.7.3 or above**

### Installation
You can install this shipping plugin, using joomla installer.

1. In the J2Store admin, go to **Extensions -> Extension Manager**
2. Click on the *Browse* button and select **FedEx Shipping** (type=j2store) and click on *Upload & Install*
3. Enable the plugin
4. Configure the shipping plugin by entering the plugin parameters

![](./assets/images/aus-ship-doc-1.png)
![](./assets/images/fedex-ship-method-list.png)
![](./assets/images/fedex-ship-config-1.png)
![](./assets/images/fedex-ship-config-2.png)


### Parameters
Consider the images for setting up the parameters.

**Here is the instructions for identifying Fedex credentials** (Authentication key and meter number).
https://support.shippingeasy.com/hc/en-us/articles/203087899-How-do-I-find-my-FedEx-Meter-Number-

##### 1. Key
This is a unique FedEx key required to login.

##### 2. Password
This is the password provided by FedEx and not your website login password.

##### 3. Account Number
This is your FedEx account number.

##### 4. Meter
This is your meter number provided by FedEx.

##### 5. Handling Cost
If you need to charge a handling cost for the shipping, you can provide it here.

##### 6. Display Delivery Time
To show the delivery time, set this option to **Yes**.

##### 7. Test Mode
For live account, set this to **No**. For test account, set this to **Yes**.

##### 8. Services
You can select one or more services offered by FedEx in this field for display in checkout page. 

##### 9. Drop Off Type
Here is a list of drop off types and you can select one from the list.

##### 10. Packaging Type
Here, a list of packaging types are available, with various dimensions. You can select one or more types.

##### 11. Rate Type
Valid values for rate type are:
1. Account - This method uses the customers' account rate as the basis for the calculation of additional charges.
2. List - This type uses the FedEx list rate as the basis for the calculation of additional charges. 

##### 12. Tax Class
If shipping is taxable and you want to add tax rate, select a tax profile in this option.

##### Geozone
If you want limit this shipping method to particular areas, then you can select the corresponding geozone in this option. If this shipping is applicable to all areas, then set it to **All**.

##### Debug
If you set this to **Yes**, then an error log file will be maintained in the cache folder. It suitable for test account.

>Always set Debug option to **No** in live accounts

### Support
Still have questions? You can reach us in support@j2store.org 

Thank you for using our extension.











