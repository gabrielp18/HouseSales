# Property Buyer
![pic](https://github.com/gabrielp18/HouseSales/blob/main/img/at.jpg?raw=true)  
*The complete analysis is in the notebook.*
  
  
# The business
A new real estate buying and selling startup decided to enter the market in a new region, King Country – USA.  
To optimize the performance of this startup, we were tasked with carrying out an analysis of the properties available
in that region and developing a machine learning method to predict the price of future properties with similar characteristics in this region.  
In addition, the startup's CEO would like a simulation of potential properties to be bought and resold.

# Business Criterion
The startup is focused on residences, so we were asked not to consider properties that present characteristics of being warehouses, commercial rooms and offices.

# Business Problems
The hypotheses formulated were formulated based on possible influences on the price.
1. The number of bathrooms, rooms and floors can influence the price variation?
2. The characteristic of the property being in front of the water, how can it influence the price?
3. Does the property classification influence the price?
4. Does the condition of the property exert what weight on the property's value?
5. Does the size of the land, the house built, the upper floors and basement influence the price? In what way?
6. Does the year of construction influence the price? Does the price of homes vary from year to year? And does the retirement year also exert the same influences?
7. What is the sales behavior?
8. Does the region where the property is located influence the price?
9. Which type of property has the highest cost?
10. What are the best times to sell properties?
11. What is the result of machine learning?

# Insights
1. Properties with 2 bathrooms are in greater quantity. However, properties that have 5 bathrooms have a median higher than the others of 113%.  
![bathrooms](https://github.com/gabrielp18/HouseSales/blob/main/img/2.png?raw=true)  
The 3 bedroom properties are in greater quantity when compared to the others (1-7 bedrooms), presenting a median 40% higher than the other properties.
It is expected that with the increase in rooms there will be an increase in price, however for properties with 7 bedrooms there was a 5% reduction in the median price.  
![bedrooms](https://github.com/gabrielp18/HouseSales/blob/main/img/1.png?raw=true)  
With the increase in floors, an increase in house prices was expected, but the results obtained are somewhat divergent. 
Houses with 2.5 floors (2 floors + basement) have the highest median prices, with a cumulative 41% of prices, but represent only 0.5% of all properties present.
Properties with 3 floors have a lower median than properties with 2 floors, and 50% of properties have only 1 floor.
![floor](https://github.com/gabrielp18/HouseSales/blob/main/img/15.png?raw=true)  
  
2. More than 90% of the properties are not located near the region with water, however, 
the properties close to the water have a median higher than 200% when compared to properties outside this region.  
![waterfront](https://github.com/gabrielp18/HouseSales/blob/main/img/5.png?raw=true)  
  
3. The properties with rating 7 are in greater quantity, followed by ratings 8 and 9. 
This gives us an assumption that the properties are in good condition due to the evaluation carried out. 
As expected, the properties with the highest rating, 12, 11 and 10, have a median greater than 100% when compared to the other properties.  
![grade](https://github.com/gabrielp18/HouseSales/blob/main/img/3.png?raw=true)  
  
4. In line with the results for the classification, most of the properties are in condition 3, being in the median level of classification. 
Also as expected, the higher the condition, the higher the price of the property, where the highest rating, 5, has a median higher than 44% over the other properties.  
![condition](https://github.com/gabrielp18/HouseSales/blob/main/img/4.png?raw=true)  
  
5. The three characteristics in relation to the size of the property (sqft_living, and sqft_above) positively influence the price, 
since these features are the ones that most correlate with the price.  
![corr](https://github.com/gabrielp18/HouseSales/blob/main/img/19.png?raw=true)  
  
6. Among all the properties investigated, more than 22% of them were built between 2010 and 2015.  
![houseyear](https://github.com/gabrielp18/HouseSales/blob/main/img/6.png?raw=true)  
95% of the properties do not have renovations and the year that presented the greatest amount of renovations was the year 2010.  
![reno](https://github.com/gabrielp18/HouseSales/blob/main/img/10.png?raw=true)  
Interestingly, the properties that presented a higher accumulated value after the renovation were the properties dated in 1956, with a median higher than the others.
  
7. In a more in-depth analysis, it can be noted that 67% of the homes were sold in 2014 with a total gross revenue of 6 billion. 
However, the year 2015 presented a median higher than that of 2014, which may show that this year there was a sale of higher cost properties.  
![yearsell](https://github.com/gabrielp18/HouseSales/blob/main/img/7.png?raw=true)  
It was possible to observe a sales trend in the months of the year. 
The highest percentage of sales occurs between April and July, where all 4 months had a median higher than the other months and also higher gross revenue, reaching 1 billion.  
![month](https://github.com/gabrielp18/HouseSales/blob/main/img/8.png?raw=true)  
As expected, properties sell more on weekdays, with weekends selling less than 2%. The biggest selling days were Tuesdays and Wednesdays. 
It is interesting to note that Saturday was the day when there was the highest median price. 
The highest accumulated gross revenue occurred on Tuesday, with an accumulated 2 billion.  
![day](https://github.com/gabrielp18/HouseSales/blob/main/img/9.png?raw=true)  
Finally, the seasons seem to have some influence on property sales, with a percentage of 30% in spring, with an accumulated sales value of 3 billion.  
![season](https://github.com/gabrielp18/HouseSales/blob/main/img/11.png?raw=true)  
  
[To see the price grow over the years, Click here]((https://gabrielp18.github.io/HouseSales/image1.html)  
  
8. You can see regions that have a high property price through thedata by ZIPCODE. That region is Seattle, which makes up King Country County.  
[Click to see the distribution of price in King Country, with max price at 1M](https://gabrielp18.github.io/HouseSales/image2.html)
  
9. The properties were divided into three categories: houses, apartments and Kitnet (Studio). 
Kitnet were considered all properties with 1 bedroom, apartment between 2 and 3 bedrooms and houses all properties with 4 bedrooms or more.  
Note that 59% of properties fall under the apartment classification, and this is to be expected due to a metropolitan city.  
![counttype](https://github.com/gabrielp18/HouseSales/blob/main/img/18.png?raw=true)  
In addition, the houses have a higher median price, also expected due to the size of the properties compared to the other two.  
The cumulative sales value is higher for apartments, with a total of 5 billion.
![type](https://github.com/gabrielp18/HouseSales/blob/main/img/17.png?raw=true)  
  
10. A greater purchase behavior can be observed in the months of April and July, on weekdays between Tuesday and Wednesday. 
Spring is the season that presented the highest level of accumulated sales, however this season encompasses 4 months in total, 
and with a more assertive focus on the best times for sale, those of the months can bring better results.  
![compare](https://github.com/gabrielp18/HouseSales/blob/main/img/12.png?raw=true)  
  
11. Two algorithms with different feature selection were tested.
The first model tested was the linear regression model, where the maximum result presented was r2 = 0.90 and MSE 68061. 
These data obtained by the model were in agreement with the values ​​obtained statically by OLS.
The model that presented the best result was the XGBRegressor, with a score of 99%, however the MSE = 175844
