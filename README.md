# Aircraft Take-Off Weight Prediction

## About me
I am an aspiring Data Scientist and this project is part of my journey to gain practical experience in data analysis and machine learning. I welcome feedback and suggestions for improvement. Feel free to reach out or contribute to this project!

## Project Goal
The goal of this project is to develop a regression model that predicts the Take-Off Weight (TOW) of an aircraft based on various flight and operational parameters.

## Description of the Dataset
The dataset used in this project includes the following columns:
- **DepartureDate**: Date of departure
- **DepartureYear**: Year of departure
- **DepartureMonth**: Month of departure
- **DepartureDay**: Day of departure
- **FlightNumber**: Flight number
- **DepartureAirport**: Departure airport code
- **ArrivalAirport**: Arrival airport code
- **Route**: Route of the flight
- **ActualFlightTime**: Flight time
- **ActualTotalFuel**: Burnt fuel
- **ActualTOW**: Take-off weight (kg)
- **FlownPassengers**: Number of flown passengers
- **BagsCount**: Number of flown bags
- **FlightBagsWeight**: Weight of flown bags

## Project Overview
In this project, we aim to build and evaluate various regression models to predict the Take-Off Weight (TOW) of aircraft. The process involves data cleaning, feature extraction, exploratory data analysis, and model training and evaluation.

### Steps Involved:
1. **Data Import and Understanding**: Loading the dataset and understanding its structure and content.
2. **Data Cleaning and Preparation**: Handling missing values, converting data types, and extracting relevant features.
3. **Exploratory Data Analysis**: Visualizing the data to understand distributions, correlations, and outliers.
4. **Model Training and Evaluation**:
   - Building a Linear Regression model and evaluating its performance.
   - Building a Random Forest model and tuning it using GridSearchCV.
   - Filtering outliers and comparing model performance before and after filtering.
5. **Model Selection**: Selecting the best performing model based on error metrics.
6. **Prediction on Validation Data**: Using the best model to predict TOW on a separate validation dataset and saving the results.

## Key Findings
- **Linear Regression Model**: Filtering outliers significantly improved the performance of the linear regression model. The RMSE decreased from 1,130.25 to 775.79, indicating a better fit to the data.
- **Random Forest Model**: The Random Forest model performed better than the linear regression model before filtering outliers. The RMSE for the Random Forest model was 994.51. On the filtered data, the Random Forest model achieved an RMSE of 781.96.
- **Best Model**: The best model was the linear regression model after filtering outliers, with an RMSE of 775.79. This model was used to predict the Take-Off Weight on the validation data.

## Conclusion
This project demonstrates the process of building and evaluating regression models to predict aircraft take-off weight. By cleaning the data, performing exploratory analysis, and applying different modeling techniques, we identified the most effective model for our prediction task.

## Future Work
Further improvements can be made by exploring more advanced regression techniques, incorporating additional features, and conducting more extensive hyperparameter tuning.
