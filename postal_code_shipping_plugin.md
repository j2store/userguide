# Postal Code Shipping Plugin

The plugin integrates a postal code based shipping method for J2Store

### Requirements 
* PHP 5.3+ 
* Joomla 2.5 / 3.x + 
* J2Store 2.6.8 + 

### Installation 

You can install the plugin through the standard Joomla installer. 

### Configuration 

#### Method name
Enter a name for this shipping method. This is what your customers will see at the checkout.

#### Postal codes and rates
You can enter the postal codes and rate in a comma separated format. **Example**: 95100=10.00, 95101=15.00 i.e., postcode=rate, postcode=rate

#### Geozone
You can select a geozone and restrict the availability of this shipping method to the countries/zones in that geozone. Leave empty / un-selected for making this shipping method available to customers from all regions. 

#### Debug
If you set this to yes, then debug messages will be logged and saved in the cache folder in your Joomla root directory. 

>Set this to NO in Live websites. 

#### Support 
You can contact ***support@j2store.org*** if you have any questions. 