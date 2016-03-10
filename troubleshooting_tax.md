#Troubleshooting Tax Issues

* **[How to display Prices without including tax?](#price_without_tax)**
* **[How to display prices with including tax?](#price_with_tax)**
* **[Why the tax rate is not showing up for particluar zone?](#zone_not_showing)**
* **[Configured all the things properly but still tax is not showing.Why?](#add_tax_profile)**
* **[Why tax is not displayed when changing the setting of the tax calculation from billing address to the delivery address?](#change_shipping_address)**

<a name="price_without_tax"></a>
####How to display Prices without including tax?

Go to J2store -> Configuration -> Tax tab
Select **No, I will enter prices exclusive of tax** to Prices Entered With Tax option.
Select **Excluding tax** for both Display prices in product pages and Display prices during cart/checkout.

<a name="price_with_tax"></a>
####How to display prices with including tax?

Go to J2store -> Configuration -> Tax tab
Select **Yes, I will enter prices inclusive of tax** to Prices Entered With Tax option.
Select **Including tax** for both Display prices in product pages and Display prices during cart/checkout.
Set **YES** to Display tax information below the prices (in product pages).

<a name="zone_not_showing"></a>
####Why the tax rate is not showing up for particular zone?

For example, do you want to setup the tax rate for california ?

* ***First thing is you have to create Geozone for california***

  Go to J2store -> Localisation -> Geozones and click **NEW** button on top left.
  Enter the Geo Zone Name in the text box.
  Select **Enable**.
  Click on Add Country/Zone button then you will get two dropdowns for choosing country and zone.
  Choose the country name and zone name from the dropdown list.
  Click Save & Close.
  
* ***Add the Geozone to the tax rate you have created***

  Open the tax rate you have created and the geozone you have created will be listed in the Geo Zone list.
  
<a name="add_tax_profile"></a>
####Configured all the things properly but still tax is not showing.Why?

You might have missed one most important step. You should add the tax profile to the product.
Open the product, go to J2store cart and navigate to the general tab.
Add your tax profile created.

<a name="change_shipping_address"></a>
####Why tax is not displayed when changing the setting of the tax calculation from billing address to the delivery address?

If you choose shipping address in J2store configuration then you should also change the associated address to shipping address in the tax profile.

Go to tax profile and set the associate address as shipping address.

