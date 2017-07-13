# Sagepay Payment Plugin

The SagePay Plugin enables you to receive payments via SagePay Payment Gateway. Getting a SagePay account is very easy. Look at more about SagePay here http://www.sagepay.com/

NOTE: The Plugin uses the Direct Integration method of the SagePay. Please refer the link to learn more about this integration method in  http://www.sagepay.com/help/userguides/590 

#### Requirements
* PHP 5.2 or higher
* Joomla 2.5.x
* J2Store 1.0 or above 

#### Installation Instructions 

1. Use the Joomla installer to install the plugin. 

2. In the backend, go to Extensions->Plugin Manager and open the SagePay Payments plugin (type=**j2store**). 

3. Enable the plugin 

4. Enter the parameters (read the explanation about each parameter given below) 

5. Save and close it. 

Now you can see the SagePay Payments as an option during the Check out process. 

#### Parameters

##### SagePay Vendor Name
This is your  Vendor/Merchant name provided by the SagePay

##### SagePay Encryption Password
While signing up for SagePay account, you will be given a unique Encryption password. Please enter the pass here.

##### Use SSL to post back to SagePay?
If you are using SSL certificate (https), enable this. If you dont know what SSL is better leave it as No 

##### SagePay Test Server
SagePay offers a testing suite called Simulator. Before going live, it is advised to test your store using the SagePay's test server. Read more about SagePay test server http://www.sagepay.com/developers. 

>NOTE: To receive payments (except during testing), you dont have to enable this. IN LIVE SITE, THIS SHOULD BE SET TO NO. 

##### Thanks Msg Joomla Article ID
You can create a Joomla Article to say thanks to the users, who purchased in your online store. Enter the article ID here.

#### Support
Still have questions? You can post your questions in our support forum: http://j2store.org/forum/index.html

Thank you for using our extension.












