### King County House Sales With Multiple Linear Regression
### Author: Paul Mbuitu Muriithi

### Overview
Understanding the mechanisms that drive house prices is essential since the real estate market is a complicated ecology driven by a variety of factors. The purpose of this study is to employ multiple linear regression modeling to delve into the world of house sales analysis in King County. The correlations between different features and the sale prices of homes in the area will be investigated utilizing the power of data analysis and machine learning techniques so that they may be used by a housing development firm to make lucrative judgments.

### Business Problem
The stakeholders are searching for the qualities that lead to higher home sale prices. The aim is to develop an accurate and reliable multiple linear regression model by leveraging the King County House Sales dataset, a model that can predict house prices based on various independent variables.

### Main Objective
To develop an accurate and reliable multiple linear regression model that can predict house prices based on various independent variables.

### Specific Objectives
* To find out which attributes have a significant impact on house prices in ing County.
* To find out the relationship between the independent variables and the sales prices of houses.
* To find out how accurately house prices can be predicted using the available attributes.

### Hypotheses
* **Null hypothesis(Ho):** There is no relationship between our features and our target variable, price.
* **Alternative hypothesis(Ha):** There is a relationship between our features and our target variable, price.

A significance level (alpha) of 0.05 will be used to decide if to reject or fail to reject the null hypothesis.

If the p-value is lower than the significance level, it is considered statistically significant, and we reject the null hypothesis.

### Notebook Structure
* Data Collection
* Read and check the data
* Cleaning the data
* Exploratory Data Analysis
* Modelling
* Recommendations, Conclusions, and Next Steps.

### Data Understanding
* King County House Data will be used. The file contains data for 21,597 homes built in King County from 1900 to 2015. Each home in the set contains information regarding features such as number of bedrooms/bathrooms, number of floors, square footage, zipcode, condition of the house, year when house was built and more.

### Data Wrangling
From the datasets used, only some features and rows were considered relevant to the process. Therefore, in this step, the features that are not required from the dataset were dropped. 

### Exploratory Data Analysis and Modelling
Outliers in our price for houses was checked. Absolute outlires was considered to be any price above 5 million and they were dropped.
<img src = 'images\output_1.png' />


Corrrelations between our feautures was found. A heatmap was generated to display correlations DataFrame.
<img src = 'images\output_2.png' />


The relationship between out target variable, price, and the predictors, independent variables, was determined.
<img src = 'images\output _3.png' />


Residuals, differences between the predicted values and the actual values in the final model was found. This plot provides insights into the distribution of the residuals, helping to assess if they follow a normal distribution and detect any patterns or outliers.
<img src = 'images\output_5.png' />


### Results
* The multiple linear regression model built has an **R-squared value of 0.825**, which indicates that the model can explain **83%** of the variance of the markethouse sale prices which is a good sign that the model is effective in predicting the prices.
* For an average house and its overall grade related to the construction and design of the **house being poor**, **no waterfront** and being at **zipcode_98001**, we would have a sale price of **1,084,000 dollars**.
* The model is **off** by about **91,226 dollars**.
* All of the available features are impactful for inferring and predicting house sale prices and can be considered by home developers in order to increase selling price.

### Recommendations*
* Increase square-footage of living space.
* Attain the highest possible building condition.
* Attain the highest possible building grade.

By following the above recommendations, a housing development company in King County can increase its chances of selling higher-priced homes.

### Conclusions
* The prob(F-statistic) of 0.00 tells us that there is an extremely low probability of achieving these results with the null hypothesis being true, and tells us that our regression is meaningful. Our p-values for our features are well below our alpha or significance level, showing that they are each contributing to the model significantly. With an alpha of 0.05, at a confidence level of 95%, we reject the null hypothesis that there is no relationship between our features and our target variable, price.
* There are some limitations to the model. To meet regression assumptions, we had to try out log-transformation on certain variables. Therefore,any new data used with the model would require similar preprocessing. Additionally, since housing prices vary regionally, the model's usefulness for datafrom other counties may be restricted.

### Next Steps
* In the future, reducing noise in the data to improve the accuracy of our model is needed. 
* Additionally, it is good to investigate certain features, such as proximity to a top school and coffee shop to see what trends could be discerned from that.