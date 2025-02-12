# Flight-Booking-Price-Prediction

## Overview
This project focuses on predicting flight ticket prices based on various factors such as airline, source city, destination city, departure time, stops, and days left for departure. By leveraging machine learning algorithms, the model provides insights into pricing trends and builds an accurate prediction system.

## Dataset
The dataset consists of 300,153 records with 11 attributes:
- **Airline**: Name of the airline
- **Flight**: Flight code
- **Source City**: Departure city
- **Destination City**: Arrival city
- **Departure Time**: Time of departure
- **Arrival Time**: Time of arrival
- **Stops**: Number of stops between source and destination
- **Class**: Seat class (Economy/Business)
- **Duration**: Travel time in hours
- **Days Left**: Days between booking and departure
- **Price**: Ticket price (target variable)

## Key Features
1. **Data Preprocessing**:
   - Handling missing values.
   - Encoding categorical features using One-Hot Encoding.
   - Feature selection using Variance Inflation Factor (VIF) to reduce multicollinearity.

2. **Exploratory Data Analysis (EDA)**:
   - Visualizing relationships between ticket price and features like airline, days left for departure, and number of stops.
   - Identifying pricing trends and patterns.

3. **Machine Learning Models**:
   - Linear Regression:
     - Root Mean Square Error (RMSE): 7259.93
     - Mean Absolute Percentage Error (MAPE): 34%
   - Decision Tree Regressor:
     - RMSE: 3620
     - MAPE: 7.7%
   - Random Forest Regressor:
     - RMSE: 2824
     - MAPE: 7.3%

4. **Model Evaluation**:
   - Metrics used include R² score, RMSE, MAE, and MAPE.
   - Random Forest achieved the best performance with the lowest error rates.

## Results
The Random Forest Regressor outperformed other models with an RMSE of 2824 and a MAPE of 7.3%, making it the most accurate model for predicting flight ticket prices.

## Conclusion
This project demonstrates how machine learning can be effectively applied to predict flight prices, providing valuable insights for both passengers and airlines. The Random Forest model's accuracy makes it a reliable tool for price prediction.
