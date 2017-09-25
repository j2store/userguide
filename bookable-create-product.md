# Creating a bookable product

Once the global settings have been completed, we are all set to create a bookable product. To create a bookable product, go to Article Manager and create a new article.

While creating new product, choose **Booking** as a product type.
![](./assets/images/select-bookable-product.png)

Apart form the default options that are available for all the product types, these are the various parameters that distinguish the booking type product from the other product types:

* **[Creating a bookable product](#creatingabookableproduct)**
   * **[General tab](#general)**
   * **[Pricing tab](#pricing)**
   * **[Persons](#persons)**
   * **[Availability](#availability)**

<a name="general"></a>
### General Tab

#### Booking duration

The duration can be defined by admin or by customer.

**Fixed blocks**  You can define a fixed block of dates that are to be allowed for booking while the others are being disabled in the frontend. For example: If you set up the booking duration parameter to be Fixed block of 1 days, then the user will be allowed to choose a single date for booking.

**Customer-defined blocks** you can allow the user to choose the start dates and end dates by themselves. You can also set up the minimum and maximum number of blocks that can be chosen when you choose the Booking duration as customer-defined blocks. 

If you select the booking duration to Customer-defined blocks of 1 days, you would be prompted to choose the minimum and maximum duration allowed. If you choose 2 and 4 respectively, then the users will get a message if they choose dates that are more than 4 days or less than 2 days.

 ![](./assets/images/app_bookingbookingdurationfixedback.png)

 The frontend will be like this:

 ![](./assets/images/app_bookingbookingdurationfixedfront.png)

 When the booking duration is chosen to be Customer-defined blocks of 1 days, the following options pop up:

 * Minimum duration- To set the minimum number of blocks that have to be selected.

 * Maximum duration- To set the maximum number of blocks that have to be selected.

 ![](./assets/images/app_bookingbookingdurationcusback.png)

 The frontend will be like this:

 ![](./assets/images/app_bookingbookingdurationcusfront1.png)

 When the user chooses more blocks than the specified limit, error occurs as follows:

 ![](./assets/images/app_bookingbookingdurationcusfront2.png)

 When the maximum duration is exceeded, the following error occurs:

 ![](./assets/images/app_bookingbookingdurationcusfront3.png)

#### Calendar display mode

 Choose when to display the calendar. You can choose to display the calendar by default or only after clicking.

 The following video demonstrates the use of the calendar display mode option:

 ![](./assets/images/app_bookingcalendarviewbehav.gif)
 
#### Allowing booking cancellation

It is possible to choose whether the store admin want his/her user to have the option to cancel their booking. Setting **YES** to **Can be cancelled?** will allow customer to cancel the booking after it has been purchased.

![](./assets/images/app_bookingcanceloptionfront.png)

<a name="pricing"></a>
### Pricing tab

 The pricing tab for a booking type product has one extra option in addition to the default options as follows:

 **Block pricing**

 While you are able to set a price to the product, the booking type product allows block-wise price charging in addition to the regular pricing which is now an added advantage.

 Here is a screenshot to showcase the use of the block pricing option:

  ![](./assets/images/app_bookingpricingback.png)

 Now that we have set up block pricing, the users will be charged in this way:

  ![](./assets/images/app_bookingpricingfront.png)

<a name="persons"></a>
## Persons

This tab allows you to make the booking for multiple persons. To enable this feature, select **YES**. It is also possible to set a minimum and maximum number of persons.

For example, A car could be rented and maximum 4 persons can only travel. So if you set **Minimum person : 1** and **Maximum persons: 4**, then booking will not be taken for more than 5 persons.

![](./assets/images/booking-enabe-persons.png)

![](./assets/images/person-count-exceed.png)

### Persons will also come into the following cost options:

**Multiply block price by person count**: If this option is enabled, all costs are multiplied by the number of persons the customer defines. It is also possible to enable person types. For example, Booking ticket for the journey might be having following restriction **Only 2 Adults and 3 Children allowed**. In this case, you could add person types and the pricing could be defined accordingly.

![](./assets//images/booking-person-types.png)

Once you enabled person types, you have the option to add multiple types.

Give your Person type a name (for example: Adult, Children) and define the cost (Base cost and Block cost) for the type. Adding a description is optional.

You can define a minimum and a maximum number for each person type. For example, you could require upto 2 adults and maximum 3 children for each booking. If you leave Max blank, there are no other restrictions than those of the bookable product itself.

![](./assets/images/person-type-frontend.png)

<a name="availability"></a>
## Availability

This tab controls the availability of blocks (i.e.) what blocks can be booked. Availability of blocks can be defined based on following time frame:

1. Day(s)
2. Month(s)
3. Hour(s)
4. Minute(s)

**Max bookings per block** : By using this option, you could define the number of bookings per block. For example, if you enter 2, more than 2 bookings on individual blocks are not allowed.

**Minimum block bookable and maximum block bookable** : If today is March 1 and you set minimum block bookable to 1 day into the future, then the first date a customer could book would be March 2. The same applies to the maximum date bookable. If you set maximum block bookable to 2 day into the future, then blocks avalaiable for booking are March 2, March 3.

**All dates are** : This option allows you to define specific date range to be availble or not available by default. The date range can be defined based on following time frames Months, Days, Hours, Minutes.

### Add date range

To add a custom date range, click the **Add Range** button:

On the new row created, choose a range type, From / to range and choose whether it is bookable or not and a priority number. The following are the several date ranges:

1. Date range – from and to will show a datepicker field
2. Range of days – from and to will show a dropdown of days of the week (Monday to Sunday)
3. Range of months – from and to will show a dropdown of months (January to December)
4. Range of weeks – from and to will show a dropdown of weeks (1 to 52)
5. Time ranges – from and to will show time inputs
6. Date Range with time – a time range can be set based on a custom date range

For example, if you would like to make the days from March 20 to March 22 to be non bookable, then you will have to choose **Available by default** to the All dates option and the date range should be set like below:

![](./assets/images/block-available.png)

![](./assets/images/non-available-dates.png)