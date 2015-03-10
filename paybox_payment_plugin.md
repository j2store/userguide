# Paybox Payment Plugin

This plugin integrates Paybox Payment gateway with J2Store.

>IMPORTANT NOTE: Most of the payment options provided by Paybox accept Euro as the currency. So make sure that you create EUR as one of the currencies in J2Store.

#### System Requirements
* PHP 5.3
* Joomla 2.5+
* J2Store 2.6.7+

#### Configuration

The plugin has the following parameters need to be addressed.

**Payment option title**

The value entered here will be used as the title for this payment method. Customer will see this value when he checks out.

**Site Number (PBX_SITE)**

The site number provided by the Paybox

**Rank Number (PBX_R ANG)**

Rank number provided by Paybox

**Rank Number (PBX_IDENTIFIANT)**

Identifier provided by Paybox

**Secret key**

A secret hash provided by Paybox. The value to put in this field can be found in the merchant back office in the information tab in the menu. For individual merchant accounts
you need to follow the procedure to generate your own secret key. For test account, the secret key is fixed and can be obtained from *Paybox*

**Public Key**

A public encryption key provided in the form a certificate. You can download it from the paybox site. We have also attached the certificate downloaded from paybox. Open the file and copy its content to this field.







