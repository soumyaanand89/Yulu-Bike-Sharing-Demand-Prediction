
# Bike Sharing Demand Prediction

This repository contains a machine learning project that predicts bike rental demand based on various features, such as weather conditions, time of day, and environmental factors. The model utilizes ensemble methods like Bagging Regressor and Random Forest Regression for superior predictive accuracy, providing key insights for improving business operations in bike-sharing services.

## Project Overview

The goal of this project is to predict the number of bikes rented in a shared bike system. By analyzing data on bike rentals and related factors, this model helps in forecasting demand, allowing businesses to optimize operations such as fleet management and resource allocation.

### Key Features:
- Predictive modeling using Bagging Regressor, Random Forest, and Linear Regression.
- Comprehensive data analysis including weather, temperature, and time factors.
- Insights on seasonality, hourly trends, and impact of weather conditions on bike rentals.
- Evaluation of outliers, including extreme weather events that impact rental patterns.

## Dataset

The dataset contains features like:
- **Rented_Bike_Count**: Number of bikes rented per hour.
- **Hour**: Time of day (0-23).
- **Temperature**: Real-time temperature in degrees Celsius.
- **Humidity**: Real-time relative humidity.
- **Wind_Speed**: Real-time wind speed in m/s.
- **Visibility**: Real-time visibility in meters.
- **Solar_Radiation**: Solar radiation in MJ/m².
- **Rainfall**: Rainfall in mm.
- **Snowfall**: Snowfall in cm.

### Data Preprocessing:
- Handling missing values.
- Encoding categorical variables.
- Outlier detection and treatment.
- Feature scaling for numerical variables.

## Exploratory Data Analysis (EDA)

The EDA reveals trends such as:
- Bike rentals are higher in summer than in winter.
- Rental counts peak during certain hours of the day.
- Temperature and wind speed significantly impact rental counts.
- Holidays do not show an increase in bike rentals compared to non-holidays.

## Machine Learning Models

The project uses three machine learning models for predicting bike rentals:

1. **Bagging Regressor**:
   - Outperforms other models in predictive accuracy.
   - Shows the lowest error metrics (MSE, MAE, RMSE).
   - Best suited for capturing complex relationships in the data.

2. **Random Forest Regression**:
   - Performs well but slightly less accurate than Bagging.
   - Useful for understanding feature importance.

3. **Linear Regression**:
   - Exhibits the lowest R² score and the highest errors.
   - Not suitable for this task due to poor performance on capturing non-linear patterns.

## Model Evaluation Metrics

- **R² (Coefficient of Determination)**: Indicates the proportion of variance captured by the model. Higher values signify better predictions.
- **MSE (Mean Squared Error)**: Measures average squared differences between predicted and actual values. Lower values are better.
- **MAE (Mean Absolute Error)**: Average absolute differences between predicted and actual values.
- **RMSE (Root Mean Squared Error)**: Similar to MSE but penalizes larger errors more strongly.
- **Cross-Validation**: Used to ensure model generalization across different subsets of data.

## Insights

- **Seasonality**: Bike rentals are higher in summer and lower in winter.
- **Hourly Trends**: Rentals peak during specific hours, especially in the early morning and late afternoon.
- **Weather Impact**: Wind speed and temperature are significant predictors of demand.
- **Outliers**: Unusual conditions like heavy snowfall or extreme rainfall lead to unpredictable rental patterns, impacting overall resource allocation.

## Business Impact

By using this model, bike-sharing services can:
- Optimize fleet availability during peak hours and seasons.
- Allocate resources effectively by predicting demand under various weather conditions.
- Reduce costs associated with maintenance, storage, and staffing.
- Improve customer satisfaction by ensuring better bike availability during high-demand times.

## How to Run the Project

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/bike-sharing-demand-prediction.git
   cd bike-sharing-demand-prediction
   ```

2. **Install the required libraries**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Jupyter Notebook**:
   Open the notebook to explore data preprocessing, EDA, and model building.
   ```bash
   jupyter notebook bike_sharing_demand.ipynb
   ```

## Future Enhancements

- Include additional data sources (e.g., traffic patterns, holiday events).
- Experiment with more advanced ensemble methods like Gradient Boosting and XGBoost.
- Deploy the model using Flask or Streamlit to create an interactive web application for real-time predictions.

## Conclusion

This project demonstrates how machine learning can predict bike rental demand based on environmental and temporal factors. The Bagging Regressor provides the most accurate results, enabling better operational decisions for bike-sharing services, leading to increased efficiency, cost reduction, and improved customer satisfaction.

---

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
