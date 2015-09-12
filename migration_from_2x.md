# Migrating from old 2.8.x versions to 3.x

- **[Introduction](#introduction)**
- **[Actions to be taken before migration](#actions)**
- **[Pre-requisites](#pre-requisites)**
- **[Download the migration tool](#download)**
- **[Using the migration tool](#using-migration-tool)**
- **[Reverting back to 2.x after the migration](#revert)**

<a name="introduction"></a>
##Introduction

Version 3 is re-written from scratch using the FOF Framework for Joomla. It comes with loads of new features and follows a different table structure (schema). So a migration is required if you want to update your store from 2.x to Version 3.

We have created a tool, which simplifies the migration of your 2.x store to the latest 3.x version. 
```language
Please read the documentation carefully before you attempt the migration.
```
<a name="actions"></a>
## Actions to be taken before migration

Please install Akeeba Backup, which is one of the best backup apps available for Joomla (and it is free! ) and take a **FULL BACKUP** of your site.
```language
Warning
If you proceed without taking a BACKUP and if you wanted to revert back to old version, you will end up going in the toughest route. So please take a FULL BACKUP of your site before proceeding with the migration
```

Also
- Make sure your J2Store version is 2.8.x or later
- If you are using an old 2.x version, first update it to 2.8.x
- Set your site offline
- Set Error Reporting to None in the Global Configuration

<a name="pre-requisites"></a>
## Pre-requisites

1. Joomla 3.3.x 
2. J2Store 2.8.0 or later

You can use the migration tool only when your Joomla version is 3.3 or later.
If you are currently running the store in Joomla 2.5, please consider upgrading your website to latest Joomla version because the Joomla 2.5 life has ended in December 2014 itself.

<a name="download"></a>
## Download Migration Tool

You can download the migration tool directly from the following url: https://bitbucket.org/j2store/j2store_migration/downloads

<a name="using-migration-tool"></a>
## Using the Migration Tool

### 1. Installation

You can use the standard Joomla installer for installing the tool.

Login to Joomla administrator and go to Extension Manager
and install the tool

### 2. Backup! Backup! Backup!
Take a FULL BACKUP of your website using Akeeba Backup. 
If you proceed without taking a BACKUP, you will not be able to recover your data in case something went wrong.

The Tool will not allow you to proceed if you do not have the Akeeba Backup component installed. 
We had to force this check because some Joomla web masters do not have the habit of taking regular backup of their site.

### 3. Important points to note down
J2Store Version 3 is completely re-written from scratch. We have made quite a lot of structural changes. So some of the product types require additional inputs after the migration.

#### 3.1 Variant stock
If you are to maintain stock for product options (aka Variable product), the tool will migrate all the data except SKU, Price and Stock.

These products will be treated as Variable Product types.
The tool will list the products that fall under the variable product type. Please note down the Article IDs.

Once the migration process is completed, go to Article manager and open these articles. Click Generate variants button (J2Store cart -> Variants tab).
Once generated, click Edit against each variant and then enter the SKU, Price and Stock.

#### 3.2 Downloadable products
The tool will migrate all the data of your downloadable products. There are few changes in the structure of the downloadable products in J2Store Version 3.

##### 3.2.1 Download Limit
Earlier, download limit was set against each file. But now, the limit is set per product. Plus, there is an expiry control.
You can set the download availability to expire XX days after the order is confirmed.

The limit and the expiry control has to be set by opening all your products. Otherwise, J2Store v3 will not limit the number of downloads per user.

#### 4. Prepare for migration

Once all checks passed, the tool will display the Prepare for Migration button.
Click the button. It will backup all your J2Store 2.x tables
Once backup is done, you can see the Start Migration button

#### 5. Start Migration

Click the Start Migration button and wait. 
The tool will migrate the data, remove old modules, install the new tables / db schema for J2Store version and uninstall old J2Store version 2.x.

If the migration is successful, you can will see a success message. If there is an error, it will display the error.

##### 5.1 What should i do if an error occured
Please post the error at the forum http://j2store.org/forum/j2store-version-3-feedback.html

#### 6. Install Version 3
Download J2Store Version 3 latest version from the site and install it. 
Free users can download from http://j2store.org/download.html

PRO users can download the PRO version from http://j2store.org/my-downloads.html

#### 7. Post migration
Once migration is successful, download the latest J2Store Version 3 from our site and install it.

Then Go to Joomla administrator -> Components -> J2Store

- Go to Set up - Configurations
- Review the parameters and set them up as per your requirements.
- Go to Catalog - Products - Open a product
- Check if everything is right and save it.

<a name="revert"></a>
## Reverting back to 2.x after the migration
```language
VERY IMPORTANT: Apply the following steps only if you migrated from 2.8.x to 3.x and then want to downgrade.
You should be familiar with Joomla tables and PhpMyAdmin operations.
Otherwise, **NEVER EVER** attempt this if you DO NOT understand any of the steps below.
```

**Step 1:** Backup your site using Akeeba Backup

**Step 2: ** Uninstall J2Store version 3

**Step 3:** Go to Phpmyadmin

You will see

a. Tables with the follwing prefix: 

```_v2_j2store_```  = These are your 2.x tables backed up by the migration tool

b. Tables with the prefix:
```_j2store_``` = these are J2Store 3.x tables

Delete the tables with the prefix ```_j2store_```

Rename the ```_v2_j2store_``` tables to ```_j2store_```

Example: ```_v2_j2store_orders``` to ```_j2store_orders```

**Step 4:** Install J2Store 2.8.x version