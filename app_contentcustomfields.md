# Content Custom Fields

To specify more information about your product, you might be  using the description part of the product page. Generally, the description part will be displayed at the bottom of the product page after the title, price and the cart button. What if you wish to display text somewhere else apart from the description part?

Well, of course, you might consider using special module positions or publishing custom html modules. Some might even think of trying overrides. But in these cases, the text would be static.
But, when you want the content to be dynamic, how to you achieve this?

Here are the steps to be done:
 * Create Joomla fields.
 * Download and install the app Content Custom fields.
 * Configure the app by choosing where the content has to be displayed.
 * Specify the content in the Fields tab of your product article and insert the shortcode for field in the content section of the article.

## Create Joomla fields
  Joomla custom fields can be created by carrying out the following steps:
  * Navigate to Content->Fields->New.
  * We are going to specify text in our product page. So the Field type must be set to Text.
  * Give the field a name, description, label and other details.

  **Screenshot**
    ![](./assets/images/app_contentcustomfieldscreatingfields.png)

## Download and install the app Content Custom Fields

  * The app can be downloaded from our site and installed using the default joomla installer.s
  * Post installing the app, it has to be enabled under J2Store->Apps.

  * NOTE: The app helps you display the Joomla 3.7 content fields (custom fields) in the product description. Works only in the single product view.


## Configure the app

  *  **Display content fields using**

    Choose where the custom field has to be displayed. The available options are:
        * Field Shortcode(If this is chosen, then the shortcode has to be specified in the product article). Setting chosen here affects the next option.
        *  Display all the fields at the end of product description
        * Before price
        * After price
        *  Before add to cart button
        * After add to cart button

* **Display fields in long/short description**

    Choose if the content should appear in the long description or the short description part of the page. This option is applicable only if the type chosen in the previous Setting is Field short code.

* **Display layout**

   Select the layout in which the custom field should appear:
    * Product view only- In the individual product view or item view.
    * Category view only- In the product list view or the category view.
    * Both views- In the product list view as well as in the item view.
    * Hide display content in layout- To hide the content in both views.

* **Enable Accordion style**

  Choose the mode of display of the fields, either as an accordion or in the normal mode.

* **Category view fields**

  Select the fields that have to be displayed in the category view or the list view.

* **Product view fields**

 Select the fields that have to be visible in the item view or the product view.

 **Screenshot**

 ![](./assets/images/app_contentcustomfieldsconfiguration.png)

# Specify the content and insert shortcode in the product article

 * Edit the product article. Navigate to the fields section and mention the content that has to be displayed in the product page.

 * Move to the content tab of the article and click on the field option and choose the field that has been created for this.

 ![](./assets/images/app_contentcustomfieldsprofield.png)

![](./assets/images/app_contentcustomfieldsprocontent.png)

![](./assets/images/app_contentcustomfieldsfront.png)
