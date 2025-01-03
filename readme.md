# PM2.5 Time-Series Prediction Using Machine Learning and Deep Learning

Air pollution, particularly PM2.5 (particulate matter smaller than 2.5 micrometres), poses severe risks to public health. This project aims to develop a machine learning model capable of forecasting PM2.5 concentrations using historical air quality and meteorological time series data. By providing actionable short-term forecasts, this predictive tool will help authorities and individuals manage air quality more effectively.

## Motivation

Accurate PM2.5 predictions are critical but challenging due to the complex, nonlinear nature of the data and the presence of noise and missing values. While traditional models like ARIMA handle linear relationships, they struggle with the intricacies of air quality forecasting. This project explores advanced ML and DL methods to address these challenges.

## Dataset

- **Source**: Hourly air pollutant and meteorological data from 12 monitoring sites in Beijing (2013-2017).
- **Metrics Evaluated**: 
  - R² Score
  - Mean Absolute Error (MAE)
  - Root Mean Square Error (RMSE)

## Methodology

1. **Baseline Models**:
   - Linear Regression
   - Random Forest Regression (tuned)

2. **Advanced Deep Learning Models**:
   - Long Short-Term Memory (LSTM)
   - Gated Recurrent Unit (GRU)
   - Recurrent Neural Networks (RNN)

3. **Hybrid Models**:
   - LSTM + Random Forest
   - GRU + XGBoost

## Results Summary

| Location                     | Metric | Linear Regression | Random Forest | LSTM  | LSTM+RF | XGBoost |
|------------------------------|--------|-------------------|---------------|-------|---------|---------|
| **Beijing**                  | R²     | 83.9              | 93.4          | 95.2  | 95.6    | 90.8    |
|                              | MAE    | 20.54             | 12.08         | 9.63  | 9.87    | 16      |
|                              | RMSE   | 32.04             | 18.22         | 16.63 | 17.67   | 24.81   |
| **Ahmedabad**                | R²     | 83.9              | 85.56         | 84.2  | 87.65   | 90.99   |
|                              | MAE    | 16.64             | 6.67          | 7.9   | 9.68    | 8.66    |
|                              | RMSE   | 29.18             | 16.74         | 12.11 | 22.74   | 18.91   |
| **Delhi**                    | R²     | 81.52             | 96.4          | 98.4  | 98.42   | 95.44   |
|                              | MAE    | 26.52             | 10.46         | 7.55  | 6.61    | 11.82   |
|                              | RMSE   | 40.68             | 17.61         | 10.96 | 11.15   | 19.8    |

*(Additional results for Hyderabad, Aizawl, Amaravati, Amritsar, Jorapokhar, Kochi, and Kolkata are included in a detailed report.)*

## Tools and Technologies

- **Programming Language**: Python
- **Libraries**: TensorFlow, Scikit-learn, XGBoost, PyTorch
- **Data Visualization**: Matplotlib, Seaborn
- **Models**: Linear Regression, Random Forest, LSTM, GRU, RNN, Hybrid Models

## Future Scope

1. **Real-Time Prediction Platform**:
   - Build a real-time platform for continuous PM2.5 monitoring.
   - Develop a user-friendly dashboard for visualizing air quality forecasts.

2. **Integration with IoT Devices**:
   - Incorporate real-time data from IoT-enabled air quality sensors.

3. **Expanded Geographical Coverage**:
   - Extend the model to more cities globally using diverse datasets.

4. **Enhanced Models**:
   - Experiment with transformers and attention mechanisms for further accuracy improvements.

5. **Public Awareness Tools**:
   - Create mobile applications to alert users about air quality and suggest preventive measures.
