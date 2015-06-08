# Weight based per Order - Example

To create a shipping method of type **Weight based per Order**, follow the steps given below:

> Assume that you have a store in California, USA. You will get orders from all over USA. You need to ship the consignment to the customer, with shipping rate based on weight of items per order. Let us see how a **Weight based per order** shipping method can be created for your store.

For a better understanding, consider this:

Your shop is in California, US. For shipping within California, a separate geozone is created for California and the shipping charges will be as levied as follows, provided the **minimum** quantity eligible for shipping is 50 Kgs. The below table shows the weight and the corresponding shipping charges.

| Weight (In Kilograms - Kg) | Rate (In USD - $) |
| -- | -- |
| 50 - 250 | 25 |
| 251 - 500 | 35 |
| 501 - 1000 | 50 |

Like this, you can set different rates for shipping outside California, by creating different geozones and fixing different shipping rates, based on the distances of the locations from California, as given below:

| Weight (In Kilograms - Kg) | Philadelphia Rate (In USD - $) | Texas Rate (In USD - $) | New Jersey Rate (In USD - $) |
| -- | -- | -- | -- |
| 50 - 250 | 30 | 40 | 45 |
| 251 - 500 | 40 | 50 | 50 |
| 501 - 1000 | 50 | 60 | 65 |

Now, we will see how to create a shipping method based on the weight of the order itmes.

1. Go to **J2Store Dashboard -> Setup -> Configuration** and select the **Store** tab, as shown in the image. Enter the details and ensure that **United States** and **California**, are selected for country and zone, respectively.
![Store Details](store_details.png)

2. Go to **J2Store Dashboard -> Localization -> Geozones** and click on the **New** button in the top left corner to create new geozone, as shown in the image. 
![Create Geozone](create_geozone.png)
Enter the name for the geozone as **Default Geozone** and select country and zone as **United States** and **California** respectively, as shown below. Click **Save & Close**.
![geozone](geozone_creation.png)

3. Go to **J2Store Dashboard -> Setup**
![Dashboard](flat_rate_per_order_dashboard.png)

4. Select **Set Up -> Shipping Methods**
![Shipping Methods](flat_rate_per_order_dashboard_setup.png)

5. From the list, click on the **Create / Edit / Link** in the **Standard Shipping Methods** category
![list of methods](list _of_shipping_methods.png)

6. From the window you get after you follow the previous step, click on the **New** button in the right side, as indicated in the image below.
![shipping methods](ship_methods_list.png)

7. You will get the form to create new shipping method. Fill in the details as shown in the image.
![Add shipping method](add_weight_ship_mthd.png)

8. **Save & Close** window. Now you can see the created shipping method in the list as show in the image below. Now, you need to set the rate for the shipping method. To do that, click on the link **Set Rates**.
![list of methods](add_weight_ship_mthd_list.png)

9. You will get a pop-up window to set the rates for the shipping method, as shown below. 
![Set shipping rate](weight_ship_set_rate.png)

Now all are set and your shipping method is ready for use.
