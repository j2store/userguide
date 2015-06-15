# Seblod

### Introduction

The plugin integrates Seblod content construction kit with J2Store, thus adding ecommerce capability to Seblod. 

#### Requirements
* PHP 5.2 or higher
* Joomla 3.x
* J2Store 3 or above
* Seblod 3.x
* Plguin plg_cck_field_j2store

#### Installation Instructions 
Use the Joomla Extension manager to install the plugin.

#### Adding J2Store Field 
1. In the backend, go to Components -> SEBLOD 3.x, as shown in the image below:
![step 1](step-1.png)

2. Click on the icon "Forms & Content Type". Click on the admin menu link "Construction" then "Forms & Content Types".
![Step 2](step-4.png)

3. In the "Form & Content Type Manager", you should click on the item "Article".
![Step 3](step-5.png)

4. Now we have to add j2store custom field to the "Article" content type, click on the "+" (button is placed at the right of the "Contruction"  block). A Form in window popup appears.
![Step 4](step-6.png)

5. To add a "Text" field to an "Article" content type:
![Step 5](step-7.png)

6. Choose App Folder **Seblod**: then choose type "J2store" field.
![](create-article-step-3.png)

7. Save the changes. Now J2store field will appear under the Fulltext field (at the bottom of your form on the first tab).
![](create-article-step-4.png)

8. Save and close the article. 

9. Go to the menu, **Content** -> **Article Manager** -> **Add New Article**. You will get the screen as shown below:
![](add-new-article-1.png)
Now scroll down. You will see the integrated j2store product type as shown below:
![](add-new-article-2.png)

10. The J2Store element appears at the bottom because, it is placed below the End of the Tab in the construction layout. So we need to rearrange the element to appear in the tabs. Consider the below image:
![](rearrange-j2store-element.png)

11. We need to add the J2Store element in the tab. To create a tab panel, click on the + sign in the right side and follow the procedure as shown in the image:
![](create-tab-panel.png)
In the above image, enter the details as shown and click **Save & Close**. The tab panel will be created. You need to rearrange the tab, as shown below:
![](replace-j2storetab.png)
By clicking on the rounded icon, you can confirm the tab panel details and close it.

12. Now, add a new product. You will see the screen like this:
![](create-new-product.png)

13. Now you can Configure your product, Set **Yes** for Visible in store to view at frontend.
![Step 11](step-12.png)

### Displaying Products at Front end

1. To show the product in the frontend, follow the procedure, illustrated with the help of images. In the Control Panel menu, go to **Construction** -> **Forms & Content Types**
![](show-in-frontend-1.png)

2. Now, from the resulting screen, choose **Article** as shown below:
![](show-in-frontend-2.png)

3. Click on the **Site Form** as shown in the image below:
![](show-in-frontend-3.png)

4. In the right hand side, click on the '<' symbol, next to the **J2Store Tab** and it will be added to the form as shown in the below image.
![](show-in-frontend-5.png)

5. After that, in the right side, near the '+' sign, choose 'All App Folders' in the select list and you can see a list of items displayed below. Scroll down to spot **J2Store_Cart** and add it the construction layout, by cliking in the '<' arrow seen in the extreme right of the item. All these actions are illustrated in the image below:
![](show-in-frontend-6.png)
Place the **J2Store Tab** and **J2Store_Cart** items as shown in the image by drag and drop.

6. Go to Joomla admin Control panel -> Choose the Menu -> Menus -> Menu Manager -> Menu Item -> New 

   a.Enter the Menu Title.

  ![](seblod-new-menu-item-0.png)   

   b.Choose the Menu Item type **SEBLOD** -> choose **Forms**.
![](seblod-new-menu-item-1.png)

   c.You will see Search Type input, select **Article** from the  List.
![](seblod-new-menu-item-2.png)

  d. Save the changes.
  
7. In control panel, go to **Construction -> Forms & Content Types** and click on **New**. In the resulting screen, enter the details as shown in the image below:
![](form-content-type-new-1.png)

8. You will get the screen like this, after you have rearranged J2Store Tab. Now, click **Save**



3. click on the Article title to view the product. 
![Step 14](step-14.png)

4. Now you can add the product to the cart. Finally you can see Item added to the Cart.
![Step 15](step-15.png)

 

*** --- CONTENT ADDITION IS UNDERWAY --- ***

 