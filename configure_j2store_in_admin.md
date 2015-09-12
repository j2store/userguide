# Configure J2Store in admin

In this section, you will see how to create a SEBLOD article in the backend and frontend.

#### Adding J2Store Field 
1. In the backend, go to Components -> SEBLOD 3.x, as shown in the image below:
![step 1](./assets/images/./assets/images/step-1.png)

2. Click on the icon **Forms & Content Type**. Click on the admin menu link **Construction** then **Forms & Content Types**.
![Step 2](./assets/images/step-4.png)

3. In the **Form & Content Type Manager**, you should click on the item **Article**.
![Step 3](./assets/images/step-5.png)

4. Now we have to add j2store custom field to the **Article** content type, click on the "+" (button is placed at the right of the **Contruction**  block). A Form in window popup appears.
![Step 4](./assets/images/step-6.png)

5. To add a **Text** field to an **Article** content type:
![Step 5](./assets/images/step-7.png)

6. Choose App Folder **Quick Folder**: then choose type **J2store** field.
![](./assets/images/create-article-step-3.png)

7. Save the changes. Now J2store field will appear under the Fulltext field (at the bottom of your form on the first tab).
![](./assets/images/create-article-step-4.png)

8. Save and close the article. 

9. Go to the menu, **Content** -> **Article Manager** -> **Add New Article**. You will get the screen as shown below:
![](./assets/images/add-new-article-1.png)
Now scroll down. You will see the integrated j2store product type as shown below:
![](./assets/images/add-new-article-2.png)

10. The J2Store element appears at the bottom because, it is placed below the End of the Tab in the construction layout. So we need to rearrange the element to appear in the tabs. Consider the below image:
![](./assets/images/rearrange-j2store-element.png)

11. We need to add the J2Store element in the tab. To create a tab panel, click on the + sign in the right side and follow the procedure as shown in the image:
![](./assets/images/create-tab-panel.png)
In the above image, enter the details as shown and click **Save & Close**. The tab panel will be created. You need to rearrange the tab, as shown below:
![](./assets/images/replace-j2storetab.png)
By clicking on the rounded icon, you can confirm the tab panel details and close it.

12. Now, add a new product. You will see the screen like this:
![](./assets/images/create-new-product.png)

13. Now you can Configure your product, Set **Yes** for Visible in store to view at frontend.
![Step 11](./assets/images/step-12.png)

### Product Creation in Front end

1. To create the product in the frontend, follow the procedure, illustrated with the help of images. In the Control Panel menu, go to **Construction** -> **Forms & Content Types**
![](./assets/images/show-in-frontend-1.png)

2. Now, from the resulting screen, choose **Article** as shown below:
![](./assets/images/show-in-frontend-2.png)

3. Click on the **Site Form** as shown in the image below:
![](./assets/images/show-in-frontend-3.png)

4. In the right hand side, click on the '<' symbol, next to the **J2Store Tab** and it will be added to the form as shown in the below image.
![](./assets/images/show-in-frontend-5.png)

5. After that, in the right side, near the '+' sign, choose 'All App Folders' in the select list and you can see a list of items displayed below. Scroll down to locate **J2Store_Cart** and add it to the construction layout, by cliking in the '<' arrow seen in the extreme right of the item. All these actions are illustrated in the image below:
![](./assets/images/show-in-frontend-6.png)
Place the **J2Store Tab** and **J2Store_Cart** items in the positions, as depicted in the image by drag and drop.

6. Go to Joomla admin Control panel -> Menus -> Menu Manager -> Add New Menu

   a.Enter the Menu Title.

  ![](./assets/images/seblod-new-menu-item-0.png)   

   b.Choose the Menu Item type **SEBLOD** -> choose **Forms**.
![](./assets/images/seblod-new-menu-item-1.png)

   c.From **Content Type (Form)** input, select **Article** from the  List.
![](./assets/images/seblod-new-menu-item-2.png)

  d. Save the changes.
  
7. In control panel, go to **Construction -> Forms & Content Types** and click on **New**. In the resulting screen, enter the details as shown in the image below:
![](./assets/images/form-content-type-new-1.png)

8. You will get the screen like this, after you have rearranged J2Store Tab. Now, click **Save**
![](./assets/images/form-content-type-new-2.png)

9. Thats it. You have successfully created a SEBLOD article. You can choose it in the following ways.
    
    I. Click on the **Add Content** as shown in the following image. 
![](./assets/images/new-form-content-type-listed.png)
If you click on the **Add Content** you will get this pop-up window:
![](./assets/images/add-content-clicked.png)

  II. In main menu, go to **Content -> Article Manager** and click on the **New** button as shown below:
![](./assets/images/article-manager-list.png)
You will get the pop-up like this:
![](./assets/images/article-manager-list-new.png)

10. But before you add an article in this type, you need to do edit the article you have created further. Open it for editing.
![](./assets/images/edit-form-article.png)
Still you need to follow some more steps to complete the procedure. Arrange the items in the construction layout as shown in the image below:
![](./assets/images/form-article-final-setting.png)

11. Now, **Save** the page and create an article of type **Form_Article** and you will have the product creation page like this: 
![](./assets/images/form-article-new-product-details.png)
![](./assets/images/form-article-j2store-tab.png)


**The images below illustrates how to create a product in your frontend**

In your site frontend, you can see the newly created SEBLOD article, listed in the top right. See the image:

![](./assets/images/frontend-article-creation-1.png)

As shown in the image, click on the **New Article** and you will get the product creation page as shown in the next image. Enter a name for the new product and content for the product. This is **Contents** tab. Now, go to **J2Store** tab. Here, select **Yes** to ***Treat as a product*** option and now click on **Save**. 

![](./assets/images/frontend-article-creation-2.png)

![](./assets/images/frontend-article-creation-3.png)

Your product is created and you can configure the product with the product specific details, change the product type, set prices, etc.