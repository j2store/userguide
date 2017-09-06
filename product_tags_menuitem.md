# Product Tag Layout


Starting from the J2Store version 3.2.25, we have presented a new menu item type  for creating tags for products.

With this new feature,you could display products based on  the tags.

When a tag is added to two or more products in the backend , the products that fall under that particular tags will be displayed in the front end,when the  menu is chosen.

## Overview

* It is necessary to create a product tag before creating a menu of the type product tags.

* Create an article and add the tag to it.

* Create the menu item of the type Product tags and choose the tag that would act as the filter to display the products(More like the category).

## Creating a product tag

To create a product tag, the steps given below have to be followed:

* Navigate to Components->Tags.

* Click New to create a new tag.

* Enter the title of the tag,give a description to the tag and choose the parent tag(if any)  as per the requirements.

* You could also add a note to the tag,refrain the user groups and choose the language for which the tag has to be applied.

The following screenshot is an example for a tag:

![](./assets/images/creatingatag.png)

## Adding a tag to the product


Once a tag has been created, the next step would be to add it to the product.That can be done as simple as this:

* Navigate to Content->Product article.

* In the Content tab,the tag can be added in the Tags column.

![](./assets/images/addingtagtoproduct.png)


## Creating a menu of the type product tag

Post creating  the tag and adding it to the product's article,the next step would be to Create a menu item of the type Product Tags.Following are the steps that have to be done:

* Click on Menus->Menu Items->New.

* The menu title has to be given and the menu item type should be "J2store product Tag Layout".

* The next option would require you to select the tag for the menu item.Choose the tag that has to be associated with the menu item.

* Additional Step: Click on the Common options tab and choose the Sub-template to tag_bootstrap3. This is the sub-template that should be chosen to display the tags on the layout unlike the default one.

* You could also choose the level of sub tag until which the products have to be displayed under the "Item view in Category listings" tab in the option "Sub Tag level".

The  below images show how a menu item of the type "Product tag" is created.

![](./assets/images/producttagmenu1.png)

These are the other options that can be chosen when it comes to Product Tag layout.

![](./assets/images/producttagsubtemplate.png)

You could choose the sub-tag level in case you have tags that contain parents in the followinfg way:

![](./assets/images/producttagsubtag.png)

The frontend display of the tag layout will be as below:

![](./assets/images/producttagfrontend.png)
