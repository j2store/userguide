# Product display module

The module which helps you to display the products wherever you want in your site. Sometimes you would like to showcase best selling products or featured products in your site on some specific place. In this case, the product display module will do that.

### Installation

1. Download the product display module package from our site and install it via Joomla installer.

2. After installing, go to Extensions > Modules and create a new module with type J2Store products display and configure it.

### Basic settings

**Sub-template**

The module comes with three following sub-templates:

   * **Default**: Choose this as your sub-template if your site's template has bootstrap 2 support.

   * **Bootstrap 3**: If your site's template has full bootstrap3 support, then choose Bootstrap 3 as your sub-template.

   * **Carousel**: If you would like to showcase your products in a slider mode, then choose carousel as your sub-template. This will enable auto slide on the products.

**J2Store menu id**

If you have atleast one menu item with type as J2Store > Product list view, the links on the product will take the id of that menu. If you don't have any menu, then the link will use the non-sef url for the title and image on the product.

If you wants to use sef url, then create atleast one menu item with type J2Store > Product list view and then choose this menu in this option.

**Display product based on following sort**

You can sort out the arrangement of product by using this option. For example, if you would like to display the products based on SKU, then you can choose either SKU (A_Z) or SKU (Z_A).

**Product source**

There are three sources from where you could fetch and dislay the products. For example, if you would like to display the products from categories, then choose **Categories** as your product source.

#### Select based on categories

**Category**

If you have chosen the categories as your product source (to the above parameter), then you must select product categories here. Product under the selected categories here will be displayed.

**Include Subcategory**

If you wants to include sub categories of the above selected categories, then set this option to YES.

**Subcategory level**

If you have enabled include sub categories, then you must have to choose the level of subcategories to include. For example, 3.

#### Select based on product Ids

This option will be used only if you have chosen **Selected products** as your product source. Following steps should have to be done to add specific products to the module:

1. Click on **Add products** button.

2. The popup window will be displayed on the screen. On the popup window, check the box near to the product name.

3. After selecting the products, click on set values button and close the popup window.

4. The products will be added. Save.