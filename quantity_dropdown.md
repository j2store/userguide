# Quantity Dropdown

This app allows your store to update the price of a product based on quantity in the product page itself. Your product page normally displays the price for a unit quantity of a product. When a customer selects a higher quantity of the product, he can view the total price of the product only in his cart. But with this app he can automatically view the updated price for a higher quantity of the product in the same product page.

#### Requirements

* PHP 5.4 or higher
* Joomla 3.x or higher
* J2Store 3.2.10 or higher

#### Installation

1. Download Quantity dropdown from our site and install it using Joomla installer.
2. After installing the app, go to J2Store > Apps and find Quantity Dropdown app.
3. Click on **Enable** to activate the app.
4. Click on **Open** to configure basic settings of the app.

#### Configuration

**Apply change price based on ?**

Choose how the app should work. If you select **Common settings**, quantity dropdown feature will apply for all product (i.e.) it will work as global. Choose **Per product settings** to work based on individual product setting.

If you choose **Per product settings**, go to Article manager -> Open the product -> J2Store cart tab -> Apps where you should enable Product quantity dropbox. See the image below

![per-product-level](./assets/images/quanity-dropdown-02.png)

**Apply price change based on quantiy for all product ?**

Choose **YES** to enable price change for all products. This option will work only when you choose **Common settings**.

**Display quantity box type?**

Choose Quantity box display type from the options(Dropbox, Default) available.

* **Dropbox :** Choosing this option will display quantity box in dropdown type.
* **Default :** Choosing this option will display default quantity box.

**Quantity**

This option is used when you select quantity box display type as **Dropbox**. Enter the values for quantity dropdown here with comma (,) separated. For example, 10,20,30.
![common-settings](./assets/images/quanity-dropdown-01.png)

#### Frontend Demo

![frontend](./assets/images/quanity-dropdown-03.png)

#### Support

Still have questions? You can post in our support forum: http://j2store.org/forum/index.html

Thank you for using our extension.