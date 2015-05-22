# DHL Shipping Plugin

This plugin integrates DHL Shipping Rate API with J2Store.

### Requirements

* PHP 5.2 or higher
* Joomla 2.5 or above
* J2Store 2.7.3 or above

### Installation

1. Use Joomla installer to install the plugin.
2. In the Joomla control panel, go to **Extension -> Plugin Manager.** Open the DHL Shipping(type=j2store).
3. Enable plugin.
4. Enter Plugin Params
 
#### Params :
1. **Site ID:**
	This is your DHL Site Id associated with your DHL accout.

2. **DHL Password:**
	This is your DHL Password associated with your DHL accout.

3. **DHL Account Number:**
	This is your DHL Account Number associated with your DHL accout.

4. **Test Mode:**
	1. NO for “live Account” 
	2. Yes for “Test Account” 
		Before going live, you can test your store using the Test mode. IN LIVE SITE , THIS	SHOULD BE SET TO “NO”.

5. Show Date/Time:
	Set to Yes for display delivery Date/Time in DHL service.

6. Tax class:
	If you want to add tax rate for your shipping, Select tax profile.

7. Geo Zone:
	By selecting a geozone here, you can restrict this Shipping method from showing to customers from only that geo-region. Choose All geozones to show this method to all customers.

8. Handling cost:
	If you need to charge an additional handling fee, enter the handling cost in this field.

9. Debug Mode:
	Enable/Disable Log file for Debug DHL Shipping Plugin. This Must set to “NO” in Live Site.

Support
	Still have questions? You can reach us in support@j2store.org 
Thank you for using our extension.