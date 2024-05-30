
# Customer Preference Analysis on Zomato's Dataset

<br />

## Table Of Contents

- [Overview of Dataset from Kaggle](#overview-of-dataset-from-kaggle)

- [Choosing our Business Problem](#choosing-our-business-problem)

- [Technologies Used](#technologies-used)

- [Visualizations and Insights](#visualizations-and-insights)

	- [1. Table Booking Preference.](#1-table-booking-preference)

	- [2. Online Order Trends.](#2-online-order-trends)

	- [3. Number of Online Orders for The Top 10 Hotels.](#3-number-of-online-orders-for-the-top-10-hotels)

	- [4. Number of Table Books for the Top 10 Hotels.](#4-number-of-table-books-for-the-top-10-hotels)

	- [5. Location Preferences based on Rating.](#5-location-preferences-based-on-rating)

	- [6. Most Expensive Hotels according to the rest Types.](#6-most-expensive-hotels-according-to-the-rest-types)

	- [7. Number of Restaurant in Each Location.](#7-number-of-restaurant-in-each-location)

	- [8. Relationship between Cost and Rating.](#8-relationship-between-cost-and-rating)

	- [9. Most Popular Cuisines Top 10 Locations.](#9-most-popular-cuisines-top-10-locations)

	- [10. Top 10 Locations with Most Unique Cuisines.](#10-top-10-locations-with-most-unique-cuisines)

	- [11.Restaurant Density Availability.](#11restaurant-density-availability)

	- [12. Top 10 Locations with Most Online Orders.](#12-top-10-locations-with-most-online-orders)

	- [13. Top 10 Locations with Moost Table Bookings.](#13-top-10-locations-with-moost-table-bookings)

	- [14. Most Affordable Locations for a Couple with the most Available Hotels.](#14-most-affordable-locations-for-a-couple-with-the-most-available-hotels)

  

<br />

  

<a  id="overview-of-dataset-from-kaggle"></a>

  

## Overview of Dataset from Kaggle

  

This project's dataset is available on [Kaggle](https://www.kaggle.com/). Click [here](https://www.kaggle.com/datasets/rajeshrampure/zomato-dataset) to get access to the Zomato's Dataset.

  

This dataset is a collection of restaurants that are registered on Zomato in Bengaluru City. In this dataset, we have more than 50000 rows and 17 columns, a fairly large dataset.

  

You will be able to get hands-on experience while performing the following tasks and will be able to understand how real-world problem statement analysis is done.

  

<br />

  

Here' a detailed breakdown of the dataset:

| **Column Name** | **Description** | **Total Records** | **Missing Values** | **Type of Data** |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------- | ----------------: | -----------------: | ---------------- |
| url | This link opens up the profile of the Hotel on the zomato website. It starts as the starting point for the users activity. | 51717 | 0 | Categorical |
| menu_list | It is the collection of dishes the Hotel offers. | 51717 | 0 | Categorical |
| reviews_list | It is the list of customer review (what they had to say about the hotel / service, etc) | 51717 | 0 | Categorical |
| listed_in(type) | Specifies what category of the food place is. | 51717 | 0 | Categorical |
| votes | votes may give an indication of recommending this hotel to the other website visitors. | 51717 | 0 | Numerical |
| listed_in(city) | It is listed in which city. It defines a bigger province than the actual location. | 51717 | 0 | Categorical |
| book_table | Tells whether the booking a table in advance is available or not. | 51717 | 0 | Categorical |
| online_order | Tells whether the ordering online is available or not. | 51717 | 0 | Categorical |
| name | Name of the Hotel | 51717 | 0 | Categorical |
| address | Detailed Address including plot no, street no, etc. | 51717 | 0 | Categorical |
| location | The landmark or city or town. It is a smaller region under the city (larger province) | 51717 | 21 | Categorical |
| cuisines | Style of Food the hote offers accordnig to geographical speciality. | 51717 | 45 | Categorical |
| rest_type | Tells what the Hotel is most suitable for various moods, time constraints, etc. | 51717 | 227 | Categorical |
| approx_cost(for two people) | Cost in INR | 51717 | 346 | Numerical |
| phone | contact no. of the Hotel | 51717 | 1208 | Numerical |
| rate | Rating given to the Hotel on the scale of 0 to 5 | 51717 | 7775 | Numerical |
| dish_liked | Most favourite dishes of the customers of all time. | 51717 | 28078 | Categorical |

  

<br /> <a  id="choosing-our-business-problem"></a>

  

## Choosing our Business Problem

  

In the Kaggle's Project Description there was no problem statement defined. Thus we had the freedom to choose from many out of which we decided to proceed with "Customer Preference Analysis".

  

Other potential business problems that can be solved using data analytics:

  

- Location Selection for New Restaurants
- Price Optimization
- Identifying Unique Selling Points (USPs)
- Customer Retention
- Operational Efficiency
- Marketing Strategy
- Competitor Analysis
- Staffing Optimization
- Predicting Success for New Restaurants

<br /> <a  id="technologies-used"></a>
## Technologies Used

- [Numpy](https://numpy.org/) (1.26.4)
- [Pandas](https://pandas.pydata.org/) (2.2.2)
- [Matplotlib](https://matplotlib.org/) (3.9.0)
- [Seaborn](https://seaborn.pydata.org/) (0.13.2)

If want to install all the above libraries, open your project in the terminal and execute the following command:
```
pip install numpy pandas matplotlib seaborn
```
The above command should install the necessary libraries of the stable releases.

If you wish to use `conda` instead of `pip` or want to install specific versions, feel free to visit their official websites linked above.


<br /> <a  id="visualizations-and-insights"></a>
## Visualizations and Insights


### 1. Table Booking Preference.

![1. Table Booking Preference.](/Visualizations/01.png)

- There are almost **5.5 time more hotels** that _don't allow_ booking tables in advance.
- This might lead to higher crowds in the most places and waiting periods.
- This is an opportunity for the hotel to get more customers on boards and practice delivering better service.


### 2. Online Order Trends.

![2. Online Order Trends.](/Visualizations/02.png)

- Almost **30% more hotel offer online delivery services** to thier customers, that counterparts.
- It more like that hotel offering online order, have more customer and thus more revenue.


### 3. Number of Online Orders for The Top 10 Hotels.

![3. Number of Online Orders for The Top 10 Hotels.](/Visualizations/03.png)

-  _Cafe Coffee Day_ tops the list of hotel offering oline delivery, with approx. **85 orders** alone.

- On the contrary, other top hotels offer deliver count ranging from **55 to 65**.


### 4. Number of Table Books for the Top 10 Hotels.

![4. Number of Table Books for the Top 10 Hotels.](/Visualizations/04.png)

-  _Cafe Coffee Day_ tops the list of hotel offering booking table, again, with approx. **85 orders** alone.
- On the contrary, other top hotels offer deliver count ranging from **55 to 65**.
-  _There is no significant difference in the number of table bookings between top and bottom rated hotels_


### 5. Location Preferences based on Rating.

![5. Location Preferences based on Rating.](/Visualizations/05.png)

- All the Top Hotels with the most number of Rating will the minimum rating of **3.8**.
- Hence, you're asured to get the best service from these top locations.


### 6. Most Expensive Hotels according to the rest Types.

![6. Most Expensive Hotels according to the rest Types.](/Visualizations/06.png)

- In terms of Cost, Fine Dining - Microbrewery, Fine Dining - Lounges and Fine Dining, Bar are the most expensive Restaurant types with **approx. cost of 2,900 and above**.
- Other best option range from **1,900 to 2,900** respectively.


### 7. Number of Restaurant in Each Location.

![7. Number of Restaurant in Each Location.](/Visualizations/07.png)

- Considering the availability of the Hotels, BTM tops the list with 2,500+ hotels.
- Comparing to other locations, the number of restaurants range from **1,500 to 2,000 for top 4 locations** and **1,000 to 1,500** for the other best location.


### 8. Relationship between Cost and Rating.

![8. Relationship between Cost and Rating.](/Visualizations/08.png)

- Majority of Hotel offer the will ave the **rating of above 3.25** and will cost anything from **1,000 to 3,000** which is fairly reasonable.
- when looking for hotel with **rating above 4**, the range from **1,000 to 5,000.**
- To an extent, **the cost for a couple is directly proportional to the rating.**


### 9. Most Popular Cuisines Top 10 Locations.

![9. Most Popular Cuisines Top 10 Locations.](/Visualizations/09.png)

- North Indian and Chinese are the 2 most popular cuisines in all locations.
- Specifically, BTM and Marathahalli offer the best in class North Indian and Chinese cuisines.


### 10. Top 10 Locations with Most Unique Cuisines.

![10. Top 10 Locations with Most Unique Cuisines.](/Visualizations/10.png)

- Whitefield is the top location with approx. **350+ unique cuisines**.
- Hotel from 2nd to 6th ranks do offers uniques **300 to 350 cuisines.**


### 11.Restaurant Density Availability.

![11.Restaurant Density Availability.](/Visualizations/11.png)

- BTM location has the most number of hotel, i.e., 2500+.
- Other best 4 best performing locations have **approx. 1500 to 2000** number of hotel.
- The rest of the locations have **alteast 1000** hotels.


### 12. Top 10 Locations with Most Online Orders.

![12. Top 10 Locations with Most Online Orders.](/Visualizations/12.png)

- Out of all the hotels with the most number online orders, **90% of the hotels have higher chance of ofeering online orders**, except _Electronic City_.


### 13. Top 10 Locations with Moost Table Bookings.

![13. Top 10 Locations with Moost Table Bookings.](/Visualizations/13.png)

- Out of all the hotels allowing table booking, only, _Koramangala 4th Block_ and and _MG Road_ have 50% possibility of offering table booking.
- For other locations, the allowing booking table is **near to 20%.**


### 14. Most Affordable Locations for a Couple with the most Available Hotels.

![14. Most Affordable Locations for a Couple with the most Available Hotels.](/Visualizations/14.png)

- BTM has the **lowest cost** of the other high-quality competitors, i.e., **400**.
- On the contrary, **average cost** for the other competitors goes upto **550.**
