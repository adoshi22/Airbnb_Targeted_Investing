# Airbnb_Targeted_Investing
 Investor Report for Airbnbs in San Diego

# Analysis-and-Classification-of-Stack-Overflow-Questions

## For R

## Summary
With our analysis, we have developed a business case for an investor who is interested in acquiring homes in San Diego to put them up as AirBnB rentals.For the investor to determine where to invest, we have provided a comprehensive study based on predictive analysis.With the help of statistical modeling, we have considered certain variables which have a strong effect on the investor’s decision. The selection of variables was based on certain factors which proved to serve the primary purpose of our project; to maximize the investor’s ROI. Some of the factors that were considered include the discerning of neighbourhoods which would yield high returns.One of our principal findings is that achieving a superhost status would help increase the booking rate. Identification of certain amenities which drive the customers’ selection of an Airbnb property in San Diego is a novel realisation in our analysis.


## Description

**Methodology used:**
- Determined the correlation between all the important features. Chose price and high_booking_rate to numerically measure the correlation between them. To further discover the relation between these two features, we plotted the scatter plot and box plot of the divided data against price. Concluded that prices don’t determine booking rates. Also, the properties which have higher booking rates have a median price of $120.

- Selected only those variables that are most closely related to the accommodation at a particular property. Ran logistic regression model with high_booking_rate as DV. We determined the accuracy of the model using a confusion matrix. Concluded that for an Airbnb property to have higher booking rates, it must be flexible with respect to its booking duration and be able to provide accommodation to the guests.

- Determined whether the factors which add to the price. Ran a regression model with high_booking_rate as a dependent variable. Determined the accuracy of the model using a confusion matrix Concluded that (i) If a property provides for extra_people despite charging for the same - its booking rate improves, (ii) Cleaning fee and security deposits do not have any impact on the higher booking rates (iii) If the price of a property is high, its booking rate decreases

- From our XG boost model, we concluded that the host_is_superhost is a really important variable. So, we analyzed this variable further. Selected the superhost and high booking rate columns, filtered the high booking rate = 1 then, grouped by host_is_superhost and got the count of booking rate =1 for both groups (superhost = true and supehost = false). The results of this query shows that Properties with a superhost has a higher chance of having a high booking rate.

- To determine which neighbourhoods are most likely to get high_booking_rate, we plot a map. On the map we plotted the circles whose area is basically dependent on the number of high_booking_rate properties in that area. We concluded that the regions closer to the seafront or beaches are more likely to have a high booking rate than the regions in the middle.

- . To understand the importance of the amenities provided, a column with the count of amenities was introduced. After applying a Random Forest model to the variables including the amenities count, we identified that the count of amenities was the most significant variable. To further add onto this point a density graph was plotted which depicted the amenities provided to rentals with both a high and a low booking rate. This plot was compared against a plot of amenities provided against the high booking rate. This proved that the high booking rate does not depend on the type of amenity provided in the Airbnb rental, but highly depends on the number of amenities provided. A word cloud plotted for both the amenities provided in a low booking rate rental and a high booking rate rental showed almost the same. Out of which free parking space, WiFi, smoke detectors and laptop friendly workspace and the most frequently available amenities.

**Results and Findings:**
• Neighbourhoods which would yield high returns will be Pacific beach, Mission Beach, Ocean Beach, La Jolla and North Park.
• An appropriate price range will be $100 - $120.
• The property must be flexible with respect to its booking duration and be able to provide accommodation to the guests.
• Achieving a superhost status will help in increasing the booking rates.
• A house or an apartment will have more bookings as compared to other property types.
• Amenities which matter the most are Free Parking, Smoke detectors, Wifi, and Laptop friendly workspace.
• Providing more amenities will affect the booking rate.


## References:
1. [San Diego Official Tourism website.](https://www.sandiego.org/explore/events.aspx)
2. [Leaflet for R.](https://rstudio.github.io/leaflet/)
3. [Plots in R.](https://www.statmethods.net/graphs/boxplot.html)
4. [Airbnb Superhost.](https://www.airbnb.com/how-do-i-become-a-superhost)
5. [A Gentle Introduction to XGBoost for Applied Machine Learning.](https://machinelearningmastery.com)
