# Bike_Sharing_Demand_Prediction
![Screenshot 2023-08-30 123745](https://github.com/GauravUbhad/Bike_Sharing_Demand_Prediction/assets/143088895/ebc0f1a2-acb5-4201-baba-53351607c2c2)

# Project Summary
Bike sharing systems offer both local residents and tourists a convenient, cost-effective, and efficient mode of transportation within urban areas. Users have the flexibility to access bicycles from various bike stations scattered throughout the city. The aim of bike sharing is to establish itself as a dependable and straightforward form of public transportation. Its affordability is a significant draw for both locals and visitors. The dataset used for this project includes information from bike sharing programs like Seoul Bike and Capital Bikeshare, along with weather data for each hour.

The project's workflow begins with data exploration, encompassing tasks like dataset loading, identifying missing values, and assessing the data's general characteristics. Subsequently, the focus shifts to understanding the variables within the dataset. Data cleaning or data wrangling is then undertaken to ensure the dataset's quality and integrity.

Following data preparation, exploratory data analysis (EDA) is conducted to gain insights into the dataset and identify potential patterns or trends. Hypothesis testing is performed to validate assumptions and draw meaningful conclusions.

Once the data is preprocessed and thoroughly understood, the project proceeds to the implementation of a machine learning model, specifically a linear regression model. This model is trained with optimized hyperparameters using a repeated cross-validation approach. The testing set is employed to evaluate the model's performance. Various evaluation metrics such as R-squared and Root Mean Square Error are used to gauge the predictive accuracy of the regression models.

It's essential to note that the model's performance can vary depending on the time intervals used in data transformation, highlighting the importance of selecting appropriate temporal features for optimal results.

# Problem Statement
In the rapidly evolving landscape of urban mobility, These rental bikes offer the potential to reduce commuting wait times and facilitate fluid movement within cities. Yet,ensuring a consistent and timely availability of rental bikes to cater to the public's demand.

The heart of this challenge lies in the accurate anticipation of the precise number of rental bikes needed at every hour,as it directly influences the attainment of a reliable and stable supply of rental bikes across the city. A misalignment between bike availability and demand could lead to unwarranted waiting periods for users, hindering their mobility experience.

Effectively addressing this business problem necessitates the development of a robust prediction model that can forecast the required bike count for each hour. Such a model would be founded upon a complex interplay of factors including temporal patterns, day of the week, weather conditions, seasonal influences, and potential spikes due to special occasions or holidays.

The business problem revolves around the intelligent prediction of bike counts required on a hourly basis to ensure an uninterrupted and efficient supply of rental bikes.


# Data Description 
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information. Attribute Information:

Date: The date of the data entry.

Rented Bike Count: The number of bikes rented at the given date and hour.

Hour: The hour of the day when the data was recorded.

Temperature(°C): The temperature in degrees Celsius at the given date and hour.

Humidity(%): The humidity percentage at the given date and hour.

Wind speed (m/s): The wind speed in meters per second at the given date and hour.

Visibility (10m): The visibility in meters at the given date and hour.

Dew point temperature(°C): The dew point temperature in degrees Celsius at the given date and hour.

Solar Radiation (MJ/m2): The amount of solar radiation in megajoules per square meter at the given date and hour.

Rainfall(mm): The amount of rainfall in millimeters at the given date and hour.

Snowfall (cm): The amount of snowfall in centimeters at the given date and hour.

Seasons: The season corresponding to the date (e.g., Winter, Spring, Summer, Autumn).

Holiday: Whether it's a holiday on the given date (e.g., "No Holiday", "Holiday").

Functioning Day: Indicates whether it's a functioning day (e.g., "Yes", "No").


# Steps for Model Building

1- Reading and Understanding Data

2- Visualising variables

3- Data Preparation

4- Splitting the Data into Training and Testing Sets

5- Feature Scaling on the train data

6- Building the Model

7- Residual Analysis of the train data

8- Making predictions using final model

9- Model Evaluation


# Data Insights

Bike rental preferences are strongly influenced by weather conditions. People favor higher temperatures and lower humidity, avoiding rentals during rain or snow. Holiday periods witness decreased demand. Morning and evening peak demand suggests employees use bikes for commuting. Demand is highest in June, followed by July and May, but drops significantly during December, January, and February.

# Conclusion

In our analysis, we started by exploring our dataset thoroughly. First, we focused on our main target variable, 'Rented Bike Count,' and made some adjustments to it. Then, we examined categorical features and decided to drop those with a dominant majority in one category. We also delved into numerical features, checking their correlations, distributions, and how they relate to our target variable. Some of these numerical features had mostly zeros, so we removed them. Additionally, we applied label encoding and one-hot encoding to our categorical variables.

After this data preparation phase, we moved on to building predictive models using six different machine learning algorithms: Linear Regression, Lasso, Ridge, Elastic Net, Random Forest, and Gradient Boosting. To make our models perform their best, we fine-tuned their hyperparameters. This comprehensive analysis and modeling process aimed to help us understand and predict the number of rented bike counts effectively.






















