# Checkout Layout

In this tab, the checkout layout can be set.

* ***Checkout Billing Address Layout***

    This option helps to include/exclude the required fields in the layout of Billing Address. For e.g.,
    <div class="row-fluid">
		<div class="span6">[first_name] [last_name] [phone_1] [phone_2] [company] [tax_number]</div>
		<div class="span6">[address_1] [address_2] [city] [zip] [country_id] [zone_id]</div>
		</div>
    Like this any html code can be added here for one's desired layout.
    
* ***Checkout Shipping Address Layout***

    This option helps to include/exclude the required fields in the layout of Shipping Address.
    
* ***Checkout Payment Method Layout***

    This option is to decide which fields are required in the layout for the Payment Method while checking out.
    
* ***Pre-populate / Restore***

    This is a button, that restores the default setting of all the three options given above, when clicked.
    
For a better understanding, check the image below:

![](./assets/images/checkout_layout.png)
    
    
### Example to add a custom field
Assume that it would be better to add a **Title** field before the **First Name**. To achieve that, create a custom field with *title* as its name, as shown in the image:

![](./assets/images/custom-field-creation.png)

After that, the custom field has to be added to the layout settings in configuration. Go to **J2Store -> Setup -> Configuration** and select **Checkout Layout** tab.Then add the tag for the newly created custom field in the position of the desired display area. Save and close.  Check the image below:

![](./assets/images/add-cus-field-to-layout.png)

Now, in the checkout process, the added custom field **Title** will be displayed before the **First Name** field, as illustrated in the following image:

![](./assets/images/custom-field-in-frontend.png)

In this way, new custom fields can be added according to the needs of the user.