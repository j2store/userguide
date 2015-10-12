#Setting up European VAT rules for selling physical goods with J2Store

* [The VAT rules are:](#vat_rules)
* [Implementing VAT rules in J2Store](#implement_vat_rules)
	* [Store Configuration](#store_configuration)
	* [Geozone](#geozone)
	* [Tax rate](#tax_rate)
	* [Setting up the tax profile](#setting_tex_profile)
	* [Applying tax profile to a product](#apply_tax_product)

Setting up the European VAT system in J2Store is relatively easy.  We have created a plugin that automatically validates the VAT number and helps you apply the rules.

This guide walks you through the tax configuration for EU.
<a name="vat_rules"></a>

##The VAT rules are:

* Home country's residents & businesses are charged VAT (Home country's rate. That is, the rate defined by you in the Tax Profile)

* EU residents & businesses with no valid VAT number will be charged VAT (Home country's rate, That is, the rate defined by you in the Tax Profile)

* EU (Non Home country) and with a valid VAT number are charged 0% VAT

* Non EU residents & businesses are charged 0% VAT
<a name="implement_vat_rules"></a>

##Implementing VAT rules in J2Store

We have created a VAT plugin that helps you implement the VAT rules automatically.
Download and install the plugin from here:
[http://j2store.org/extensions/general-plugins.html](http://j2store.org/extensions/general-plugins.html)

Let us assume that your company is located in : United Kingdom, Bristol
And your home country (local ) VAT is 21 %
<a name="store_profile"></a>

###Store Profile

Go to Joomla admin – J2Store – Set up – Configuration - > Store tab.

Set the Default Country to United Kingdom
Set your Default Zone to Bristol
<a name="geozone"></a>

###Geozone
Go to Joomla admin – J2Store – Localisation – Geozones – New
    
Geozone Name : VAT Zone ( It can be anything. It is used just as reference )
State : Published

Add country / Zone
Choose United Kingdom from the Dropdown list and add it

** IMPORTANT: According to the rule, EU residents & businesses with no valid VAT number has to be charged based on the home country's rate. **

** So it is advised that you add all the EU countries in this geozone itself. Choose EU Vat countries and add them. Refer this article to know all EU VAT countries. [http://en.wikipedia.org/wiki/European_Union_value_added_tax](http://en.wikipedia.org/wiki/European_Union_value_added_tax) **


(You can also add all other European countries. or create a separate geozone. But then you will have to create tax rate and map that in the tax profile. Kind of a double work!).

   Save and close

###Tax rate
<a name="tax_rate"></a>

Go to Joomla admin – J2Store – Localisation – Tax Rates – New
        
Name        :  VAT Rate
Tax Percent    : 21
Geozone     :  VAT Zone    
Status     : Published
<a name="setting_tex_profile"></a>

###Setting up the tax profile

It is sufficient to set up ONE tax profile


Go to Joomla admin → J2Store – Localisation → Tax profiles → New
    
Tax Profile Name    : My Tax Profile
State            : Published

**Tax Rates Mapping**

1. Choose VAT Rate 21 %  and choose Billing Address as the Associated Address.

Save.
<a name="apply_tax_product"></a>

##Applying tax profile to a product

J2Store uses native Joomla articles as products. So go ahead and create a product.

Go to Joomla admin – Article Manager – New or open your digital product.
    
In J2Store Tab → Item Tax , Choose My Tax Profile.


Fill in other relevant fields for your product and save.     