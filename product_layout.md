# Product Layout

- **[Product Layout](#product_layout)**
	* **[Create a Product Layout](#create_layout)**
	* **[Details Tab](#details_tab)**
	* **[Common Options Tab](#common_options)**
	* **[Item View options in category listings](#item_category)**
	* **[Item View Options Tab](#item_view)**
	* **[Special Module Positions](#special_positions)**
	* **[Avoid Zoom effect and open the main image in popup](#zoom_popup)**
- **[Common Problems](#common_issues)**

<a name="product_layout"></a>
Product Layout is a powerful feature that enables the user to customize the display options and descriptions of the product. In this section, you'll learn how to create and customize a product layout.

>Note: Product layout works only with Joomla articles. If you use SEBLOD / FLEXIcontent / or any other catlog systems, then you may need to configure the product layouts using their menu items.

<a name="create_layout"></a>
### Create a Product Layout
To create a product layout, go to joomla control panel and click on the menu item **Menus -> Main Menu** as shown in the image below.

![Product_Layout](./assets/images/product_layout_create_1.png)

You will get the list of menus that are already present as shown in the image below.

![](./assets/images/product_list_view_2.png)

To create a new item, click on the **New** button and you will get this page.

![](./assets/images/product_list_view_3.png)

First you need to enter the title of the item you create. For example, it is entered with **Apparel**. The alias will be automatically generated based on the title.

Then, you have several tabs in this page. Let us see one by one. First is the **Details** tab.

<a name="details_tab"></a>
#### Details Tab
Here, you choose the **Menu Item Type** by clicking on the 'Select' button. You will get a pop-up window like this:

![](./assets/images/product_list_view_4.png)

In this pop-up window, select **J2Store** and you will get a list to choose from. From the list, select **Products List View** and close the window. You will see your selection as shown in the below image.

Your menu item is selected and the link is also created automatically. click on the **Choose a Category** text box to choose the product categories listed. You can add many categories in this box. Refer the image below.

![](./assets/images/product_list_view_5.png)

Now, go to next tab, **Common Options**.

<a name="common_options"></a>
#### Common Options Tab
![](./assets/images/product_list_view_6.png)

This tab has the common settings for all items. If you want to show images for product options or if you want to add some custom CSS code, you can do that here. Otherwise, you can leave them as they are.

>Note: In Sub-Template option, you have to choose **bootstrap3** if your bootstrap version is 3x. Leave it as **--Default--** if bootstrap version is 2x

If you do not want to show product option price in front end, you can set the option to **Hide** as shown in the image below:

![](./assets/images/product_list_view_7.png)

<a name="item_category"></a>
#### Item View options in category listings
Check the image below:

![View_category_listing](./assets/images/product_list_view_8.png)

In this tab, you are setting the configuration for how to display the product in the cart and the features and options to display with the product.

You can display any number of products as you like in the shop. Enter the no of products to be displayed in the text box provided and the number of columns in which the product display is divided.
As the no of products increases, the image display size will be decreased. 

Also, select all other options as per your choice. Refer the next image.

![View Category Listing](./assets/images/product_list_view_9.png)

From the image you can see that there are many options available to set the price, image, size of the image and many more attributes.

>CAUTION: SKU Show/Hide setting can be done in two places, i.e., in configuration setup and in product layout. Product layout setting will be given higher priority, i.e., if SKU is set to **Show** in configuration and again it is set to **Hide** in product layout, the configuration setting will be overridden and the SKU will be set to **Hide** as it is in product layout. As a result, SKU will not be shown in frontend.

Next image shows the filters.

![View_category_listing](./assets/images/product_list_view_10.png)

![](./assets/images/product_list_view_11.png)

Filters help narrow the search for a particular product. There are many filters available for the search. 

* Sort Filter
* Search Box
* Category Filter
* Price Filter
* Product Filter
* Manufacturer / Brand Filter
* Vendor Filter

One or more filters can be applied as per the needs of the customer.

<a name="item_view"></a>
#### Item View Options Tab

In this tab, you will set the configuration for what to display with the product, like price, description, image etc.

See the image below:

![Item view Options](./assets/images/product_list_view_12.png)

This image shows the options you have to set the configuration for a product on what has to be displayed along with the product. The available options are: 

* Title
* Short Description
* Long Description
* Regular Price
* Special Price
* Discount Percentage
* SKU
* Stock
* Main Image
* Additional Images
* Main Image Width
* Additional Image Width
* Enable Zoom Effect
* Brand 
* Upsells
* Cross Sells
* No of columns for related products
* Show Specification
* Show description and specifications
* Show link to product list

![Item View Options](./assets/images/product_list_view_13.png)

Using this parameters, you can determine what are the details and how they should be displayed in the online shop.

Apart from these four tabs, there are four more tabs and they should be left with the default settings. You need not worry about that.

Now, Save the item by clicking the **Save & Close** button. You will get the screen as shown in the image below.

![Product Layout Create Success](./assets/images/product_layout_create_success.png)

Now, let us see how this is viewed in the shopping page. 

![Home page](./assets/images/product_layout_frontend_home.png)

In this image, you can see that the new menu item created is listed in the top with the other menu items. You can click that to see the products of your store, like the image below.

![Shopping page](./assets/images/product_layout_frontend_apparel.png)

In this page, you can see the product layout features. The filters are positioned in the right side as per the selected choice. You have the option to filt by price, brand, vendor etc. The regular and special prices are also displayed along with discount percentage variation. 

Let us see how images are added in the backend and how they are displayed in frontend view.

Consider the image below:

![add images](./assets/images/salad_add_images.png)

In the image, you can see Main and Additional images added to the product configuration. When you configure your product, you will add images of the product for its view in the cart. You add main image of the product for the main view supported with additional images. Let us now check how it is viewed in the front end.

Check the image below: 

![additional images](./assets/images/prod_layout_addnl_images.png)

When you click on the product, it will be displayed with large image and additional images displayed below in small size. When you hover over the small images, you can see them in place of the main image. The below image explains this activity.

![additional image 1](./assets/images/prod_layout_addnl_images_1.png)

Like this, you can set different product layouts according to your wish and needs.

<a name="special_positions"></a>

##Special Module Positions

  J2store offers special module positions to place the Joomla's custom HTML module.Following are the custom module positions :

1. **j2store-single-product-top** - Top of product view layout

2. **j2store-single-product-bottom** - Bottom of product view layout

3. **j2store-product-list-top** - Top of product category listing page

4. **j2store-filter-left-top** - Top of left filter

5. **j2store-filter-left-bottom** - Bottom of left filter

6. **j2store-filter-right-top** - Top of right filter

7. **j2store-filter-right-bottom** - Bottom of right filter

8. **j2store-product-list-bottom** - Bottom of product category listing page

9. **j2store-cart-top** - Top of cart page

10. **j2store-cart-bottom** - Bottom of cart page

11. **j2store-checkout-top** - Top of checkout page

12. **j2store-checkout-bottom** - Bottom of checkout page

<a name="zoom_popup"></a>
##Avoid Zoom effect and open the main image in popup

To avoid the zomm effect and to bring the image in pop up, first thing you have to do is disable the zoom effect in admin backend.

####Disable zoom in J2store product layout

Go to menu manager and open the menu which links to J2store product layout.

Move to Item view options tab

Set **NO** to Enable Zoom effect.
![](assets/images/zoom_popup_1.png)

####Disable zoom in Category blog layout

Go to Extensions > Plugins.

Select type **content**.

Open the Content - J2Store plugin.

Set **NO** to Enable Zoom effect in Item view tab.
![](assets/images/zoom_popup_2.png)

####Override view_images.php

Once disbaled the zoom effect, follow the override procedure given below :

Copy /components/com_j2store/templates/default/view_images.php

to

/templates/YOUR_TEMPLATE/html/com_j2store/templates/default/view_images.php

Open the file and on around line no 22 find the below code

```php
<span class="<?php echo $class; ?>" id="j2store-item-main-image-<?php echo $this->product->j2store_product_id; ?>">
		  	 <img itemprop="image"
		  	 alt="<?php echo $this->product->product_name ;?>"
		  	 class="j2store-product-main-image j2store-img-responsive" src="/<?php echo $image_path.$main_image;?>"
		  	 width="<?php echo intval($main_image_width); ?>"
		  	 />
		  	 </span>
```
Change this with
```php
 <span class="<?php echo $class; ?>" id="j2store-item-main-image-<?php echo $this->product->j2store_product_id; ?>">
		   <?php JHTML::_('behavior.modal', 'a.modal'); ?>
		  	 <a href="<?php echo $this->product->main_image;?>" class="modal"><img itemprop="image"
		  	 alt="<?php echo $this->product->product_name ;?>"
		  	 class="j2store-product-main-image j2store-img-responsive"
		  	 src="<?php echo $image_path.$main_image;?>"
		  	 width="<?php echo intval($main_image_width); ?>"
		  	 /></a>
		  	 </span>
```
<a name="common_issues"></a>
##Common Problems

####Grid layout not working/columns.Why?

 The issue seems to be the wrong sub-template.
 
 Open your product list layout menu. In Common options tab -> set the sub-template as Bootstrap3.
 
 Save

 This should solve the issue. If it is already set to Bootstrap 3, then try to set it as Default.
   
####Preview addictional image after click

 copy
 /components/com_j2store/templates/default/view_images.php

 to

 /templates/YOUR_TEMPLATE/html/com_j2store/templates/default/view_image.php

 edit the file and remove the highlighted line fully.
   
 ![](assets/images/avoid_mouseover.png)
   
####How to add Category description in list view

* Create custom module and assign it to the menu which links to J2store product layout.
  
* Set the module position to j2store-product-list-top.
  
* Save.

Now the custom module will display the description only in list view.