# Inventory

#### *This is a J2Store PRO exclusive feature*

This is a basic inventory management system offered by j2store.

* ***Enable Inventory***

    Set this option to **'Yes'** to enable inventory management. Provide the available quantity when a product is added and it will be kept in track whenever an order is processed. Upon successful completion of an order, the product quantity will be deducted from the available quantity and the result will be the new available quantity and when available quantity for a particular product becomes zero, the add to cart button will be disabled. Also, the user cannot enter a quantity greater than available quantity.
    
* ***Cancel New/Pending orders to release stock***

    Enabling this option by setting it to **'Yes'** will cancel the orders with status **'Pending' / 'New'**, if they were not confirmed within the stipulated time, and the stock will be released and added to available quantity.

* ***Hold stock for (in minutes) before canceling***

    If the previous option is set to yes, this option will be enabled for entering the allowed time for order confirmation, else, it will stay disabled.

* ***Stock Display Format***    

    This option is used to display the available stock. There are three formats available for the view.
    1. Always Show Stock e.g., 12 in stock.
    2. Show only when stock reaches low stock threshold. e.g., only 2 left in stock.
    3. Never show stock.

* ***Min Sale Quantity***

    This global setting default value is 1 and it can be overwritten for user's desired quantity in products view.

* ***Max Sale Quantity***

    Global setting. By default, it is left empty. It can also be overwritten.

* ***Notify if stock goes below***

    The global setting for this field is empty and it can be overwritten for the user's desired quantity. And when the stock goes beyond the preset level it will be notified.
    
Check the image below for a clear understanding.

![Inventory Setup](Inventory_setup.png)
