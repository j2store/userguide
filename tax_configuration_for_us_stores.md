# Recommended Tax configuration for US Stores

This is an example setting for stores in United States. This also applies to many other countries that follow a US style of tax system. For detailed information on tax, please consult an expert.


**Note:** Current US law requires you to collect taxes where you have an interest/ongoing concern — that is, where you have physical stores, distribution centers, headquarters, and so on. For many online stores this is only one location. However if you have stores that operate in many states or countries, or if you have revenues exceeding approximately $2M per year, we recommend that you use a third-party tax provider because there can be a considerable number of tax rules and tax zones to manage.

**Important:** No guarantee is offered with respect to any of the information given here. Please contact an expert before you take any decisions about tax matters

**NOTES:**

The example assumes you have a store in Texas and you charge 8.5% tax on the goods sold to customers in Texas. All customers coming from other states are NOT taxed


#### Step 1 : Create a geozone for Texas

Go to Localisation -> Geozones -> New

**Geozone Name:** Texas Zone

**Country :** United States

**Zones :** Texas

#### Step 2: Create a tax rate

Go to Localisation -> Tax Rates -> New

**Name :**  Sales Tax (you can give any name here)

**Tax Percent :** 8.25

**Geozone :** Texas Zone

**Status :** Published

#### Step 3: Create a tax profile and rules

Go to Localisation -> Tax Profiles -> New

**Name:** Default Tax Class
**Enabled:** Yes

**Tax rules**

Click Add 

**Rate:** Sales Tax
**Associated Address: ** Billing


Step 4: Configure tax settings

Go to Set up -> Configuration -> Tax

**Prices Entered with Tax:** No, i will enter prices EXCLUSIVE of tax
**Calculate tax based on:** Shipping address
**Default Customer address:** Store address
**Display prices in product pages:** Excluding tax
**Display prices in cart / checkout :** Excluding tax
**Apply discounts :** Before tax

Save.

Step 5: Create a product and choose the tax profile

J2Store uses Joomla articles as products. So go to Article Manager and create a New Article / Product (If you sue any other catalog source like Zoo or Sebold, you should head there). 

Product creation steps are explained under the topic **Products**
Here let us just see how to choose the tax profile

Go to J2Store Cart tab -> General tab 

**Tax Profile :** Default tax class
![](Selection_036.png)
**IMPORTANT** If you do not choose the tax profile, then tax will not apply in the store front.