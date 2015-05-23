# Seblod

### Introduction

The plugin integrates Seblod content construction kit with J2Store, thus adding ecommerce capability to Seblod. 

#### Requirements
* PHP 5.2 or higher
* Joomla 3.x
* J2Store 3 or above
* Seblod 3.x
* Plugin plg_cck_field_j2store

#### Installation Instructions 
1. Use the Joomla Extension manager to install the plugin.

#### Adding J2Store Field 
1. In the backend, go to Components -> Seblod, as shown in the image below:

![step 1](step-1.png)

2. Click on the icon ***Forms & Content Type***. Click on the admin menu link ***Construction*** then ***Forms & Content Types***.

![Step 2](step-4.png)

3. In the "Form & Content Type Manager", you should click on the item "Article".
![Step 3](step-5.png)

4. Now we have to add j2store custom field to the ***Article*** content type. To acheive this, click on the **+** button, placed at the right of the ***Contruction*** block. A Form in pop-up window appears.

![Step 4](step-6.png)


5. To add a ***Text*** field to an ***Article*** content type:

![Step 5](step-7.png)

6. Choose App Folder ***Seblod***, then choose type ***J2store*** field.

![Step 6](step-8.png)

7. Save the changes. Now J2store field will appear under the Fulltext field (at the bottom of your form on the first tab).

![Step 7](step-9.png)

8. Now save and close the article. Click on the Add Content Button at the bottom of the page.
 
![Step 8](step-10.png)

9. Now Choose the article Icon from the  pop up window.

![Step 9](step-11.png)

10. Add New Article->, Enter the title and other required fields, Save the article Once. You can Click the J2Store cart Tab -> Set ***Yes*** to **Treat as Product** and choose the type of the product. Save the changes.
 
![Step 12](step-add-product.png)

11. Now you can Configure your product. Set ***Yes*** for Visible in store to view at frontend.

![Step 11](step-12.png)

12. Save the changes.

### Displaying Products at Front end

1.Go to Jooml admin Control panel -> Choose the Menu -> Menus -> Menu Manager -> Menu Item -> New 

   a.Enter the Menu Title.

  ![Step 1.a ](step-16-a.png)    

   b.Choose the Menu Item type "Seblod" -> choose " List & Search".
   
![Step 2.a](step-16-b.png)

   c. You will see Search Type input, select Articles from the  List.
   
![step 16-c](step-16-c.png)

  d. Save the changes.
  