# Inventory

This is a basic inventory management system offered by j2store.

* Enable Inventory

    Set this option to 'Yes' to avail inventory management. While adding an item in k2, provide the available quantity and it will be kept in track whenever an order is processed. Upon successful completion of an order, the order quantity will be deducted from the available quantity and the result will be the new available quantity and when available quantity becomes zero, the add to cart button will be disabled. Also, the user cannot enter a quantity greater than available quantity.
    
* Cancel New/Pending orders to release stock

    Enabling this option by setting it to 'Yes' will cancel the orders with status 'Pending' / 'New', if they were not confirmed within the stipulated time, and the stock will be released and added to available quantity.

* Hold stock for (in minutes) before cancelling

    If the previous option is set to yes, this option will be enabled for entering the allowed time for order confirmation, else, it will stay disabled.