# Use cases


#### Book a hall

#### Scenario:

1. Renting the hall on a daily basis.
2. Setting the capacity of the hall to 50 persons.
3. Booking slots will be available only on week days and not on weekends.

#### Creating a product

1. Go to Article manager and create a new article.
2. Move to J2Store cart tab and choose **YES** to treat as a product.
3. Choose product type as **Booking** and save.

#### General tab

After creating the product, navigate to general tab.

**Booking duration**

In our sample scenario, we are renting the hall on a daily basis. So Set the Booking duration to Fixed blocks of 1 day(s).

#### Pricing tab

Set the pricing and navigate to the next tab.

#### Persons tab

Our instance says that we are going to restrict the capacity only to 50 Persons. So following are the criteria to be set:

```
Min persons = 1

Max persons = 50
```
#### Availability tab

The hall would be rented on a daily basis. The parameters should be set as follows:

```
Max bookings per block = 1

Minimum block bookable= 1 day(s) into the future

Maximum block bookable= 30 day(s) into the future

```

To restrict the availability of the hall only to week days and block the availability on weekends:


```
Range type = Range of days

Range = Saturday to Sunday

Bookable = No

```

Here are the screenshots that demonstrate the workflow of the above conditions:

![](./assets/images/bookingusecases1.png)

![](./assets/images/bookingusecases2.png)

![](./assets/images/bookingusecases3.png)

![](./assets/images/bookingusecases4.png)


### 1. Rent a party hall

A person owns a party hall that people can rent for a Birthday parties.

##### Instance

1. The hall will be available for only 30 days.
1. It can accommodate upto 75 people.
2. The party hall owner wants customers to not book a party hall on specific set of date range.
3. The party hall owner wants to restrict multiple bookings per block.
4. The hall can be booked for only one day.

### Booking Configuration

#### Creating product

1. Go to Article manager and create a new article.
2. Move to J2Store cart tab and choose **YES** to treat as a product.
3. Choose product type as **Booking** and save.

#### General tab

After creating the product, navigate to general tab.

**Booking duration**

To allow customers to book the party hall only for one day, set this parameter to **Fixed blocks of 1 day(s)**.

**Calendar display mode**

Choose whether the calendar must be opened by default or should be displayed when customer click on choose button. Setting **Display calendar on click** will hide the calendar until customer clicks on choose date.

![](./assets/images/usecase1-booking-duration.png)

#### Pricing tab

After defining booking duration, navigate to pricing tab and set the product's regular price and block price.

![](./assets/images/usecase1-booking-pricing.png)

#### Persons tab

In our example, the maximum persons we allowed is 75. So set **YES** to enable person and then set

```
Min persons = 1

Max persons = 75
```
![](./assets/images/usecase1-booking-person.png)

If you would like to multiply the block price with person count then set **YES** to **Mutiply block price by person count**.

#### Availability

1. To restrict customers from multiple booking per block, give **1** (one) to the text box named **Max bookings per block**.

2. **To make the hall unavailable after 30 days, set**

   ```
   Minimum block bookable = 0 or 1 day(s)

   Maximum block bookable = 30 day(s)
   ```

3. **Restrict booking on specific date range**

 To make specific date range to be unavailable for booking, set **All dates** parameter to **available by default** and click on **Add range** button to define specific date range.

 After clicking on Add range, on the new row created, define the date range like below:

 **Range type** - Date range
 **Range** - 27-09-2017 to 29-09-2017
 **Bookable** - No
 **Priority** - 1

 ![](./assets/images/usecase1-booking-availability.png)

<a name="custom-date-time-range"></a>
### 2. Block availability with date and hour range

This use case will show you how to make the blocks available with date and hour range.

#### Instance

1. Booking will be available only on **Tuesdays** from **10.00 AM to 7.00 PM**
2. Booking will be unavailable on **03-10-2017**.

#### Creating product

1. Go to Article manager and create a new article.
2. Move to J2Store cart tab and choose **YES** to treat as a product.
3. Choose product type as **Booking** and save.

#### General tab

After creating the product, navigate to general tab.

**Booking duration**

Set this parameter to **Fixed blocks of 1 Hour(s)** to make the block available with custom time range.

Then move to pricing tab to define the booking cost and then navigate to Person tab if you would like to define minimum and maximum persons.

![](./assets/images/usecase2-booking-duration.png)

#### Availability

1. Define the number of bookings per block. If you wish to restrict customers from multiple booking then give 1 to this option.

2. To make the blocks available for 12 months, you will have to set the minimum and maximum bookable block like below:

```
Minimum block bookable = 0 Day(s)

Maximum block bookable = 12 Month(s)
```

Then, set all the dates to not available. Choose **not-available by default** to All dates are parameter.

Now set the date and time range by click in **Add Range** button and set priority accordingly. Refer the screen shot below:

![](./assets/images/usecase2-booking-availability.png)

#### On frontend

![](./assets/images/usecase2-booking-demo.png)

<a name="boat-ride"></a>
### Book for a boat ride

#### Instance

An owner of boat offers boat ride for daily on hourly basis. The duration of journey is 2 hours and the start times are 10:00 AM, 2:00 PM, & 6:00 PM. The booking price for Adults and Children can be vary. The maximum capacity of boat is 25.

#### Configuration of bookable product

1. Go to Article manager and create a new article.
2. Move to J2Store cart tab and choose **YES** to treat as a product.
3. Choose product type as **Booking** and save.

#### General tab

After creating the product, navigate to general tab.

**Booking duration**

In our example, the duration of boat ride is **2 hours**. So set booking duration to **Fixed blocks of 2 Hour(s)**.

#### Persons tab

In this example, the pricing can be vary based on person types. To set different pricing for Adults and Children, **Enable person types**.

Set **YES** to Enable person types and 	click on **Add person types** button to add person type Adults and Children. And then define the base cost, block cost, minimum and maximum number for each person type.

Take a look at below demo screen shot to see how the parameters under person tab are configured.

![](./assets/images/usecase3-booking-person.png)

#### Availability

```
Maximum bookings per block = 25
All dates are = not available by default
```
**Add time range for boat ride by referring to the below picture**

![](./assets/images/usecase3-booking-availability.png)

#### Frontend

![](./assets/images/usecase3-booking-frontend.png)
