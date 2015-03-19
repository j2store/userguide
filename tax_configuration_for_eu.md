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




