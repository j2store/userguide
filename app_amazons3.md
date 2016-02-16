#Amazon S3#

   The purpose of Amazon s3 app is to sell your files using amazon s3.
   
####Requirments####
* PHP 5.4 or higher
* Joomla 3.3 or above
* J2Store 3.2.x or above

####Installation Instructions
1. Use the Joomla installer to install the app.
2. In the backend, go to J2Store Dashboard -> Apps as shown in the image below.
3. Click Enable in the Amazon S3 app.
4. Once the app is enabled, click on Open to set the configuration for the app.

####Parameters

* ***Access key ID***

     Enter the Access key ID provided by Amazon.
     
* ***Access secret key***

     Enter Access secret key provided by Amazon.
     
     Once you entered Access key ID and Access secret key, save it. You will get your bucket list.

####How to find your AWS Access Key ID and Secret Access Key####

* Login into your Amazon web services account.
* Open the IAM console.
* In the navigation pane, choose Users.
* Choose your IAM user name (not the check box).
* Choose the Security Credentials tab and then choose Create Access Key.
* To see your access key, choose Show User Security Credentials.
* Choose Download Credentials, and store the keys in a secure location.

  Your secret key will no longer be available through the AWS Management Console; you will have the only copy. Keep it confidential in order to protect your account, and never email it. Do not share it outside your organization, even if an inquiry appears to come from AWS or Amazon.com. No one who legitimately represents Amazon will ever ask you for your secret key.
  
* ***Amazon Bucket name***

     Bucket will be listed once you entered Access key ID and Access secret key and save it.
     
* ***Download file time(Min)***

     Set the expiration time to download URL.
     
####How to sell the files using Amazon S3

* Create a downloadable product product and start selling. Create a J2Store product with product type as "Downloadable product". Configure all basic options such as price and navigate to the Files tab.

***Note :*** Make sure you have set path to **Folder path for digital goods** in J2store configuration basic settings.