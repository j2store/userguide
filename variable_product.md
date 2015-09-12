# Variable Product

- **[Introduction](#introduction)**
- **[Product Settings](#product-settings)**
	- [General](#general)
	- [Images](#images)	
	- [Variants](#variants)
	- [Filters](#filters)
	- [Relations](#relations)
	- [Apps](#apps)
- **[A step-by-step example to create a variable product](#example)**

<a name="introduction"></a>
##Introduction

Variable is a complex product type. It lets you define variations of a product where each variant may have a different attributes, e.g. SKU, price and stock level.
```
Since this is a complex product type, it might take some time (quite some time) to create it. You will need a lot of patience and also require quite some work. So be prepared.

```
A perfect example for a variable product is: T-Shirts. T-Shirts always come with the size and colour combination. Example: Small-Blue, Small-Red, Small-Green.

You will be adding a price, sku and stock PER combination.

**NOTE:** If your product does not require a combination or stock / price management for each variation, then a simple product will suit your requirements.


![Variable Product](./assets/images/product_variable.png)

<a name="product-settings"></a>
### Product settings


* **[General](#general)**
* **[Images](#images)**
* **[Variants](#variants)**
* **[Filters](#filters)**
* **[Relations](#relations)**
* **[Apps](#apps)**

<a name="general"></a>
### General

![Variable General](./assets/images/product_variable_general.png)

* **Visible in Storefront** - First select whether the product is to be displayed in front of the store. If it is, set the option to **'Yes'**
* **Brand or Manufacturer** - Select the brand or manufacturer of the product from the available list
* **Vendor** - Select the vendor from whom the product is available for purchase - ***This is J2Store PRO feature***
* **Tax Profile** - Specify whether the product is taxable and if it is, select the taxprofile relevant to the product

<a name="images"></a>
### Images

![Variable Images](./assets/images/product_variable_images_1.png)

This feature is available for native Joomla articles and in J2Store Product Layouts

To display the thumbnail, main and additional images in Joomla articles, you should first configure the Content - J2Store plugin in Plugin Manager. Otherwise, you wont see these images in your products.

Lets assume that a customer would like to purchase a car. Now, car images need to be loaded in this tab. 

* **Main Image** - The main image will be a general photo image of the car, that has to be uploaded by clicking on the 'Select an image' button and select the appropriate image from the files.

* **Thumbnail Image** - The thumbnail image would be something that represents the original product, but it would be a much smaller one to fit into a button, that will be shown up in the cart. By seeing this, the customer will understand that his product is displayed on the button and will click the button to see more details about the car.

* **Additional Images** - Additional images help the customer to know more details about the car, which will be showing the car view in many angles, and the customer will understand it clearly how it looks like, what the technical details of the car, the colour, and so on.


<a name="variants"></a>
### Variants

Variants are products of same type and nature but with different attributes. For e.g., consider a Laptop of a particular brand with certain attributes, say
* **Colour - Metallic Grey**
* **Screen - 15.6 inches**
* **RAM    - 2 GB**
* **HDD    - 500 GB**
* **SKU    - MTG8620**

and so on. This is a variant of the particular brand. Now, the same product with same brand, will be another variant with some attributes changed, like
* **Colour - Black**
* **Screen - 15.6 inches**
* **RAM    - 2 GB**
* **HDD    - 500 GB**
* **SKU    - BLK8640**

For both the items, brand and model name may be same, but the attributes like colour and SKU differs. These are two variants of a particular laptop brand.

* A variant defines how this product differs from other products of same type
* It may be SKU no, price, stock level or color

Lets discuss it with some image illustrations:

![Variant 1](./assets/images/product_variable_variant_1.png)

If you select 'Colour' from the list, your screen will look like this:

![Variant 2](./assets/images/product_variable_variant_2.png)

You can see the option you have selected from the list added down there. Now, save the form to proceed.

![Variant 3](./assets/images/product_variable_variant_3.png)

You can see '**Set Values**' near the option name **Colour** and click it. You will get a pop-up window to add attributes as illustrated below:

![Variant 4](./assets/images/product_variable_variant_4.png)

Once you are done, save changes and close the pop-up window to get back to the main window. Now you have set the values for the variants to be generated. Why wait, just go and generate the variants like this:

![variant 7](./assets/images/product_variable_variant_7.png)

The button you have clicked for variant generation will adjust itself to show you a message, 'Generating variants... Please wait'.

![Variant 8](./assets/images/product_variable_variant_8.png)

And that's it. You have your variants generated! Wonder how? Just check the image below for a surprise...

![Variant 5](./assets/images/product_variable_variant_5.png)

If you want to edit the properties of the variants, click the respective edit button of the property you wish to edit to get a pop-up window like this:

![Variant 6](./assets/images/product_variable_variant_6.png)

Now you know how to deal with variants, options, attributes, properties and how to edit them.

<a name="filters"></a>
### Filters

Filters are certain attributes that help narrow the search of a particular product.

For e.g., assume that a customer searches for purple t-shirts in the store. Now, the productfilter is set as colour > purple, to narrow the search. See the image below:

![Filters](./assets/images/product_variable_filters.png)

Now the cart will display only the purple t-shirts.

<a name="relations"></a>
### Relations

![Relations](./assets/images/product_variable_relations.png)

* In this tab page, relations are set for Upsells and Cross sells
* An ***upsell*** is to get the customer to spend more money – buy a more expensive model of the same type of product considered for purchase.
* A ***cross-sell*** is to get the customer to spend more money buy adding more products from other categories, additionally, along with the product intended for purchase.
* **Example**:
    The terms cross-sell and upsell are often used interchangeably because, let’s face it, this gets confusing. Say the customer is viewing a Laptop with 2GB/500GB for $500.

    * 4GB/500GB-> $550 - Upsell, same product family, more expensive
    * 4GB/1TB -> $700  - Upsell, same product family, more expensive
    * Laptop Bag -> $25 - Cross sell, related product, additional sell


<a name="app"></a>
### App

Custom fields / settings from applications will be displayed in this tab.

*****
<a name="example"></a>
## A step-by-step guide to create a variable product

**J2Store** implements an innovative concept in creating products. It uses the Joomla articles as products. So to create a product is to create an article.

So, lets create an article.

### Creating an Article

Have a look at the image below:

![Add Article](./assets/images/add_simple.png)

As given in the above illustration, click in the top menu or in the left pane of the control panel. You will get a new screen like this.

![Create Variable 1](./assets/images/create_variable_cart_1.png)

* Enter the name for your product. 
* Since you are creating article, you need to tell that the article be treated as product. So, select 'Yes'. 
* Select the type of the product, i.e., 'Variable'.
* Now, click the 'Save and Continue' button.

Your product is successfully created and a message will be displayed like this.

![Create Variable 2](./assets/images/create_variable_cart_2.png)

#### General
Now you need to configure your product with necessary details. Begin with general tab.

![General](./assets/images/create_variable_cart_general.png)

* If you select 'Yes' in the first option, your product will be displayed in the storefront
* Select the brand or manufacturer of the product from the list
* Select the vendor to order the product
* Select the taxprofile that mathces the product profile

Now switch to Images tab.

#### Images

![Images](./assets/images/create_variable_cart_images.png)

You can add main, thumbnail and additional images relevant to your product in this tab. Click the 'select an image' button to get a pop-up window to select the image.

![Images Select](./assets/images/create_variable_cart_images_select.png)

Move on to variants tab.
#### Variants

![Variants 1](./assets/images/create_variable_cart_variants_1.png)

If you select the option, then you need to set values for the option.

![Variants 2](./assets/images/create_variable_cart_variants_2.png)

In the image, as you can see, you have added the option color. Now, save the configuration by clicking ONLY the green coloured button 'Save'. DO NOT press any other button. Now, see the changes in the screen.

![Variants 3](./assets/images/create_variable_cart_variants_3.png)

You can see the blue link, 'Set Values' adjacent to the option 'Color'. Click this link to set some values for the option 'Color'. Then only you can generate variants. Go ahead with setting values and see what happens...

![Set Values 1](./assets/images/create_variable_cart_variants_setvalues.png)

If you select the value for the option and click the create button, you will get the resulting screen like this.

![Set values 2](./assets/images/create_variable_cart_variants_setvalues_1.png)

Close the window using the X in the top right corner and return to the tabs.

![Generate Variants](./assets/images/create_variable_cart_generate_variants.png.png)

Now, as shown in the image, click on the 'Generate Variants', a green colored button, to generate variants for the products.

![Generating Variants](./assets/images/create_variable_cart_genrating_variants.png.png)

As you click the buttons to generate variants, the buttons adjusts itself to display the message 'Generating variants... please wait'. Now its done. See the variants listed below, as shown in the image.

![Generated Variants](./assets/images/create_variable_cart_variants_generated.png.png)

Once the variants are generated, you can edit the variants and add necessary details to the variant. When you edit a variant, you will have all the tabs in cart except variant tab. Fill in the required details for the product variant.

![Edit Variants](./assets/images/editing_variants.png)

Having completed variants tab, now move on to filtes tab.

#### Filters

Here, you can set the filters to narrow product search. When you set filter value as 'Mens', all mens T-Shirts will be displayed. Likewise, women and kids. See the illustration below:

![Filters](./assets/images/create_variable_cart_variants_filters.png)

#### Relations

![Relations](./assets/images/create_variable_cart_relations.png)

The next tab is Relations. Here, you can add products of higher value than the one being viewed by the customer and recommend the customer to buy that product, citing its advantages and additional features. This is an upsell.

Also, you can add some other products to convince the customer to buy theses products additionally. This is cross sell.

For more detailed explanation, refer to the **Relations** section of the **Variable Product**.

#### Apps

![Apps](./assets/images/create_variable_cart_apps.png)

In this tab, you can add third party tools or plugins, that are available, to enhance the J2Store functionality, like adding additional fields, applications, functions or features.

Now, lets have a look on how your product is viewed in your online store. Check the image below:

![Poloshirt on cart](./assets/images/poloshirt_on_cart.png)