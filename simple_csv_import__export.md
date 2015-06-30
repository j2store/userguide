# Simple CSV Import and Export

This is an app that facilitates the import and export functionalities with regard to .csv files.

#### Important instructions before using this app

1. **Backup your site** - 
Before you tend to use this app for import / export operations, you **MUST** be careful enough to take a full backup of your site. Use Akeeba backup to take the backup.

2. **Export once** - 
Export your products into .csc format once, to see how the format looks like. Check for field names. They should match. Also, the SKU of the product in the exported .csv file should be the same as the original SKU.

3. **Importing New Products** - 
If you import new products, then you can ingnore the product id. Otherwise, you have take care of the product id. If any of the importing products has an id matching with existing id, it will result in an error. 

4. **Unique SKU**
    1. SKU of the products **MUST** be unique. If there is a match, it will result in an error.
    2. The app depends on SKU to find a product. So, if an SKU is found when searched, the existing product will be updated with the imported product details. Else, a new product will be created with the SKU. 

5. Refer this user guide before exporting excel file to .csv file. 

6. Support for importing products options and / or product variants are not available.



























