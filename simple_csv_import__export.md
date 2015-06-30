# Simple CSV Import and Export

This is an app that facilitates the import and export functionalities with regard to .csv files.

#### Important instructions before using this app

1. **Backup your site** - 
Before you tend to use this app for import / export operations, you **MUST** be careful enough to take a full backup of your site. Use Akeeba backup to take the backup.

2. **Export once** - 
Export your products into .csv format once, to see how the format looks like. Check for field names. They should match. Also, the SKU of the product in the exported .csv file should be the same as the original SKU.

3. **Importing New Products** - 
If you import new products, then you can ingnore the product id. Otherwise, you have to take care of the product id. If any of the importing products has an id matching with existing id, it will result in an error. 

4. **Unique SKU**
    1. SKU of the products **MUST** be unique. If there is a match, it will result in an error.
    2. The app depends on SKU to find a product. So, if an SKU is found when searched, the existing product will be updated with the imported product details. If a match is not found, a new product will be created with the SKU. 

5. Refer this user guide before exporting excel file to .csv file. 

6. Support for importing products options and / or product variants are not available.

### Parameters

1. **Choose Import Type** - 
There are two options in this parameter. If you select **Upload**, then a preset path will be used. If you select **Path**, then you have to enter the correct path. It is recommended to leave the default setting of **Upload**.

2. **Upload the CSV file** - 
Click on the *Browse* button to select the file for uploading.

3. **Character Set** -
There are numerous character sets listed here to select from. If you are not sure about which is the one to select, it would be safe to leave it as **Not Known**.

4. **Update product if SKU already exists** -
If you select **Yes** in this option, it will update the existing product details, if a match is found. If you are aware of the consequences, then carefully select to **Yes**. Else, to be on the safer side, leave it as **No**.

5. **Export** -
Clicking this button will export your products to csv format. But, before that, double check your SKU numbers are correct. If you have additional images, you can export them, using '|' as separator between two images.

The follwing image illustrates the actions that are involved in import and export of .csv file.

![](csv-import-settings-edited.png)

















