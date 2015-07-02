# AcyMailing Integration App

This app integrates J2Store with AcyMailing to enable option for subscription to newsletters.

#### Requirements

* PHP 5.2 or higher
* Joomla 2.5 or above
* J2Store 3.1.6 or above

#### Installation Instructions
1. Use the Joomla installer to install the app. 
2. In the backend, go to **J2Store Dashboard -> Apps** as shown in the image below. 
![](acymail-app-1.png)
3. Click **Enable** in the Acymailing plugin. (type=j2store). 
![](acymail-app-2.png)
4. After the app is enabled, click on **Open** to set the configuration for the app.
![](acymail-app-4.png)
5. Enter the parameters (read the explanation about each parameter given below) 
6. Save and close it.

#### Parameters
The below image illustrates the settings of parameters:
![](acymailing_config_options.png)

1. **Acymailing List** -
This option is used to display all your Acymailing subscribers list. You can select multiple lists in this option.
![](choose_the_list_from_the_dropdown.png)

2. **Acymailing List Title** -
The text entered here will be displayed when customer is about to select payment method. If you use a muliti-lingual site, language constants can be entered here and then language over-ride can be made.

3. **Auto Subscription** -
If you enable this by choosing **Yes**, then the customer will be automatically added to subscribers' list. A confirmation email will be sent to the customer. All this will be done on successful order placement.

4. **Display Auto subscription in products** -
If you enable this option, then a check box will appear in both the back end and front end. This is to offer product specific subscription. Consider the image below:
![](acymail-app-5.png)
If you check this option, then it will override the previous 'Auto Subscription' option.

### Front end view of Auto Subsctiption

In the front end, if you add your desired product to the cart and proceed to checkout, then you will see the auto subscription status. It will reflect your settings in your product configuration. 

Consider the below image:



























