# Downloadable Product

- **[Introduction](#introduction)**
- **[Product Settings](#product-settings)**
	* **[Files](#files)**	
- **[A step-by-step example to create a downlodable product](#example)**

<a name="introduction"></a>
## Introduction

The product type allows you to sell digital products like PDF, images, audio, video, software, e-books etc.
Customer will be able to download the file immediately after making the payment.

<a name="product-settings"></a>
## Product Settings


The settings in this type are almost identical to simple product except a very few.

Since this is downloadable, obviously it has no shipping option. Likewise, there is no options page also, to choose a color or size, because it has no physical existence.

But there is unique option **Files** for this product type. Have a look over that option.

<a name="files"></a>
### Files
There are three options here to set before further action.

![Downloadable Files](./assets/images/product_down_files_1.png)

#### Product Files
First there is a button to select the downloadable files to set for the customer to view. When clicked, it will direct to a popup window in which the display name and the path of the downloadable file are set.

![Downloadable Files 2](./assets/images/product_down_files_2.png)

```php
VERY IMPORTANT: In configuration -> basic settings, the File attachment path field should point to an existing directory inside your website root.
If you specify a directory outside the public root, then you should enter the full file path manually.
```

#### Download limit
This determines the maximum number of copies allowed to be downloaded by a single customer. Enter a numeric value to set the limit.

#### Download Expires(in days)
This will set a deadline for the product link to be active to download the product. If the deadline set to be 15 days, for instance, the link goes inactive on the start of 16th day.

All other options are same as simple product.

<a name="example"></a>
## A Step-by-step example to create a downloadable product

**J2Store** implements an innovative concept in creating products. It uses the Joomla articles as products. So to create a product is to create an article.

So, lets create an article.

### Creating an Article

Have a look at the image below:

![Add Article](./assets/images/add_simple.png)

As given in the above illustration, click in the top menu or in the left pane of the control panel. You will get a new screen like this.

![Create Downloadable Product](./assets/images/down_create_cart.png)

A downloadable product is one that has no physical existence. It can be downloaded as per the terms and conditions of the seller. It can be a book, a video, a music album or even a software extension like joomla extension. To create a downloadable product, follow the steps:

* Enter the name for your product. 
* Since you are creating article, you need to tell that the article be treated as product. So, select 'Yes'. 
* Select the type of the product, i.e., 'Downloadable'.
* Now, click the 'Save and Continue' button.

Your product is successfully created and a message will be displayed like this.

![Downloadable product created](./assets/images/down_create_success.png)

Add a description for the product, as illustrated below.

![Add Description](./assets/images/down_create_content.png)

The Configuration process follows:

#### General

Enter the details as required by the fields in the tab, like, SKU, UPC/EAN, brand, vendor, tax profile and the caption for the cart button. Once you enter them, you can navigate to the next tab, pricing.

![General Tab](./assets/images/down_general.png)

#### Pricing

In Pricing you can set the price for your product. You have the option to set up advanced prices, like discount offers, as shown in the following images.

![Pricing](./assets/images/down_pricing.png)

In the above image you set up the regular price for the E-Book. Click the set prices button to set advanced/special prices. It will pop-up a window to set the special prices, like this.

![Set Price 1](./assets/images/down_add_price_1.png)

In the above image, you can set a date range for the special price, otherwise, you can leave it empty for the special price to be applied always. For example, if a customer buys 2 or more copies of the E-Book, you can offer a discount in price, throughout the year. Now, you have entered the values, and click the blue 'Create' button and you will get the special price listed below, as shown in the image.

![Set Price 2](./assets/images/down_add_price_2.png)

#### Images

When you select the images tab, you will get a screen like this.

![Images](./assets/images/down_images.png)

Click on the select an image button. You will get a pop-up window, where you can select suitable image for your ebook, as shown below:

![Select an Image](./assets/images/down_image_select.png)

Once you finish the selection, your tab will be like this.

![Images Selected](./assets/images/down_images_selected.png)

#### Files
Unlike other products, you do not have options and shipping tabs for a downloadable product. But there is a unique tab, **Files** is present here. You must have a separate folder or directory in your site to place the downloadable products. From that folder, the product will be downloaded, when the buyer fulfills the requirements for the download.

The following steps will guide you to set up a folder with downloadable product.

##### Step 1 : Create a folder on your site to upload the files

You can use your Hosting Provider's CPanel File manager or an FTP client like FileZilla, to access your web root (public_html / www / httpdocs ).

Once you are in the web root, you can create a folder. Name it as: myfiles.

##### Step 2: Protect the folder from outside access

We do not want people to access this folder using their browser and download files. So let us protect this folder using a **.htaccess** file.

Create a file called htaccess.txt in your computer and open it with your favorite text editor. Add the following lines to it.

    order deny, allow

    deny from all

Save the file. Now upload it to the folder we just have created in our web root. In our example, it is myfiles.

>**IMPORTANT**: Rename the file as ***.htaccess*** 

All the files uploaded to this folder, are now protected.

##### Step 3: Point J2Store to use the files in this folder.

Go to Joomla admin -> j2store Dashboard -> Set up -> Configuration -> Basic settings

In File attachment path field, enter the name of the folder that contains your files. In our example, it is: **myfiles**.

Check the image below:

![Set folder to place downloadable Products](./assets/images/down_upload_folder_config.png)

Finally, save the configuration. You have created a folder to upload your digital products like ebook, pdf files, image files etc., set up protection mechanism from unauthorized access and configured the folder in your configuration page.

Now, Configure your **Files** tab in your downloadable product creation.

The tab will look like this:

![Files](./assets/images/down_files.png)

When you click the set files button, you will get a pop-window to select the file to be downloaded. See the picture.

![set files 1](./assets/images/down_set_files_1.png)

And select the file and click the create button, and you will get the product listed below as shown in the picture. You can add as many files as you can to the folder. When a customer purchases the product, all the files associated with the product will be available for download.

![set files 2](./assets/images/down_set_files_2.png)

Set the download limit (0 for unlimited downloads) and expiry of the download, in days, as shown in the picture below:

![Files](./assets/images/down_files_1.png)

##### Let us create a Downloads Area for the customers

* Go to Joomla admin -> Menus -> YOUR MENU
* Click New to create a new menu
* Enter a Name
* Click Select against the Menu Item Type. You will get a popup
* Choose J2Store -> Downloads
* Save

Check the image below.

![my profile](./assets/images/down_my_profile.png)

You just have to tell the customers to visit this menu to get their files after the purchase.

When the customer purchases the downloadable product, and finishes the checkout process, the order is completed and the status become 'Confirmed'. If My Profile is clicked, the orders will be listed as shown below:

![My Profile](./assets/images/down_my_profile_front_end.png)

And when 'Downloads' tab is clicked, it will show the download link like this:

![Downloads](./assets/images/down_downloads_front_end.png)

#### Filters
The filters will help to narrow the product search, for specific products. For e.g., if you add filter with value 'music', the search will display only music files.

See the image below:

![Filters](./assets/images/down_filters.png)

#### Relations

The next tab is Relations. Here, you can add products of higher value than the one being viewed by the customer and recommend the customer to buy that product, citing its advantages and additional features. This is an upsell.

Refer the image below:

![Relations](./assets/images/down_relations.png)

Also, you can add some other products to convince the customer to buy theses products additionally. This is cross sell.

For more detailed explanation, refer to the **Relations** section of the **Downloadable Product**.

#### Apps

In this tab, you can add third party tools or plugins, that are available, to enhance the J2Store functionality, like adding additional fields, applications, functions or features.

![Apps](./assets/images/down_apps.png)

Now, lets have a look on how your product is viewed in your online store. Check the image below:

![E-Book cart View](./assets/images/down_product_on_cart.png)