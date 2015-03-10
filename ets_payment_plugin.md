# ETS Payment Plugin

This plugin integrates J2Store with ETS Payment Gateway (Hosted payment).

#### Requirements

The minimum requirements for this plugin to be installed is as follows:
* PHP 5.2 or higher
* Joomla 2.5 or above
* J2Store 2.7.3 or above

#### Installation Instructions:
1. Use the Joomla installer to install the plugin.
2. In the backend, go to Extensions->Plugin Manager and open the ETS Payments plugin. (type = **j2store**).
3. Enable the plugin.
4. Enter the parameters (read the explanation about each parameter given below).
5. Save and close it. 

#### Parameters
**Payment option title**:

Enter a title for this payment method. This text will be displayed while listing the payment methods during checkout. This is an optional parameter.

**API Key:**

The API key provided by ETS ( Please enter the key without the curly braces )

**Geo Zone**:

By selecting a Geozone here, you can restrict customers of a selected Geo-regions from viewing the payment method. Choose all Geozones to show the payment method to customers of all Geo-regions.

**Display text on selection:**

The text entered here is displayed when a customer selects this payment method. You can enter a language constant as a value here, if you are using a multi-lingual site and then
write a language override. Refer the tips below:

>**Tip - ONLY FOR MULTI-LINGUAL SITES**

For example, enter a language constant:
**J2STORE_TEXT_TO_DISPLAY_ON_SELECTION**

Now you can go to Joomla admin-> Language Manager->Overrides and create overrides for the language constant in all languages.