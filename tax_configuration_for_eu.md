# Recommended Tax configuration for EU Stores

This guide will walk you through the configuration of tax in J2Store for EU stores. This is an example configuration for stores in Europe. For detailed information on tax, please consult an expert.

**Important:** No guarantee is offered with respect to any of the information given here. Please contact an expert before you take any decisions about tax matters

>NOTE:The example assumes you have a store in Germany and you charge 19% tax on the goods. All customers coming originating from Germany are charged with 19 % of tax.


#### Step 1 : Create a geozone for base rates (home country tax)

Go to Localisation -> Geozones -> New

**Geozone Name:** Base rates

**Country :** Germany

**Zones :** All

#### Step 2: Create a tax rate

Go to Localisation -> Tax Rates -> New

**Name :**  VAT

**Tax Percent :** 19

**Geozone :** Base rates

**Status :** Published

#### Step 3: Create a tax profile and rules

Go to Localisation -> Tax Profiles -> New

**Name:** Base Tax Profile
**Enabled:** Yes

**Tax rules**

Click Add 

**Rate:** VAT
**Associated Address: ** Shipping

![taxprofile](Selection_033.png)


#### Step 4: Configure tax settings

Go to Set up -> Configuration -> Tax

**Prices Entered with Tax:** Yes, I will enter prices with tax
**Calculate tax based on:** Shipping address
**Default Customer address:** Store address
**Display prices in product pages:** Including tax
**Display prices in cart / checkout :** Including tax
**Apply discounts :** After tax

Save.

#### Step 5: Create a product and choose the tax profile

J2Store uses Joomla articles as products. So go to Article Manager and create a New Article / Product (If you sue any other catalog source like Zoo or Sebold, you should head there). 

Product creation steps are explained under the topic **Products**
Here let us just see how to choose the tax profile

Go to J2Store Cart tab -> General tab 

**Tax Profile :** Base tax profile
![](Selection_035.png)

**IMPORTANT**: If you do not choose the tax profile, then tax will not apply in the store front.


### Step 6: Selling in multiple countries with multiple tax rates

If you are selling your products to other countries in Europe, then there are three scenarios

* Charge the same VAT rate for customers from certain countries 

    In this case, you will just have to open the Base Geozone and add the countries / zones to which you want to charge 19%. Then all customers from all those countries will be charged with the 19% tax rate.
    
* Charge different VAT rate for customers from certain countries

    Let us say, you want to charge 12 % tax for customers from Switzerland and France
    
    1. Create a new Geozone and include Switzerland and France
    
    2. Create a new tax rate and set the tax percent to 12 %
    
    3. Go to Localisation -> Tax Profiles -> Open Base tax profiles
    Under Tax rules, Click add
    Choose your New tax rate and associate it to the Shipping address.
    Save.
    
    Now customer from Switzerland and France will be charged with 12 % of tax instead of your base rate of 19 %