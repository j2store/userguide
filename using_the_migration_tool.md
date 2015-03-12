# Using the migration tool

### 1. Installation

You can use the standard Joomla installer for installing the tool.

Login to Joomla administrator and go to Extension Manager
and install the tool

### 2. Backup! Backup! Backup!
Take a FULL BACKUP of your website using Akeeba Backup. 
If you proceed without taking a BACKUP, you will not be able to recover your data in case something went wrong.

The Tool will not allow you to proceed if you do not have the Akeeba Backup component installed. 
We had to force this check because some Joomla web masters do not have the habit of taking regular backup of their site.

### 3. Read the instruction
Go to Joomla administrator -> Components -> Migration Tool for J2Store

Read the on-screen instruction. 

#### 3.1 Variant stock
If you are maintain stock for product options (aka Variable product), the tool will migrate all the data except SKU, Price and Stock.

These products will be treated as Variable Product types.
The tool will list the products that fall under the variable product type. Please note down the Article IDs.

Once the migration process is completed, go to Article manager and open these articles. Click Generate variants button (J2Store cart -> Variants tab).
Once generated, click Edit against each variant and then enter the SKU, Price and Stock.

#### 3.2 Downloadable products
The tool will migrate all the data of your downlodable products. There are few changes in the structure of the downlodable products in J2Store Version 3.

##### 3.2.1 Download Limit
Earlier, download limits were set






