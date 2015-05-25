# SobiPro

### Introduction
This plugin integrates SobiPro directory component with J2Store, thus adding ecommerce capability to Sobipro. 

#### Requirements
* PHP 5.2 or higher
* Joomla 3.x
* J2Store 3 or above
* Sobipro
* Application_j2store_sobipro
* plg_system_spj2store

#### Installation Instructions 
* Note: When you download the Sobipro Plugin You will have the package named "j2store_sobipro_unzip",if you unzip the package you will find to zipped package .These two package are most important and need to be installed and t be enabled.
    
##### Installing System Plugin
1 .Use the Joomla Extension manager to install the plugin the system plugin "plg_system_spj2store". 

2. Enable the the plugin.To enable the Plugin Go to Menu -> Extension Manager->Plugin Manager -> At the left side you can see filter  

##### Installing J2Store Application
1. In the backend, go to Components -> SobiPro -> Application Manager -> Here you can find an input for installing application  “Select Application” Browse to the path "application_j2store_sobipro" file located and select the package for installation.

![](sobipro_step_1.png)

![](sobipro_step_2.png)

![](sobipro_step_3.png)

2. After successful installation, you can now see the list displaying the j2store application.

![](step_6.png)

![](step_7.png)


3. Now choose the section in which you want to enable j2store application.

![](step_8.png)

### Enabling Application in the section
* Click on the Application Sections Tab -> Applications,   you can see the list of applications. Enable the J2Store Application. 

![](step_12.png)

* Now J2Store application is ready.
 
![](step_13.png)

* You can start adding new entries and also treat them as J2Store product by enabling "Treat as product" from the J2Store Tab.

![](step_13_a.png)

Fill the required fields and click "Save and exit". After saving the entry you can see the J2Store Tab having "Treat as product" Controls.

![](step_17_b.png)

Now set "Treat as Product" to 'Yes' and choose the type of the product and click "Save and Exit" once.

![](step_17_c.png)

Now open the Entry. You can see the J2Store Tab having all the fields. Now your product is ready and you can enter the details about the product.

![](step_17_d.png)

Save the changes .

#### Displaying Front end
1. Go to Menus -> Main Menu -> Add New Menu Item and add a menu item. Choose SobiPro Section or Category -> Choose functionality and set other menu parameters, then save.

2. Go to your Front end and click on the menu item you have created. You'll see a category page like this, depending on what choices you have made and what template you are using. Go to the category and click on the entries detail view. You can see the J2Store Cart.

![](final_product_display.png)







