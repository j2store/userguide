# Postal Code Shipping Plugin

The plugin integrates a postal code based shipping method for J2Store. It will calculate the shipping cost based on the postal code range, weight range and quantity range. You can use all three or just one of them.

### Requirements 
* PHP 5.3+ 
* Joomla 2.5 / 3.x + 
* J2Store 2.6.8 + 

### Installation 

You can install the plugin through the standard Joomla installer. 

### Configuration 

#### Shipping Method name
Enter a name for this shipping method. This is what your customers will see at the checkout.

#### Tax Class 
The value selected will be used in calculating tax rates.

#### Enabled
The value  selected  yes will enable the shipping plugin while displaying in the checkout.

#### Geo zones
Choose geozones for which this shipping method is available. Choose at least one.

#### Override Shipping Method
If you set this to Store address, then the shipping address provided by the customer will be ignored for calculating rates and shipping rates will be calculated based on store address.

#### Min SubTotal
If you enter a value here, then this method will apply only if the order subtotal is greater than or equal to the value.
	
#### Max SubTotal
The shipping method will apply only if the order subtotal is less than or equal to the value entered here. 

>Enter -1 to turn off this filter


#### Postal Code Format

Choose the postal code format. Most of the countries follow the US based zip codes.
**Example**: 95100 to 95300

Quite a few commonwealth countries including **UK**, follow a different post code system. 

If you are not sure about post code, do not select any format here.

After saving the plugin, click Set Rates link to set the rates.
#### Geozone
You can select a geozone and restrict the availability of this shipping method to the countries/zones in that geozone. Leave empty / un-selected for making this shipping method available to customers from all regions. 

#### Debug
If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. 

>Set this to NO in Live websites. 

#### Support 
You can contact ***support@j2store.org*** if you have any questions. 