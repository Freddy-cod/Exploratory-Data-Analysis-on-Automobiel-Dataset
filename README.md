
# Exploratory Data Analysis on Automobile Dataset .

The purpose of this project is analyising autombile data so 
as to extract usefull insights and trends in the autombile
industry . Thus , the project only focuses on Exploratory Data Analysis . 

### What data is being analysed ?

The dataset contains data about cars. It has the details of different set of cars with its properties and functionalities. There are 205 car entries and 26 columns (features) in the dataset, however the analysis will not focus on every single feature but a few answering the questions we seek from the data.
The data is basically divided into categorical and numerical forms of data. Thus its datatypes are either of object (strings), integers or floats. The data contains missing values and some inconsistencies and deserves to be cleaned. It only occupies memory of 41 kb .


### How the data is being analysed ?
Before tackling issues to do with analysis i cleaned the data .
### Data Cleaning 
Firstly I changed the datatypes, to types that can be used for comparison and analysis. For this reason , I created two functions that convert columns into integers and floats .The normalized losses , engine-size, wheel-base, bore, price columns were of string datatype and were changed into integers and some into floats .

Secondly I renamed some rows within columns so that they can be consistent. The drive-wheel column‘s records were renamed because the data points were not consistent e.g. fwd appearing as 4wd in some cases.

For efficiency reasons I dropped columns like normalized losses as they will not be used in our EDA .





### Missing data 

The first missing data was found on the normalized column .Instead of a numbers there where question marks. I handled this missing value by replacing the marks by zeros .
I used a module called ‘missingno’ to visualize the missing data. When used, it revealed that there are no any other missing values that we should take care of.


### Data analysis 
### What are the main findings ?

The first graph shows the data distribution of car prices. A distribution plot and a boxplot is used for this purpose. It shows us mean, median, mode and the interquartiles of the data. In this case, mode is at 10000, the mean at 1249 and the median 10198. These two graphs also shows us some outliers within the car prices dataset, there are few cars costing over 4000, the majority of the cars cost between 900 and 1500.


The second graph seeks to understand the relationship between the horsepower of a car and its engine size using a scatterplot. The plot reveals that the lesser the engine size the lesser the horsepower. Thus it can be concluded that from this dataset, if a car has a bigger engine size. , the more the horsepower it will have.

Is there a relationship between the price of a car and the size of its horsepower? .Using a scatter plot, we were able to answer this question. Car with higher horsepower are more expensive than the cars with lower horsepower. More so, it seems to be the case that the engine size has a strong correlation with prize. The bigger the engine size the higher the prize of the car.

Symbolling shows us how risky a car is , -3 indicates that a car is safe and 3 indicate that its risky .Wheel base is the horizontal distance between the centers of the front and rear wheels. . The question is, How risky is a car given its wheelbase? The scatterplot shows that as the wheelbase decreases, symbolling values tends to be risky. Thus a car with higher wheelbase will be safer compared to the one with smaller wheelbase.

Is there any relationship between wheelbase, highway-mpg and city-mpg? From the analysis and the graph visualization highway mpg has a strong correlation with city mpg. A car with more city mpg has more highway mpg. However the price of a car with higher city mpg is low. Expensive cars have low city mpg and cheap cars have more, with the majority between 30 – 40 city mpg for a price ranging from 1000 to 2000.

Can we figure out the most peak-rpm? Through a distribution plot I managed to figure out that the most peak rpm of the cars in the dataset is between 5000 and 5900. RPM stands for revolutions per minute and it’s how fast the engine of a car is spinning. This has implications on both performance and fuel efficiency of the car. 

To understand the statistical distribution of our data with regards to compression ration I used the box plot. Most cars have an average compression ratio of 9. This It helps understand the outliers in our data. We have cars that have a compression ratio as high 22, these are outliers because the average ratio is between 8 and 10. Also, this graph help us to measure the IQR, the mode and the median of the compression ration data. This data can help us in decision making perhaps in engineering, because a high compression ratio is desirable as it allows an engine to extract more mechanical energy.

Can we determine which body style is expensive in our data set? Using a bar graph we can determine this. From the graph we can see that hardop is the most expensive body style costing 4500, whereas hatchback is the least expensive body style.

What is the most expensive car make?.  A bar graph easily answers this question showing us that the most expensive car make is Mercedes Benz costing over 4000 followed by BMW. On the flip side, Chevrolet is the cheapest car in our dataset. This helps us understand how the price distribution is in relation to car make. After figuring out which one is the most expensive car, can we safely conclude that the most expensive car is the most popular?

A bar graph help us dissolve this assumptions .Even though Mercedes Benz is the most expensive car , Toyota is the most popular car and mercury is the least popular .Most expensive seem not to be popular perhaps due to the fact that most people can’t afford them . Whereas cars which are moderately affordable like Toyota seems to be popular.
 
Lastly which is the most fuel type used by the cars on our dataset , it seems that most fuel type used is gas . Over 170 cars use gas, whereas about 24 cars use diesel. This can help in deciding which fuel should be invested in.

## Acknowledgements

 - [Analytics Vidhya](https://www.analyticsvidhya.com/blog/2020/08/exploratory-data-analysiseda-from-scratch-in-python/)
 - [SatyamDG](https://medium.com/@gsatyam625/extracting-insights-from-car-sales-data-using-eda-72d341267f22)
 

  
## Authors

- [@Freddy-cod](https://github.com/Freddy-cod)

  
## Tech Stack

Python , Numpy , Pandas , Matplotlib  


  