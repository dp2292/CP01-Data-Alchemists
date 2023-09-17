# CP01-Data-Alchemists
## Dataset - Seoul Bike Trip Duration Prediction
## Team Id - 23
### Team Members:
| Name              | Student ID   | Contribution |
| ----------------- | ------------ | ------------ |
| Prarthee Desai    | 202001257    |              |
| Devansh Patel     | 202001262    |              |
| Dhruv Patel       | 202001271    |              |
| Krish Patel       | 202001452    |              |
| Jaykumar Navadiya | 202001465    |              |


## Project Overview

The Seoul Bike Trip Duration Prediction project aims to develop a data mining solution for predicting the trip duration of bike rentals in Seoul, South Korea. This project utilizes the "Seoul Bike Trip Duration" dataset, which contains various attributes related to bike rentals, weather conditions, and other environmental factors. By building a predictive model, we aim to assist bike rental services and riders optimize trip planning and resource allocation. 

In addition to predicting trip durations, our research delves into temperature forecasting for specific geographic locations. Utilizing various parameters from the dataset, we aim to predict ambient temperatures. This analysis provides insights into temperature variations and their relationships with environmental variables.

Accurately predicting trip duration is paramount across various modes of transportation, playing a pivotal role in advancing Intelligent Transport Systems (ITS) and traveler information systems. In this professional assignment, we leverage data mining techniques to forecast the trip duration of rental bikes within the Seoul Bike sharing system. Our prediction models are developed based on a comprehensive dataset that incorporates essential variables, including trip duration, trip distance, pickup, and dropoff geographical coordinates, as well as meteorological data such as temperature, precipitation, wind speed, humidity, solar radiation, snowfall, ground temperature, and 1-hour average dust concentration. This research seeks to contribute valuable insights into trip duration prediction, benefiting the optimization of transportation systems and enhancing the overall user experience in Seoul's bike-sharing network.

## Dataset Description

The dataset used in this project contains the following key attributes:

- **Duration**: The target variable representing the trip duration in seconds.
- **Distance**: The distance of the trip in meters.
- **Pickup and Drop-off Longitudes**: Longitude coordinates of the pickup and drop-off points.
- **Pickup and Drop-off Lattitudes**: Latitude coordinates of the pickup and drop-off points.
- **Haversine Distance**: The distance between two points on the Earth's surface based on the coordinates.
- **Temperature, Precipitation, Snow and Humidity**: Weather-related attributes that may affect trip duration.
- **Wind Speed, Solar radiation, Ground Temperature, and Dust Level**: Additional weather-related attributes.
- **Pickup and Drop-off Month**: Month of the pickup and drop-off for a trip.
- **Pickup and Drop-off Day**:  Day of the month of the pickup and drop-off for a trip.
- **Pickup and Drop-off Hour**: Hour of the day of the pickup and drop-off for a trip.
- **Pickup and Drop-off Minute**: Minute of the hour of the pickup and drop-off for a trip.
- **Pickup and Drop-off Week of the day**: Day of the week of the pickup and drop-off for a trip.

## Objectives

The primary objectives of this data mining project are as follows:

1. **Data Preprocessing**: Data preprocessing refers to the initial step in data analysis, where raw data is cleaned, transformed, and organized to make it suitable for further analysis and modeling. It involves handling missing values, dealing with outliers, standardizing data formats, and encoding categorical variables, ensuring that the data is usable and consistent before applying data mining or machine learning techniques.
2. **Exploratory Data Analysis (EDA)**: Exploratory Data Analysis (EDA) is visually and statistically analyzing a dataset to summarize its main characteristics, gain insights, and uncover patterns or anomalies. It involves techniques such as data visualization, summary statistics, and correlation analysis to understand better the data's structure, relationships between variables, and potential areas of further investigation in data analysis and modeling tasks.
3. **Feature Engineering**: Feature Engineering is the process of creating new, relevant, and informative features or transformations of existing ones from raw data to improve the performance of machine learning models. It involves selecting, combining, or transforming variables better to represent the underlying patterns and relationships in the data, ultimately enhancing the model's ability to make accurate predictions or classifications.
4. **Model Selection:**: Model Selection is the process of choosing the most suitable machine learning algorithm or model from a set of candidate models to best address a specific problem or task based on factors like performance, accuracy, and generalization ability.
5. **Model Training and Tuning**: Model Training and Tuning involves training a machine learning model on a dataset to learn patterns and relationships and then optimizing the model's hyperparameters to achieve the best possible predictive performance. This iterative process aims to find the most accurate and effective model configuration for a specific task.
6. **Evaluation Metrics**: Evaluation metrics are quantitative measures used to assess the performance or accuracy of a predictive model or algorithm by quantifying the degree of its predictions' agreement with the actual observed outcomes. These metrics help understand how well a model performs its intended task, whether predicting values, classifying data, or solving other machine learning and data mining tasks. Common evaluation metrics include Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), accuracy, precision, recall, and F1-score, depending on the specific task and context.

## Correlation Heatmap of the Data

![correlation_heatmap](https://github.com/dp2292/CP01-Data-Alchemists/blob/Prarthee/correlation_heatmap.png)

## Expected Outcomes
 - A predictive model capable of accurately estimating Seoul bike rentals' trip duration and temperature of a place.
 - Insights into the factors that most influence trip duration, including weather conditions, time of day, and seasonal variations.
 - Improved user experience for bike riders through more accurate trip duration and temperature predictions.

## Conclusion
1. In **predicting the trip's duration**, a thorough evaluation of machine learning models reveals that the **XGBoost Regressor** is the most favorable option among the other methods used, namely Linear Regression, Ridge Regression, Lasso Regression, ElasticNet Regression, XGBRgressor, Random Forest Regression and LGBMRegressor It demonstrates an adept ability to strike an appropriate equilibrium between effectively capturing the nuances of the training data and exhibiting robust generalization to the test data, resulting in a commendable overall predictive performance. The insights for each model are given below:
    - ElasticNet Regression: Train Score:  0.53 & Test Score:  0.54
    - Random forest Regression: Train Score 0.96 & Test Score 0.70
    - XGBoost Regressor: Train Score 0.78 & Test Score 0.77
    - LGBMRegressor: Train Score 0.75 & Test Score 0.75
- In **predicting the temperature**, we conclude from the provided scores that it might seem like Random Forest has the best performance because it has perfect scores of 1.00 for both the training and test sets. However, achieving perfect scores on training and test data is usually a sign of overfitting. Based on the provided scores, it's easier to conclude which model is the best with additional information or a more comprehensive evaluation. Models like XGBoost, LGBMRegressor, and ElasticNet, which have high scores but could be better, may be better choices as they are less likely to overfit and may have better generalization to unseen data. The insights for each model are given below:
    - ElasticNet Regression: Train Score:  0.94 & Test Score:  0.94
    - Random forest Regression: Train Score 1.00 & Test Score 1.00
    - XGBoost Regressor: Train Score 0.99 & Test Score 0.99
    - LGBMRegressor: Train Score 0.98 & Test Score 0.98
However, the choice between these models depends on various factors, including the specific problem you are trying to solve, the size and quality of your dataset, and computational resources.
