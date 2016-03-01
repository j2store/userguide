####[HOWTO] Change default country in checkout

1. Login to Joomla administrator and go to Components -> J2Store

2. Go to Set up - > Custom fields

3. Open the Country field and choose your default country. Save.

4. Open the Zone ID field and choose your default zone. Save.

5. Clear Joomla cache and check.

####[HOWTO] Order products in list layout
The product list layout by default takes the ordering in the Article Manager. However, you can change this ordering (on page load / refresh) via the Menu Parameters.

NOTE: This tutorial applies only for those using the J2Store's Product List Layout in Version 3. If you use the default article layouts, refer the Joomla documentation on ordering of articles.

Login to Joomla administration and open the menu that links your product list.

Under the Common Options tab, you can find Article Order parameter. There you can choose the ordering method.

![](assets/images/troubleshoot_orderproducts.png)

####Troubleshooting update related issues

J2Store uses the Joomla Extension Manager for providing updates to both the free and pro users. On a few occasions, you may not be able to access the updates via the Extensions Manager. You may get a 403 access denied when you try to update in your site. It might be due to several reasons. We have listed a few that might cause this problem.

* **Download ID:**

   We provide a Download ID when you subscribe. You can find this Download ID in two places.
1.In the PDF invoice we have issued to you
2.In our website's My Downloads section. Direct link: http://j2store.org/my-downloads.html

  You should copy the Download ID and paste it in J2Store - Set up - Configuration - Update tab.

  NOTE: If you have re-set your password in our site, then a new download ID will be issued (due to security reasons and prevent unauthorized access.) 
Please make sure that the Download ID is correct.

* **Time out:**

  J2Store uses the Joomla Extension Update tool. A time out will occur if your connection is slow or if our server responds slower (which sometime occur if there are huge number of download requests)

  In this case, just try again after a few minutes. You will usually get through.
  
* **Firewall:**

  If you make repeated attempts or requests, then our firewall might block the access for a temporary period (usually 10 minutes).

  In this case, please try after 10 minutes.

  If still you get the error, you can always download the latest version from our My Downloads section: http://j2store.org/my-downloads.html and install it via the Extensions manager.
  
####[HOWTO] Migrate from version 2.x to version 3.x

With the release of Version 3, J2Store has emerged into a much more powerful e-commerce application for Joomla. Version 3 of J2Store is completely re-written from scratch using FOF Framework and follows a completely different table structure. It comes with quite a lot of new features and supports different product types.

As a result, you cannot install Version 3 directly over the version 2. It involves a migration. And don't worry!. We have simplified the migration process by developing a nice tool. We have also created a step-by-step guide that will walk you through the entire migration process.

[Click here to Download the migration tool and read the guide](http://j2store.org/support/user-guide/migrating-from-2-x-to-3-x.html)

####[HOWTO] Options from dropdown cannot be selected

This issue occurs when your site has two instances of the Jquery UI library.

![](assets/images/options_dropdown.png)

**In Version 3:**

Go to Configuration - basic settings
Set the Load Jquery UI to Only Front End.
Save

**In Version 2 :**
Go to J2Store - Options - Basic settings
Set the Load Jquery UI to Only Front End.
Save.

Clear Joomla cache and refresh. Now try

####Troubleshooting USPS, FedEx, UPS and CanadaPost shipping plugins

You have installed the shipping plugin but it doesn't show up during the checkout. Here are a list of reasons that might be preventing the plugin from fetching shipping cost real-time from the APIs of the Shipping carrier.

* **Enable Shipping**

  Well. This might sound trivial. But some of us often forget to turn on the Enable shipping switch while creating the product. Make sure that Enable shipping is set to YES.
  
* **Weight and Dimensions**

  All the shipping carriers use the weight and the dimension of your product (Length, Width & Height)to calculate the shipping cost (besides using the destination address). So make sure that you enter the Weight and the dimension of your product.

 You should select the weight and the length measurement unit from the drop down list.
 
 ![](assets/images/troubleshoot_shipping_one.png)

 **IMPORTANT for those using UPS:** Only KG (Kilogram) and LB (Pound) are supported by UPS as the weight measurement units.  Similarly, only IN (Inch) and CM (Centimetres) are supported as length measurement units. There is more. If you use Pound (LB) as the weight measurement, then the length measurement should be Inch (IN). Similar if KG is used, then CM should be the measurement.

 Also make sure that you choose the correct measurement units in the plugin settings as well. If the measurement units used in the products does not match with the settings in the plugin, then J2Store will attempt to convert the values to the measurement unit set in the plugin.

* **API credentials**

  All shipping carriers have a web service and provide credentials to access their Rate API. Some of the carriers like USPS offer TEST accounts as well. Make sure you enter these credentials correctly in the Plugin. Some of the carriers provide Customer number (like Canada Post ) and a few other parameters as well. Refer the documentation PDF that come with each plugin for more information.
  
* **Geozone**

  All the plugin come with a geozone filter setting.

  If you choose a geozone, then this shipping plugin will apply to only to customers coming from the countries/zones added under it.

  During testing, make sure that this param is set All geozones.
  
* **Debug Mode**

  In your plugin settings, set the Debug mode to YES. This will allow the plugin to log the responses sent by the APIs of the shipping carriers.

  The log is stored in the /cache folder of your Joomla Root. You can use your Hosting CPanel's file manager or an FTP program like FileZilla to access the log file. The log should give you a lot of information.
  
  ![](assets/images/troubleshoot_shipping_two.png)

 ***VERY IMPORTANT: Debug mode SHOULD NOT be enabled in LIVE / PRODUCTION sites.***
 
Still not working, please create a private ticket or email us the log file. We will help you troubleshoot the plugin.

####A simplified guide for New EU VAT rules 2015 and setting them up in J2Store

