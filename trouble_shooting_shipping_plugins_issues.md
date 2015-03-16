# Trouble Shooting Shipping Plugins Issues


### Troubleshooting USPS, FedEx, UPS and CanadaPost shipping plugins

You have installed the shipping plugin but it doesn't show up during the checkout. Here are a list of reasons that might be preventing the plugin from fetching shipping cost real-time from the APIs of the Shipping carrier.

#### Enable Shipping

Well, this might sound trivial. But some of us often forget to turn on the ***Enable Shipping Switch*** while creating the product. Make sure that Enable shipping is set to YES.

![Enable Shipping](enable_shipping.png)

#### Weight and Dimensions

All the shipping carriers use the weight and the dimension of your product (Length, Width & Height) of your products to calculate the shipping cost (besides using the destination address). So make sure that you enter the Weight and the dimension of your product.

You should select the weight and the length measurement unit from the drop down list.

IMPORTANT for those using UPS: Only KG (Kilogram) and LB (Pound) are supported by UPS as the weight measurement units.  Similarly, only IN (Inch) and CM (Centimetres) are supported as length measurement units. There is a lot more to be taken care of.  If you use Pounds (Lbs) as the weight measurement, then the length measurement should be Inch (In). Similarly, if Kgs (Kilograms) is used, then Centimetre (cm) should be the measurement.

Also, make sure that you choose the correct measurement units in the plugin settings as well. If the measurement units used in the products does not match with the settings in the plugin, then J2Store will attempt to convert the values to the measurement unit set in the plugin.

![Weight and Dimensions](weight_and_dimensions.png)

#### API credentials

All shipping carriers have a web service and provide credentials to access their Rate API. Some of the carriers like USPS offer TEST accounts as well.  Make sure you enter these credentials correctly in the Plugin. Some of the carriers provide Customer number ( like Canada Post ) and a few other parameters as well. Refer the documentation PDF that come with each plugin for more information.

#### Geozone

All the plugins come with a geozone filter setting.

If you choose a geozone, then this shipping plugin will apply only to customers coming from the countries/zones added under the chosen geozone.

During testing, make sure that this parameter is set to All geozones.

![Geozone Setting](shipping_geozone_setting.png)