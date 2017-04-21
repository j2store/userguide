## HOWTO create a custom thank you message

You can display a thank you message, instructions or information to your customers after they have completed the purchase. For example, if you are selling digital goods, you can include a link where the customer can download the items.

if you are using offline payment, then you can include instructions or bank account details in the article and display it to the customer. You can use this feature on a number of ways.

#### Step 1: Create an article

Go to Joomla admin -> Article Manager.

Create a new article and enter your message, instructions or information or any text that you want to show to the customers after the purchase.

Save the article and note down its ID.

#### Step 2: Associating the article with the Payment Plugins

All the J2Store payment plugins have a feature to display an article after the customer makes the payment and completes the purchase.

Let us take the offline Payment Plugin as an example.

Go to Plugin Manager and open the Offline Payment Plugin.

In the Basic Options tab, you will find a param: Custom thank you Article ID

(in Joomla 2.5, you can see the plugin params on the right side of the screen)

Enter the ID of the article you just created with a message to the customer.

Save and close the plugin.

Thats it! When a customer checks out and completes the purchase, he will see this article.

**TIP:** If you use more than one payment plugins, then you have to open other plugins and enter the article ID. You have the option to enter a different article ID for different payment plugins.