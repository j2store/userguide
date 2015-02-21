# Tax Profiles

One or more tax rates are grouped to form a tax profile. The tax rates can be customized to tax calculation based on cusotmer's billing address or shipping address or the store's address.

Generally, tax is calculated for billing address. But there are odd cases, where it is calculated for shipping or store address.

Let an example help understand how it works.
This example assumes that the store is located in the state of California, US.

* In the configuration page, go to **Store** tab and create a profile with United States in the country field and California as state
* Now go to geozone pae and create one with a meaningful name of your choice. In this example, it is 'Tax 14'
* Map the country and zone in the fields show below with United States and California

See the image
![Geozone](Geozone.png)

Now create a tax rate in that page by entering the sample data.

Name        : Value Added Tax
Tax Percent : 14.2 (Enter only numbers and a single . for decimal. No other symbols should be used)
Geozone     : 14.2 (Select the geozone from the list)
Status      : Published



















