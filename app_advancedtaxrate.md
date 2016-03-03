#Advanced Tax Rate
The purpose of this app is to create the advanced tax rate. It will help you to set the tax rate for individual postal code.
####Requirements
 * PHP 5.4 or higher
 * Joomla 3.3 or above
 * J2store 3.2.x or above

####Installation Instructions

1. Use the joomla installer to install the app.

2. In tha backend, go to **J2store Dashboard -> Apps**.

3. Click enable in the Advanced tax rate app.
![](assets/images/advancetax_enable.png)
4. Once the app is enabled, click an open to set the configuration for the app.

####Configuration

Once you opened the app, you will get the screen like below. Click **New** on top left.
![](assets/images/advancetax_new.png)

* ***TaxClass Name***

  Enter the name of the tax class here.
  
* ***Enabled***

  You should select enabled to enable the tax class and save.
  ![](assets/images/advancetax_addtax.png)
  Once saved, you will get the button named with **View taxrates**. Click on the button will show you the pop screen where you have to set tax rate for specific country,zone and postal code.
  ![](assets/images/advancetax_viewtax.png)
  
####Parameters in creating Tax rate
  **Country & Zone:** Choose the country and zone available from the dropdown list.
  
  **Postal code:** Tax will be added to the sub total when the customer's postal code matches the postal code added here.
  
  **Address type:** Tax will be applied based on the address type you chosen here.
  
  **Tax Rate:** Give your tax rate(like 8.5%, 9.5%)
  
  **Name:** Name added here will be displayed in the frontend.(For example, if you add the name as Tax rate califonia, then in frontend it will display like **Tax rate california(8.5%)**)
  
  **Priority:** Set the priority and click create button.
  ![](assets/images/advancetax_taxrate.png)
  
**Note:** You can also choose import and export to import the tax and export the tax as CSV file.
  
####Support

Still have questions? You can post in our support forum: http://j2store.org/forum/index.html

Thank you for using our extension.