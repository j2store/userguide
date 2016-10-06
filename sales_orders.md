# Orders

A customer views the product and completes the checkout process, it is transformed into an order. Orders are listed here according to their statuses. They are as follows:
* Confirmed
* Failed
* Processed
* Pending
* New
* Cancelled

Every order will posses some important information that explains about it. They are:
* **Invoice No** - The number of the document that completes the process of that order
* **Order ID** - ID for reference that tracks all the processing steps
* **Date** - The date in which the order is completed
* **Amount** - The total value of the order after billing
* **Payment Method** - The method in which the customer has paid for the order viz., bank transfer, paypal, moneyorder, etc
* **Status** - Completed or still in process - like information


Check the image below to understand clearly.

![Order Listing](./assets/images/order_listing.png)

#### Adding shipping tracking ID

If you have enabled shipping in your site, in admin order history page you can see the text box to enter shipping tracking ID. Enter your shipping tracking ID and click save.
![shipping tracking](./assets/images/sales-order-01.png)

Now go to J2Store > Design > Email Templates and add the short tag [SHIPPING_TRACKING_ID] in your email template.

![tracking id email](./assets/images/sales-order-02.png)