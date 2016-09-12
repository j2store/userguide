##Troubleshoot Email Issues

####Administrator / customer is not receiving order notification emails

J2Store uses the Joomla's default mail wrapper (JMail) class for sending the order notifications to the store administrator and the customers.

There can be a number of reasons why a customer or the store administration has not received the emails. The following are a few scenarios and solutions.

* ***Is your site in localhost?***

   In this case, you won't receive any emails. Please host your site with a webhosting service provider.
   
* ***Did you set up the 'From' email and Admin email in shop settings***

  **Version 2.x:**
  Go to Joomla admin -> J2Store - Options - Shop settings

  Set your Default From email and the Admin Email there.  IMPORTANT: Make sure that your 'From' email and the Admin email are different.
  
  **For Version 3.x:**
  Go to Joomla admin - Global Configuration - Server tab

  Check your From email and other mail settings.

  Then go to J2Store - Configuration - store settings

  Make sure the Store administrator email is not same as the From email set in the global configuration.

  Many email servers and clients will flag an email as spam if the 'From' email and the admin email are the same.  So using two different emails solves the problem.

  **Example:** If your from email id is: myemail1@gmail.com then your Admin email could be someotheremail@gmail.com
  
* ***What is the status of the order?***

  Most of the Payment Plugins for J2Store are configured to send an order notification to the administrator and the customer, only when the order status is CONFIRMED. However, a few plugins such as Bank transfer, Cash on Delivery, Money Transfer, Offline Payment plugins, will send the notification for all order statuses.

  So if you are not receiving an email, then check the status of the order. Most of the Payment gateways send a feedback after a customer makes a payment successfully. Based on the feedback received, the Payment plugins set the order status and trigger the email. Occasionally, the payment gateways may not send the feedback or it may not reach your server for a variety of reasons. For those reasons, email might not be sent.
  
* ***Mail server issues***

  Sometimes, your host mail server may have issues. It might not send the emails. Here is an easy way to find out if your mail server has an issue:

  Go to Joomla admin -> User Manager. Create a new user by entering a valid email. If you did not receive any notification about the new user creation, then your mail server has an issue.

  Contact your hosting service provider. They will help you out.
  
* ***Customer receiving the email, but the store administrator is not getting or vice versa.***

  If this issue occurs, then J2Store is successfully sending the order notifications using Joomla mail functions. No problems with your Joomla installation.

  The problem is with the customer's or the administrator's email. Ask your customer / store administrator to check their SPAM folders. If still not there, contact your hosting service provider.
  
* ***Is your site hosted in GoDaddy?***

  If you are using GoDaddy as your hosting service provider and did not receive the email, then change the subject of your email template. This broken host introduced unreasonable email filters recently, which prevent sending order notification emails. Refer this **[Thread]( https://www.j2store.org/forum/2-general-questions/5036-solved-order-email-sending-problems-with-godaddy.html)**.

Still have issues ? Post your issues in the community forums if you are a free version user. Subscribers, create a private ticket providing super user logins to your site.