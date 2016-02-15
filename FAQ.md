#Frequently Asked Questions
####Product Options not working or displaying option
This problem may happen due to Jquery.
Check your j2store basic settings tab in Joomla admin->J2store->setup->configuration.
You might have set Load jQuery UI to only frontend.It should be always in Both frontend and backend.
####Unregistered users to place orders
Go to J2Store - Configuration - Cart settings
set Allow Guest checkout to YES.
####Vat not apears in check out
In Configuration - Tax, tax is set to be applied on the shipping address
In the tax profile, it is set to apply billing address.
####Donation plugin is empty.Why
The donation app adds a Donation option type.
So go to j2store - catalog - options
Create an option. Choose the option type as donation
Save.

Open your product (simple should work good)
go to J2Store Cart - Options
Search for the donation option you just created.
Add it and save.
####Multiple stores / different notification receiver depending on category
J2Store is a B2C solution where you can maintain only one store.
It does not support multi-store system. 
As a result, when an order is placed, all the store administrators will be notified.

If you just want the email notifications to be controlled and made dependent on the category, 
then a custom app could be developed that will send email for the party concerned.
####New Line Characters (\r\n) in Checkout form
Go to Joomla admin - J2Store - Configuration - Checkout Layout
Click the Populate/re-set button and Save
####Shipping Not Working
Make sure about two things
1.Setting under J2Store > Configuration > Store > Weight Unit
![alt tag](http://i.imgur.com/M4k2yE8.png)
2.Setting under Edit Product > shipping tab
The configured shipping rates with shipping rates does has an entry with matching rate.
For eg: In case the item has 829 grams, you have to configure a rate between 800 and 1000 and the estimate shipping lists the rate.
![alt tag](http://i.imgur.com/hwwqoAB.png)
![alt tag](http://i.imgur.com/Dj25Qr4.png)