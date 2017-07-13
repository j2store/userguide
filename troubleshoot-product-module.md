# Troubleshoot product display module issues

#### Why product description not showing when viewing product using J2Store Product Display Module ?

**Reason :** You have not chosen J2Store > Product list view menu in module settings.

If you have not selected a product list menu in the Product display module, then while visiting the detail page, the system wont know where to inherit the display parameters from.

Please check the product module settings and make sure you have selected a product list menu there.
Then in the respective menu, make sure that the product descriptions are set to show in the Item view options tab.

#### Are you getting error when you click to view product ?

It seems you have not chosen source category in the module settings.

If you select **Categories** as your product source. then you should select the categories. Otherwise the system does not know where to fetch and display the products.

#### [HOW TO]Change the color of the price and product-title only in the product module ?

You can use respective class name to write styles only for product module. For example, to change the color of price and product title,
```css
.j2store-product-module .product-title > a {
    color: #ffffff;
}

.j2store-product-module .product-price-container .sale-price {
    color: #ffffff;
}
```

#### [HOW TO]Remove Compare & Wishlist options from J2Store Products Module ? 

Below css will hide the compare and wishlist dislaying at J2Store Product Module.
```css
.mod_j2store_products .product-compare, .mod_j2store_products .product-wishlist {
    display: none;
}
```

#### Grid layout problem in Product Display Module

Some times the module does not display the products as per your settings. (i.e) you have set column as 3 but it displays the products in single column.

This problem seems to be choosing of wrong sub-template.

Open your module settings
Choose Bootstrap 3 as your sub template
Save.

If it is already set to Bootstrap 3, change to Default layout and check.

Still no luck ? Make sure your template has full boostrap support. Another possible reason the css might be conflicting.

#### Do you want to display specific products in your site ?

Choose Selected products as your product source in your module settings.
Then, click on **Add products** button to select specific products.
