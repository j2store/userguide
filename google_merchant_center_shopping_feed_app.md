# Google Merchant Center - Shopping feed 

The app helps you export products for Google Shopping feed. 
New to the term Google Merchant? More details can be found at [Google Merchant Center ](https://www.google.com/retail/merchant-center/)

If you have any doubts or queries regarding the Merchant center service, visit [Google merchant Support center](https://support.google.com/merchants/)

### Parameters

1. **Google Category** - Google has its own detailed taxonomy (or) classification of products. Input the category to which all your products belong to. For list of categories provided by Google, refer this [link](https://support.google.com/merchants/answer/1705911).

2. **CSV file Name** - 
Name of CSV file used to upload in merchant center. Make sure the file name does not contain any spaces (use underscores or hyphen symbol instead of space).

3. **Product Condition** -
Please select your product condition from this list. This field is mandatory and should not be skipped.


The following image illustrates the actions that are involved in import and export of .csv file.

![](csv-import-settings-edited.png)

A sample .csv file is given here for your testing purposes.

[sample.csv](sample.csv)

Below is a list of fields that are supported by the app for importing.

It is NOT necessary to have all these fields in your CSV. The following fields are the minimum required fields: sku, product_type

* sku
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
