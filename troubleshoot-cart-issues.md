# Troubleshoot cart related issues

* **[Not adding items to the cart](#items-not-added)**
* **[Cart cleared during registration](#cart-clear)**
* **[Template override for Add to cart block in category view](#template-override-category-view)**
* **[Template override for Add to cart block in detail view](#template-override-detail-view)**
* **[Is cart not responding when you click update or empty cart button?](#cart-not-responding)**
* **[Minicart icon not showing up?](#minicart-icon)**
* **[[HOW TO]Add cart module right or left below the product filter?](#cart-module-filter)**
* **[Avoid cart items cleared](#cart-items-clear)**
* **[How To Solve Mini Cart module related issues?](#cart-module-issues)**
* **[I don't see Add to Cart Button. What is the problem?](#not-show-cart-button)**
* **[HOW TO move Add to Cart Button using the Short Plugin tag](#move-cart-button)**

<a name="items-not-added"></a>
#### Not adding items to the cart

EU e-Privacy Directive plugin does not even allow the Joomla session cookie.
That means, no one can login in the front end including customers.

In the plugin settings, make sure the Joomla session cookie is allowed.
J2Store saves the cart data in the Joomla session and maintains the cart record id there and also address information (if checked out as guest).
So J2store at least requires you to allow the Joomla session cookie.

<a name="cart-clear"></a>
#### Cart cleared during registration

It is beacuse the default Registered group and Guest group chosen might be wrong.

Please go to User manager -> Options
Make sure the Default Registered Group is set to: **Registered**
Default guest user group is set to : **Guest**

![](./assets/images/cart-clear-01.png)

And make sure you do not have any cookie domains in Joomla admin - Global configuration.

To validate if your settings are correct, try this basic Joomla feature:

Try to login as a user in the frontend. If you are able to login and stay logged in, then your user settings are correct.
If you could not login, then your user manager settings are not correct.

<a name="template-override-category-view"></a>
#### To change the Add to cart block and style in category view

copy /components/com_j2store/templates/YOUR-SUB-TEMPLATE/default_cart.php

to

/templates/<YOUR_TEMPLATE>/html/com_j2store/templates/YOUR-SUB-TEMPLATE/default_cart.php

**IMPORTANT:** If you are using bootsrap 3 as a sub-template, replace the default with bootstrap3(/components/com_j2store/templates/bootstrap/..)

<a name="template-override-detail-view"></a>
#### To change the Add to cart block and style in item view

copy /components/com_j2store/templates/YOUR-SUB-TEMPLATE/view_cart.php

to

/templates/<YOUR_TEMPLATE>/html/com_j2store/templates/YOUR-SUB-TEMPLATE/view_cart.php

Make the changes and save.

<a name="cart-not-responding"></a>
#### Is cart not responding when you click update or empty cart button?

If you enable **System - Page Cache** / SpeedCache or any thidy party cache plugins, they photo copy every page including the cart page.
Though the cart page is dynamic, it would not listen. It would just photocopy the page and stores it. Until cache is cleared, it will keep serving the photo-copied page.

In eCommerce / dynamic websites, you should not use Page Caches likes System - Page cache plugin.

Please disable the cache plugins like System - Page Cache. Clear your cache and check.

Another thing:
**Progressive caching**. It is not a recommended cache method. This will override modules having dynamic content and cache the module output as well (Imagine the cart module. Its contents change. But progressive caching will not listen even if you set in the Module advanced settings to No Caching).

Please use the **Conservative caching**.

<a name="minicart-icon"></a>
#### Minicart icon not showing up?

It seems to be applying wrong font-awesome class in module settings page.

Open J2Store cart module
You can see something like below entered in the Minicart icon class text box
```html
fa fa-shoppingcart
```
Change with
```html
fa fa-shopping-cart
```

Save.

<a name="cart-module-filter"></a>
#### [HOW TO]Add cart module right or left below the product filter?

You can use special module positions in the filter display section to display the cart module to the product filter.

**j2store-filter-left-top** - Top of left filter

**j2store-filter-left-bottom** - Bottom of left filter

**j2store-filter-right-top** - Top of right filter

**j2store-filter-right-bottom** - Bottom of right filter

For more details about special module position, please click [Here](https://www.j2store.org/support/user-guide/special-module-position.html)

<a name="cart-items-clear"></a>
#### Avoid cart items cleared

Sometimes customers accidently entered wrong credit card / debit card details. He came to know that he entered wrong card details only after clicking on place order. But cart items will be cleared once you clicked place order button. So you could not retry the payment process and it makes you frustrating.

To overcome this, you can restrict clearing cart items only on order confirmation.

Go to J2Store > Configuration > Cart tab
Find the param "Clear cart items". Set this param to "On Confirmation" and save.

<a name="cart-module-issues"></a>
#### How To Solve Mini Cart module related issues?

J2Store's Mini Cart is a very handy tool for your customers when they shop. They can check the number of items in their order and the total. The cart module is refreshed in real-time using an AJax request. On a few occasions, the cart may not get updated on a real time. Here is a checklist that should help you solve the problem.

##### Cache settings
Go to Joomla admin - Global configuration - System tab.

Caching is like taking a snapshot of your pages and presenting the same to every visitor coming to your site (untill the cahce is refreshed again).

Since the cart module handles dynamic data, it should be excluded from caching. In order to exclude the module from caching, your Global cache setting should be set either to Conservative Caching or Disabled. Check the screenshot below.

If you use Progressive Caching, Joomla will override the Cache settings in the module. The cart module might work fine in smarller sites with Progressive Caching enabled but if you have a larger site with a large number of visitors, then it might cause issues with the module.

![](./assets/images/cache_settings.png)

##### Module settings

Go to Joomla admin - Module Manager - J2Store Cart module

In the Advanced tab, set the Caching to No Cache.
![](./assets/images/mod_cache_settings.png)

##### Javascript conflict

Since the J2Store updates the cart module using an AJAX request, it is important that your site does not have any javascript conflicts.

Javascript conflicts mostly occur due to loading of multiple jQuery libraries or the lack of a Javascript library. it is possible that a third party extension / module in your site might be using an older or incompatible javascript library, which might produce a conflict.

Solution A:

Please download and install a jQuery Script manager like jQuery Easy and configure it. This should solve most of the issues

Solution B:

It is not exactly a solution. Its a troubleshooting method. Open your website in the Google Chrome browser. Open the browser menu and go to Tools -> Developer Tools.

You can see the Developer Tools window opening at the bottom of the browser. Navigate to the Console tab.

Now Refresh your website. The Console tab will show you if there are any javascript conflicts in your site. It will also show you the file name and the line number that produce the error. Take a screenshot and send it to us and also send a copy to your template provider. We will check and get back to you with the solution.
![](./assets/images/developer_tools_console.png)

##### JSON support

While most of the hosting service providers enable the JSON support for PHP by default, some do not. It is easy to check if JSON is enabled or not in your hosting account.

Go to Joomla admin - System - System Information - PHP Information

You can check whether JSON support enabled or not in the PHP Information tab. if you do not find any mention of JSON, then you can assume that it is not enabled for your account. You should get in touch with hosting service provider, who can enable the JSON support for your account.

You can look for something like below in the PHP Information tab.

![](./assets/images/json_setup.png)

<a name="not-show-cart-button"></a>
#### I don't see Add to Cart Button. What is the problem?

Don't worry. This is often a simple configuration mistake. We have answered this question more than hundred times.

This post explains the reasons behind this. Make sure you check the following points before writing to us or posting in the forums.

**Step 1:**

  Go to Joomla admin - > J2Store -> configuration -> product tab
  Set the Catalog Mode to NO and save

  Catalog Mode: The term itself explains that your products are just a catalog. Set this param to YES, only when you dont want your customers to purchase from the website and just provide price information. Otherwise, this param should always be set to YES.

  Check your store front. Still you can't see the add to cart button? Move on to Step 2.
  
**Step 2:**

  If you are here, then you need to check another parameter.

  Go to Joomla admin - > J2Store -> Configuration  -> Cart tab.

  Did you set the Add to cart placement to Within article using tag:

  If yes, then go to Article Manager and open your article / product.

  In the content area, did you enter the J2store plugin tag somewhere?

  You can find the correct tag ( a plugin shortcode) under the J2store cart tab.  You can copy the shortcode and paste in the content area.

  Now save the article. Now you will be able to see the Add to cart.
  
**Step 3:**

  Still no luck. Then there might be a template override for the articles or some other plugin is causing an issue. 
Post in the forums with URL to a product in your site. Our support team will take a look and help you solve the issue.

<a name="move-cart-button"></a>
#### HOW TO move Add to Cart Button using the Short Plugin tag

  You can move the location of the Add to cart block within the product layout using a simple plugin tag. 

There are a few steps involved in using the plugin tag feature. Read on to understand.

**Step 1: Change the Add to cart placement param**

  By default, the Add to cart button will appear after displaying the product (article) content. You can, however, change this and take control of its placement. You first need to change the param that controls the add to cart placement.

Go to Joomla admin - J2Store - Configuration - Cart tab

Set the Add to cart placement to Within article using tag and save. (See the picture given below).
![](./assets/images/cart_placement.png)
```
NOTE: You can also set the param to BOTH. In that case, the cart block will display at two places - a place where you entered the plugin tag and its default location.
```
**Step 2: Using the plugin tag in product content (article)**

 Now go to Joomla admin -> Content -> Article Manager.
 Either create an article (product) and save or open an existing product.

 Go to the J2Store Cart tab. You will find the plugin tag to use for the product.
 (see the screenshot below)
 ![](./assets/images/cart_tag.png)
 
 Either copy the plugin tag  and note it down. In this example, the following plugin tag is used {j2storecart 2} Here 2 is the product ID (aka, Article ID )

Now go to the Content tab and enter the plugin tag

Now save the article.

You will now see the add to cart block placed at your preferred location.