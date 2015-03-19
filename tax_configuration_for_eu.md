# Recommended Tax configuration for EU Stores

This is an example setting for stores in Europe. For detailed information on tax, please consult an expert.

This guide will walk you through the configuration of tax in J2Store for EU stores.

**Important:** No guarantee is offered with respect to any of the information given here. Please contact an expert before you take any decisions about tax matters

NOTES:

The example assumes you have a store in Germany and you charge 19% tax on the goods. All customers coming originating from Germany are charged with 19 % of tax.


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


Step 4: Configure tax settings

Go to Set up -> Configuration -> Tax

**Prices Entered with Tax:** Yes, I will enter prices with tax
**Calculate tax based on:** Shipping address
**Default Customer address:** Store address
**Display prices in product pages:** Including tax
**Display prices in cart / checkout :** Including tax
**Apply discounts :** After tax

Save.

Step 5: Create a product and choose the tax profile

J2Store uses Joomla articles as products. So go to Article Manager and create a New Article / Product (If you sue any other catalog source like Zoo or Sebold, you should head there). 

Product creation steps are explained under the topic **Products**
Here let us just see how to choose the tax profile

Go to J2Store Cart tab -> General tab 

**Tax Profile :** Base tax profile
![](Selection_035.png)
**IMPORTANT** If you do not choose the tax profile, then tax will not apply in the store front.








