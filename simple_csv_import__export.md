# Simple CSV Import and Export

The app helps you import products from a CSV file. 

#### Important instructions before using this app

1. **Backup your site** - 
Before you tend to use this app for import / export operations, you **MUST** be careful enough to take a full backup of your site. Use Akeeba backup to take the backup.

2. **Export once** - 
Export your products into .csv format once, to see how the format looks like. Check for field names. They should match. 

3. **Importing New Products** - 
If you want to import new products, then you can ignore the product_id field. And just make sure your products have a unique SKU. If an existing product has the same SKU as your new product, then the app will only update the existing product instead of creating a new one. 

4. **Unique SKU**
    1. SKU of the products **MUST** be unique. If there is a duplicate, it will result in an error.
    2. The app depends on SKU to find a product. So, if an SKU is found when searched, the existing product will be updated with the imported product details. If a match is not found, a new product will be created with the SKU. 

5. Refer the documentation on exporting your <a target="_blank" href="https://support.office.com/en-gb/article/Import-or-export-text-txt-or-csv-files-5250ac4c-663c-47ce-937b-339e391393ba">Excel file as CSV</a>

6. Support for importing product options and / or product variants are not available.

### Parameters

1. **Choose Import Type** - 
You can choose to upload a CSV file or point the app to locate the file in a path. Recommended setting is: Upload.

2. **Upload the CSV file** - 
Click on the *Browse* button to select the CSV file for uploading.

3. **Character Set** -
If you are not sure about the charter set of your file or do know what it is, then it is safe to leave it as **Not Known**. The app will attempt to determine the character set.

4. **Update product if SKU already exists** -
If set to **Yes**, it will update existing products, if the SKU matches. Setting this to **NO** will only create new products. 

5. **Export Products** -
Clicking this button will export your products in csv format. 

The following image illustrates the actions that are involved in import and export of .csv file.

![](csv-import-settings-edited.png)

A sample .csv file is given here for your testing purposes.

[sample.csv](sample.csv)

Below is a list of fields that are supported by the app for importing.

It is NOT necessary to have all these fields in your CSV. The following fields are the minimum required fields: sku, product_type

* product_id
* visibility
* product_source
* product_source_id
* product_type
* taxprofile_id
* manufacturer_id
* vendor_id
* has_options
* addtocart_text
* enabled
* plugins
* params
* created_on
* created_by
* modified_on
* modified_by
* up_sells
* cross_sells
* productfilter_ids
* main_image
* thumb_image
* additional_images
* title
* alias
* introtext
* fulltext
* state
* catid
* created
* created_by_alias
* modified
* checked_out
* checked_out_time
* publish_up
* publish_down
* version
* ordering
* metakey
* metadesc
* access
* hits
* metadata
* featured
* language
* xreference
* is_master
* sku
* upc
* price
* shipping
* length
* width
* height
* length_class_id
* weight
* weight_class_id
* manage_stock
* quantity_restriction
* min_out_qty
* use_store_config_min_out_qty
* min_sale_qty
* use_store_config_min_sale_qty
* max_sale_qty
* use_store_config_max_sale_qty
* notify_qty
* use_store_config_notify_qty
* availability
* allow_backorder
* isdefault_variant
* quantity

### TIPS

If you want to import more than one additional images (in the additional_images field), you can use a pipe symbol (|) to separate them.

**Example:** path/to/image1.jpg | path/to/image2.jpg
