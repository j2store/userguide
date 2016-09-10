# Email Basket Plugin

This plugin allows your customers to email items in the cart to the store owner and to themselves.

The plugin nicely integrates in the default cart page of J2Store. You can ask the customers to provide their name, address or any other information while emailing the cart.

#### Requirements
* PHP 5.2 or higher
* Joomla 2.5.x
* J2Store 2.8.0 or above

#### Installation Instructions
1. Use the Joomla installer to install the plugin.
2. In the backend, go to Extensions->Plugin Manager and open the Email basket
plugin. (type=**j2store**).
3. Enable the plugin
4. Enter the parameters (read the explanation about each parameter given below)
5. Save and close it.

Now you can see the Email Basket button in the cart page.

## Parameters

#### Basic settings

**Disable proceed checkout**

If you set this to YES, the plugin will hide the checkout button in the cart.

**Enable show save cart button**

Set **YES** will display the Save cart button(which is used for un-registerd users) in cart page. Clicking on this button will redirect the customer to register. After registering and loggin in, the cart items remains in the basket.
![](./assets/images/newemail_03.png)

**Empty cart after sending email**

If you set this to YES, the plugin will empty the cart after emailing the cart items to store owner.

**Time delay in milliseconds to empty the cart**

You can set a delay for emptying the cart. Default is 2 seconds.
![](./assets/images/newemail_01.png)

#### Email Configuration

**Send email to Admin**

Set this **YES** will send the email to admin also.

**Email Subject**

Enter the subject of the email here.

**Email Body**

In the Email body section, you can use the shortcodes to display the dynamic information such as customer's name, email, country, cart items, etc..
[first_name]
[last_name]
[email]
[phone_1]
[phone_2]
[company]
[tax_number]
[address_1]
[address_2]
[city]
[zip]
[country_id]
[zone_id]
[cart_item]
[user_name]
[site_name]

To display the custom field information (enterd by the user when filling form) in an email the customer and admin receive, it is possible by adding the shortcode of respective custom field in the Email body editor. For example, if you are having text area as a custom field in your email form, then copy the field name(you can get it in custom field section J2Store > Setup > Custom fields) and paste it in Email body editor. The custom field shortcode should be enclosed with square braces. For example, [message]. Refer the image below,
![](./assets/images/newemail_04.png)

#### Layout

If you would like to add / remove the fields in Email form without affecting checkout form fields, it is possible in this section.

In this section, you can create the custom form by adding field shortcode given in the top of the layout tab page and display that field in the form.

To add any new fields, go to J2Store > Setup > Custom fields. Click NEW to create new field.

Enter the label name, field name, choose field type and set the status to **Published**.

If you don't want to display this new field in checkout and wants to display it only in Email form, then in custom field display settings, set **NO** to all layouts (Checkout billing address layout, Checkout shipping address layout, Checkout payment method layout).

Now, in form layout add the shortcodes of fields you want to display in email form. To add custom field shortcode, copy the field name in J2Store > Setup > Custom fields section and paste it in the form. The field name should be enclosed with square braces. For example, [message].
![](./assets/images/product_quote_08.png)
![](./assets/images/product_quote_06.png)
![](./assets/images/newemail_05.png)

#### Advanced

**Modal box container Inline Style**

You can add the additional inline style to the modal box container in the given text box.

**Modal box container extra class**

You can add the additional class names to the modal box container in the given text box.

**Modal style**

You can add the custom css in the given text area.

**Redirect customer to this URL**

Enter the URL to which the customer should be redirected on the form submission.
![](./assets/images/newemail_02.png)

####Video Tutorial

**[Here is the link](https://www.youtube.com/watch?v=IHpKrQI04Us)** to email basket video tutorial.

#### Support
Still have questions? You can reach us in support@j2store.org

Thank you for using our extension.












