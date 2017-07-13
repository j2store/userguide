# How to add license key and update J2Store?

* **[Adding license key](#license-key)**
* **[Update](#update)**
    * **[Updating directly](#update-directly)**
    * **[Updating via Extensions Manager](extension-manager)**
* **[Updating from FREE to PRO version](#update-free-pro)**
* **[Troubleshooting update related issues](#troubleshoot)**
    * **[Firewall](#firewall)**
    * **[Timeout](#timeout)**

<a name="license-key"></a>
### Adding license key

We provide a Download ID when you subscribe. You can find this Download ID in two places.

    In the PDF invoice we have issued to you
    In our website's My Downloads section. Direct link: https://www.j2store.org/my-account/my-downloads.html

You should copy the Download ID and paste it in J2Store - Set up - Configuration - Update tab.

**NOTE:** If you have re-set your password in our site, then a new download ID will be issued (due to security reasons and prevent unauthorized access.) Please make sure that the Download ID is correct.

<a name="update"></a>
### Update

>**Very Very Important** Take a **FULL BACKUP** of your site before you update. We recommend using the **Akeeba Backup** (free backup extension for joomla) to take a backup. DO NOT proceed to update without taking a backup.

Updating to the latest version J2Store can be updated with two different methods: installing the new version on top of the old one or using the Joomla Extensions Update feature.

<a name="update-directly"></a>
#### Updating directly

This is the failsafe approach, but the least convenient. Download the latest J2Store release from our Downloads section and save the ZIP file to your hard disk.

>Important J2Store Pro users should download the PRO version. You can download the PRO version from our site's My Account > My Downloads section

Log in to your site's backend, click on Extensions Manager. Use the Browse... button to locate the ZIP file you downloaded, then click on Upload and Install.

<a name="extension-manager"></a>
#### Updating via Extensions Manager

J2Store integrates nicely with the Extension Manager's update feature. Whenever an update is available, you will see the update notification in your J2Store dashboard. Clicking on the update button will take you to the Extension Manager update section. There you can update to the Latest version.

<a name="update=free-pro"></a>
### Updating from FREE to PRO version

There are chances that you have used the FREE version to set up your store first. And you have subscribed to a plan to get the PRO version. In this case, you should download the PRO version from our My Downloads section and install it over the free version.

>DO NOT **uninstall** the free version. Just install the PRO over the free version.

>Updating from free version to PRO version will **NOT affect you store settings and data.**

<a name="troubleshoot"></a>
### Troubleshooting update related issues

2Store uses the Joomla Extension Manager for providing updates to both the free and pro users. On a few occasions, you may not be able to access the updates via the Extensions Manager. You may get a 403 access denied when you try to update in your site. It might be due to several reasons. We have listed a few that might cause this problem.

> Make sure that the **Download ID** you have entered is correct.

<a name="firewall"></a>
#### Firewall

If you make repeated attempts or requests, then our firewall might block the access for a temporary period (usually 10 minutes).

In this case, please try after 10 minutes.

If still you get the error, you can always download the latest version from our My Downloads section: https://www.j2store.org/my-account/my-downloads.html and install it via the Extensions manager.

<a name="timeout"></a>
#### Timeout

J2Store uses the Joomla Extension Update tool. A time out will occur if your connection is slow or if our server responds slower (which sometime occur if there are huge number of download requests)

In this case, just try again after a few minutes. You will usually get through.