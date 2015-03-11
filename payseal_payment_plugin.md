# Payseal Payment Plugin

This plugin integrates the ICICI Payseal Payment gateway with J2Store.

#### Configuration
The following parameters are need to be addressed to configure the payment plugin.

##### Payment Option Title
The value entered here will be used as the title for this payment method. Customer will see this value when he checks out. 

##### Merchant ID
The merchant ID provided by Payseal. 

##### Absolute Path to the directory of key file
Upload the key file provided by the ICICI to a location in your website and enter its absolute path here. Example: You have uploaded the key file to the /home/myaccount/public_html/media folder
Then you should enter:
/home/myaccount/public_html/media

##### Transaction Type
Choose the transaction type. If you choose Authorization, payments from your customers will NOT be credited to your account immediately. You have to go to your ICIC Merchant console and capture the payments.

##### Debug
If you are testing the plugin, you can set this to YES to debug. The debug log will be saved in the cache folder of your Joomla installation.

##### Article ID for Thanks Message
You can create an article with a thank you or instructions or information to the customer and enter its ID here. This will be displayed to the customer when he returns to the site after making payment.
















