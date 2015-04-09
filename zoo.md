# Zoo

### Introduction

The plugin integrates Zoo content construction kit with J2Store, thus adding ecommerce capability to zoo. 

#### Requirements
* PHP 5.2 or higher
* Joomla 3.x
* J2Store 3 or above
* Zoo 

#### Installation Instructions 
1. Use the Joomla Extension manager to install the plugin. 

2. In the backend, go to Components -> Zoo. Click on the Setting Icon.
 
![Control Manager](ctrl_manager.png)

Let us say, you want to treat a Blog item as product. (Zoo has a number of other content types as well. Blog content type is taken as an example )

3. Edit the Blog -> Article -> Click Edit Elements

![](app_config.png)
![](step_1.png)

	
Here you can see **JTwoStore**  element in the list. (Numbers seems not working. That is why J2Store has become JTwoStore:-) )
  
![](step_2.png)
	
Now click on the element, you can see JTwoStore element added to the article element list(see Left Side).
 
![](step_3_up.png)

You have to enter the name of the element to display in the article item. Enter as J2Store as the name and Shopping cart as the description. Now save the changes.	

4. Click on the new button -> Click Article

![](create_new_article.png)

![](step_4.png)

5. Enter the Title to the article and other required fields .

![](new_item_before_save.png)

6. Enter the required fields and Save once. After successfully saved, you can see the Jtwostore Element added to your item.

![](new_item_after_save.png)

7.Now in Treat as Product, select **Yes** -> select the type of the product 

IMPORTANT: Click **Save**. Only then you can see the product related fields.

 ![](enable_product_choose_product_type.png)

After save, you will able to see **J2Store cart** tab there and you can enter the details about the product.

 ![](step_6.png)

Save changes.

#### Frontend Customization Instructions
1. In the backend, go to Components -> Zoo, click on the Setting Icon on

![](ctrl_manager.png)

2. Now edit the Blog -> Article - > your template layout-> click the Full layout   

  ![](front_end_adding_element_layout.png)

3. Now you can see J2Store Cart in the layout list, you have to drag the J2storecart from the right to the left side in your desired area. 

![![](step_7.png)](step_final.png)

4. Save changes.
		
5. To see Cart at front end, create Zoo Menu Item for the Zoo Articles.

Click on the article that you have enabled as product, you can able to see J2store Cart. 
