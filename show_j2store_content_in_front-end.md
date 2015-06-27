# Show J2Store content in Front-end

This section will help you understand how to display the SEBLOD article in front end.

The display can be achieved in the following methods:

* **Category Blog View**
* **Single Article View**
* **Search & List View**

To display SEBLOD articles in the frontend, you need to create a menu exclusively and then you can display it. 

### Category Blog View
Before you proceed to view the article in frontend, you need to check one thing. Go to **Components -> J2Store -> Setup -> Configuration**. Go to **Cart** tab. Now, check the setting of **Add to cart placement** option. Ensure it is selected with **Within article using tag** as shown in the image below.
![](seblod-cat-blog-cart-tab.png)

To achieve front end category blog view, we need to follow a few procedures as explained below:

#### Create a Menu Item
In the backend main menu, go to **Menus -> Main Menu**. You will get the **Main Menu Items** list, as shown in the image below:
![](seblod-menu-items.png)

Click on the ***Add New Menu Item*** or ***New*** button, as pointed out in the image. You will get the screen as shown in the image below: 
![](seblod-create-new-menu-item-1.png)

Enter a name for the new menu item and click on the **Select** button to select the type of the menu item.
![](seblod-create-new-menu-item-2.png)

As shown in the image, click on the **Articles** and you will get a list down the option. From the new list, select **Category Blog**. Now, you will get a new option below the menu item type, named ***Choose a category***. From that option, select **Product** as illustrated in the next image.
![](seblod-create-new-menu-item-3.png)

#### Edit SEBLOD Form Article Content Section
After you have finished, go to **Components -> SEBLOD 3.x** and in the screen that is delivered, choose **Form & Content Type Manager**. It will give you the screen that is shown in the following image:
![](seblod-j2s-frontend-1.png)

As shown in the image, select the **Intro** tab. Select **All App Folders** and locate **J2Store_Cart**. Add it by clicking on the **'<'** symbol. Now, click on the *pencil* symbol to edit the cart options, as shown in the image below:
![](seblod-j2s-frontend-2-new.png)
You can edit the cart options by changing the text in the field as per your wish, for time being **mainimage|cart**. Save the settings.

Now, go to the front end view of the site. You will get the home page as shown below:
![](seblod-cat-blog-view-1-new.png)

Your home page will display the products in your online store. Note that the new menu item, **Category Blog View** you have created is listed in the main menu list. Click on that and you will get the view as shown in the below image:
![](seblod-cat-blog-view-2-new.png)

### Single Article View

To achieve the single article view, follow the steps, as illustrated in the images below:

![](single-article-view-1.png)

As shown in the image, click select the **Form & Content Types** menu. You will get the screen as shown below:

![](single-article-view-2.png)

Click on the **Article** and you will get the settings and configuration of **Article**. Check for the settings as shown in the next image.

![](single-article-view-3.png)

If the settings match the image above, you are done. If there is no ***J2Store_Cart*** listed on the left side, you can create on using the **+** sign on the right side. Now go to the frontend. All the articles will be listed in the site, as shown in the image below:

![](single-article-frontend-1.png)

You will get all the articles listed here. Click on any one article's name, as shown underlined in the image. You will get the single article view.

![](single-article-frontend-2.png)









