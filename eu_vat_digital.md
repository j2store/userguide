# A simplified guide for New EU VAT rules 2015 for digital goods and setting them up in J2Store

* [The New VAT rules](#new_vat_rule)
* [Implementing VAT rules in J2Store](#implement_vat_rule)
	* [EU VAT plugin](#eu_vat_plugin)
	* [Implementation](#implementation)
		1. [Store Configuration](#store_config)
		2. [Tax rule for Home Country](#tax_rule_home)
		3. [Tax rule for an EU Country](#tax_rule_eu)
		4. [Setting up the tax profile](#setting_up_tax_profile)
		5. [Applying tax profile to a product](#apply_tax_profile)
* [Application of VAT rules with Examples:](#application_vat_example)
	* [Example 1](#ex_1)
	* [Example 2](#ex_2)
	* [Example 3](#ex_3)
	* [Example 4](#ex_4)

If you are a seller of digital goods and services, you would probably wondering about the new European VAT rules that came into effect from January 1, 2015.

Since the rules are a bit of pain, we have come up with a simplified guide which will help you implement the new rules easily in your J2Store joomla shopping cart.

<a name="new_vat_rule"></a>
##The New VAT rules

In simple terms, the new VAT rules are:

* if the company sells to any countries in the EU, they will have to charge VAT in the country of the buyer instead of the seller.

* if the buyer of the digital goods is an individual, the company has to charge the VAT percentage from the country of the buyer

* if the buyer of the digital goods is a company (with a valid VAT number), there is a 0 percent VAT charge.

* if the buyer of the digital goods is a company without a VAT number or has an incorrect VAT number, then VAT of the country of the buyer must be charged.

* if the company sells digital goods to companies or individuals in their own country, local VAT needs to be charged.
<a name="implement_vat_rule"></a>

##Implementing VAT rules in J2Store
<a name="eu_vat_plugin"></a>

###EU VAT plugin

We have created a VAT plugin that helps you implement the VAT rules automatically.
Download and install the plugin from here:
[http://j2store.org/extensions/general-plugins.html](http://j2store.org/extensions/general-plugins.html)

Then go to Joomla admin -> Plugin Manager and Enable the EU VAT plugin
<a name="implementation"></a>

###Implementation

>Let us assume that your company is located in : United Kingdom, Bristol
And your home country (local ) VAT is 21 %

<a name="store_config"></a>
**1. Store Configuration**
 Go to Joomla admin – J2Store – Set up – Configuration - Store tab
 
 Set the Default Country to United Kingdom
 Set your Default Zone to Bristol
 
<a name="tax_rule_home"></a>
**2. Tax rule for Home Country**
 First, we should define the geozone and tax rates for the home country, that is the country in which your shop is located.

 **2.1 Define Geozone**

![vat 2015 home geozone](./assets/images/vat_2015_home_geozone.png)

Go to Joomla admin – J2Store – Localization – Geozones – New        

 **Geozone Name:** Home VAT Zone ( It can be anything. It is used just as reference )    
 
   **State :** Published

   **Add country / Zone**

   Choose United Kingdom from the Dropdown list and add it

   Save and close

 **2.2. Define Tax rate:**

![vat 2015 home taxrate](./assets/images/vat_2015_home_taxrate.png)

Go to Joomla admin – J2Store – Localization – Tax Rates – New
        
Name        : Home VAT Rate
Tax Percent    : 21
Geozone     :  Home VAT Zone    
Status     : Published
<a name="tax_rule_eu"></a>

**3. Tax rule for an EU Country**
 Let us take Germany for this example.   Let us say, Germany's VAT charge is:  25 %
 >A few countries might have same VAT rate for the digital goods. You can group them under one geozone.
 
 For this example, I am going to stick with one EU country, that is Germany.

  **3.1 Define Geozone**
  
![vat 2015 customer geozone](./assets/images/vat_2015_customer_geozone.png)

   Go to Joomla admin – J2Store – Localization – Geozones – New
   Geozone Name : Germany VAT Zone ( It can be anything. It is used just as reference )
    State : Published

   Add country / Zone
    Choose Germany from the Dropdown list and add it
>If some other EU countries also implement a 25 % VAT, then you can group them under this geozone itself

   Save and close

   **3.2. Define Tax rate:**
![vat 2015 customer taxrate](./assets/images/vat_2015_customer_taxrate.png)

   Go to Joomla admin – J2Store – Localization – Tax Rates – New

   Name        : Germany VAT Rate
   Tax Percent    : 25
   Geozone     :  Germany VAT Zone
   Status     : Published
   
<a name="setting_up_tax_profile"></a>
**4.Setting up the tax profile**

![vat 2015 taxprofile](./assets/images/vat_2015_taxprofile.png)

It is sufficient to set up ONE tax profile for digital goods, in which we can associate many tax rates.

Go to Joomla admin → J2Store – Localization → Tax profiles → New
    
Tax Profile Name    : Digital Goods Tax Profile
State            : Published

**Tax Rates Mapping**
    
  4.1. Choose Home VAT Rate 21 %  and choose Billing Address as the Associated Address.

  4.2. Choose the Germany VAT Rate 25 %  and choose Billing Address as the Associated Address.

  Save.
  <a name="apply_tax_profile"></a>

**5. Applying tax profile to a product**

![vat 2015 product](./assets/images/vat_2015_product.png)

J2Store uses native Joomla articles as products. So go ahead and create a product.

Go to Joomla admin – Article Manager – New or open your digital product.
    
In J2Store Tab → Item Tax , Choose Digital Goods Tax Profile.


Fill in other relevant fields for your product and save.
<a name="application_vat_example"></a>

##Application of VAT rules with Examples:

Now we have successfully configured the tax rules in J2Store. Let us see how they will get applied for different scenarios
<a name="ex_1"></a>

###Example 1: Buyer  ( can be an INDIVIDUAL or company ) from the same country (Home country )

![vat order same country](./assets/images/vat_order_same_country.png)

Our shop is located in United Kingdom. And the buyer is from the same country. So local tax of 21 percent applies.
<a name="ex_2"></a>

###Example 2: Buyer ( INDIVIDUAL ) from a different EU country (Germany )

![vat order individual eu](./assets/images/vat_order_individual_eu.png)

The buyer is from Germany and he is an Individual customer. So we are charging him the Germany's VAT rate of 25 %
<a name="ex_3"></a>
 
###Example 3: Buyer ( COMPANY ) from a different EU country WITHOUT a valid VAT Number

![vat order invalid vat](./assets/images/vat_order_invalid_vat.png)

The customer is from Germany. He has entered a company name. But his VAT number is INVALID.  So we apply the Germany's VAT rate of 25 %.

(the EU VAT plugin validates the VAT number provided against the EU database )
<a name="ex_4"></a>

###Example 4: Buyer ( COMPANY ) from a different EU country WITH a valid VAT Number

![vat order valid vat](./assets/images/vat_order_valid_vat.png)

The customer is from Germany.  His VAT number is VALID.  So NO tax is applied.
<br>
If you have any questions or suggestions, please post in the [community forum](http://j2store.org/forum/index.html)
