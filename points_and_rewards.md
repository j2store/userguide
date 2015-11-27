# Points and Rewards

This app used to give rewards points to user.User can use that points for purchase.

#### Requirements

* PHP 5.2 or higher
* Joomla 3.3 or above
* J2Store 3.2.x or above

#### Installation Instructions
1. Use the Joomla installer to install the app. 
2. In the backend, go to **J2Store Dashboard -> Apps** as shown in the image below. 
![](./assets/images/acymail-app-1.png)
3. Click **Enable** in the Point and Rewards plugin. (type=j2store). 

![](step1_.png)
4. After the app is enabled, click on **Open** to set the configuration for the app.
![](step2.png)
5. Enter the parameters (read the explanation about each parameter given below) 
6. Save and close it.

#### Parameters
The below image illustrates the settings of parameters:

* #### Points Settings
    * ###### Earn Points Conversion rate
         Enter how many points the customers, should earn for each dollar spent.
![](step3_earning_rewards_every_dollar.png)
    * ###### Redeem Points Conversion rate
        Points are earned for purchases based on the conversion rate you set. For example, customers could earn 1 point for every dollar spent.
![](step3_redeem_reward_points.png)
    * ###### Maximum Points Discount 
      you can set Maximum number of points should a customer to, apply discount to his order.
![](maximum_points_discount.png)
    * ###### Points Label 
* #### Product / Cart / Checkout Messages 
    * ###### Single Product Page Message
    You can enter custom message you want to display in the product page about earning reward points on every purchase of the product.
![](product_cart_checkout_messages_1.png)
    * ###### Earn Points Cart Page Message
    You can enter a message you want to display in the cart page about the earning of reward points when the customer complete the order.
![](product_cart_checkout_messages_3.png)
    * ###### Redeems Points Cart Page Message 
    You can enter the redeem points message, So that customer can apply their points to get discount.
![](product_cart_checkout_messages_31.png)
* #### Points Earned for Actions
    * ###### Points Earned for Account Signup
![](set_signup_points.png)
![](singup_and_earn_points.png)
* #### Display Category View Message Options
    * ###### Product Page Message Enable/Disable
    ![](enable_reward_point_info_on_product_page.png)
    
    
#### Custom Tags 
  1. Adjust the message by using **{points}**, **{points_value}** and **{points_label}** to represent the points earned / available for redeemption and the label set for points.
  
  2. **{price_in_points}** tag used for display how much point need for particular product price. so use in Single Product Page Message.
  
#### Front page
Go to J2store Product Shop 
You can see the information displayed about the rewards and points.
![](product_page.png)



#### My Profile
 Go to Myprofile Menu -> Rewards (Tabs)
  
  Here you can see list of points you earned.
  



 