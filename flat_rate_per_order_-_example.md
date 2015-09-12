# Flat Rate per Order - Example

To create a shipping method of type **Flat rate per Order**, follow the steps given below:

> Assume that you have a store in California, USA. You will get orders from all over USA. You need to ship the consignment to the customer, with a flat $50.00 shipping rate per order. Let us see how a **Flat rate per order** shipping method can be created for your store.

1. Go to **J2Store Dashboard -> Setup -> Configuration** and select the **Store** tab, as shown in the image. Enter the details and ensure that **United States** and **California**, are selected for country and zone, respectively.
![Store Details](./assets/images/store_details.png)

2. Go to **J2Store Dashboard -> Localization -> Geozones** and click on the **New** button in the top left corner to create new geozone, as shown in the image. 
![Create Geozone](./assets/images/create_geozone.png)
Enter the name for the geozone as **Default Geozone** and select country and zone as **United States** and **California** respectively, as shown below. Click **Save & Close**.
![geozone](./assets/images/geozone_creation.png)

3. Go to **J2Store Dashboard -> Setup**
![Dashboard](./assets/images/flat_rate_per_order_dashboard.png)

4. Select **Set Up -> Shipping Methods**
![Shipping Methods](./assets/images/flat_rate_per_order_dashboard_setup.png)

5. From the list, click on the **Create / Edit / Link** in the **Standard Shipping Methods** category
![list of methods](./assets/images/list _of_shipping_methods.png)

6. From the obtained window, click on the **New** button
![create new](./assets/images/std_ship_methods_create.png)

7. You will get the form to add a new shipping method
![Shipping Method Details](./assets/images/ship_method_add_values.png)
>IMPORTANT NOTE: To apply flat rate shipping method, you should enable over-riding of shipping address with store address.  If over-ride option is set to **No**, then customers in **California** only can avail this method and customers in rest of the country will not be charged with shipping cost.

8. **Save & Close** window. Now you can see the created shipping method in the list as show in the image below. Now, you need to set the rate for the shipping method. To do that, click on the link **Set Rates**.
![new std ship method](./assets/images/std_ship_mthds_list.png)

9. You will get a pop-up window to set the rates for the shipping method, as shown below. 
![Set Rate](./assets/images/std_ship_method_set_rate.png)

Now all are set and your shipping method is ready for use.

 

