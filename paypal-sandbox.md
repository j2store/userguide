# PayPal Sandbox

Using the PayPal Sandbox is not even half as intuitive as you might think. Since most of our users think that our software is broken because they are not able to use the Sandbox, we have documented every single step you have to take in order to use the Sandbox on your site.

### A. Signing up for Sandbox access

1. Go to the PayPal Sandbox site [ developer.paypal.com ]

2. Click on Sign Up. Important: do not use your regular PayPal email address to subscribe!

3. You get an email. Click on the link to activate your Sandbox access.

4. Log in to the Sandbox using the email and password you created

#### A.1. Create a seller account

1. Go to the main Sandbox page [ developer.paypal.com/cgi-bin/devscr?cmd=home/main ]

2. Click on Create a preconfigured account
Warning
**MAJOR SUPER DUPER IMPORTANT PITFALL WARNING!!!** Choose a country with the same currency as your site. For example United States for transactions in USD.

3. Set the account type to Seller

4. Optional: set the login email to "seller". It will make it easier for you to remember what you're doing

5. Note down your password. This will not be visible anywhere else.

6. Set Add Bank Account to Yes and set the Account Balance to something like 100.00 USD

7. Click on Create account
Important
Make sure that Payment Review and Negative Test Mode are set to Disabled (that's the default)

8. PITFALL: PayPal will modify your email address, appending a random number and _biz to it. Please verify it at
the Test Accounts section of your Sandbox Account. Note down your email and password, you will need them!

#### A.2. Create a buyer account

1. Go to the main Sandbox page [ developer.paypal.com/cgi-bin/devscr?cmd=home/main ]

2. Click on Create a preconfigured account
Warning
**MAJOR SUPER DUPER IMPORTANT PITFALL WARNING!!!** Choose a country with the same currency as your site. For example United States for transactions in USD.

3. Set the account type to Buyer (not "Buyer In-Store")

4. Optional: set the login email to "buyer". It will make it easier for you to remember what you're doing

5. Note down your password. This will not be visible anywhere else.

6. Set Add Bank Account to Yes and set the Account Balance to something like 1000.00 USD

7. Click on Create account
**Important**
Make sure that Payment Review is set to Disabled (that's the default)

8. PITFALL: PayPal will modify your email address. Please verify it at the Test Accounts section of your Sandbox
Account. Note down your email and password, you will need them!

### B. Set up PayPal plugin for use with PayPal Sandbox

1. Go to Extensions, Plug-in Manager or J2Store > Setup > Payment methods

2. Find PayPal standard for J2Store and edit it

3. Set Sandbox to Yes

4. In the Sandbox Merchant field enter your seller's email address

5. Click on Save & Close

### C. Testing J2Store with PayPal Sandbox

1. Make sure you have at least one published article(product) with price value of AT LEAST 1. Smaller values WILL NOT go through!

2. Go ahead with buying the product

3. When you click Confirm and Make Payment button, Make sure the URL begins with www.sandbox.paypal.com . If not, you are doing something wrong and you have to set up the plugin again.

4. Make sure that in the top left corner you see the name you registered with Paypal Sandbox followed by the words "Test Store". If not, you are doing something wrong and you have to set up the plugin again.

5. Login using the Sandbox buyer email and password and go through with the payment.

6. Go to your site's back-end, Components, J2Store, Orders

7. You can see the order with either a Confirmed or Pending status. If the order with the Pending status had a transaction key, it means PayPal did communicate with your site!

**If order has a pending status**

8. Go back to the PayPal Sandbox site

9. Go to Test Accounts

10. Click on the orange "Enter Sandbox Test Site" button; a new popup window displays

11. Click on Logout. Not the one on the top right, the one right below it.

12. Now click on Log In

13. Log in with your Sandbox seller's email and password

14. If You will see the transaction with a "Payment status" of Unclaimed. Click on the Accept button to its right.

15. It may ask you what to do. If it does, choose the first Accept option and then click on Submit

16. Wait for 1-5 minutes for the payment notification to be sent to your site

17. Go to your site's back-end, Components, J2Store, Orders

18. The order will have confirmed status now. Awesome! You're ready to start selling! Remember to set the plugin's Sandbox to Off and enter your real email address to the Merchant ID field of the plugin. 