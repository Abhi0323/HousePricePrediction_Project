# HousePricePrediction_Project

Introduction:

In this project, we aimed to predict the prices of houses in Bengaluru based on various factors such as location, area, number of bedrooms, and other relevant factors. To do so, we used a dataset that contained information about various houses in the city. We used machine learning techniques to train a model that would predict the prices of houses based on the input variables.

Data Preparation:

To begin the project, we first loaded the dataset into a Pandas dataframe. We then explored the data by checking the shape of the dataframe, the columns present, and the types of data present in each column. We also checked for any missing data and removed it from the dataset. We then used feature engineering techniques to convert the 'size' column into a numerical feature that represents the number of bedrooms in each house.

Feature Engineering:

We also created a new column called 'sqft' by extracting the numerical values from the 'total_sqft' column. We then removed the 'total_sqft' column from the dataset since we did not need it anymore. Additionally, we calculated the price per square foot for each house by dividing the price by the area of the house. We then cleaned up the 'location' column by removing any extra spaces and grouping together any locations that had fewer than 10 houses.

Outlier Removal:

To ensure that our model was accurate, we removed any outliers from the dataset. We did this by grouping the data by location and then removing any data points that were more than one standard deviation away from the mean.

Visualization:

To help us better understand the dataset, we used various data visualization techniques. We created scatter plots of the price vs. the area for each location and number of bedrooms. We also created histograms of the price per square foot for each location. These visualizations helped us identify trends in the data and select the most important features to include in our model.

Model Building:

We used the scikit-learn library to build a linear regression model that predicts the price of a house based on the input variables. We split the data into training and testing sets and trained the model on the training set. We then evaluated the performance of the model on the testing set using various metrics such as mean squared error and r-squared.

Conclusion:

In conclusion, we successfully built a machine learning model that predicts the prices of houses in Bengaluru based on various features such as location, area, and number of bedrooms. We used data cleaning, feature engineering, and visualization techniques to preprocess the data and select the most important features for our model. We also removed any outliers to ensure that our model was accurate. Overall, this project serves as an excellent example of how machine learning techniques can be used to predict real-world phenomena.
