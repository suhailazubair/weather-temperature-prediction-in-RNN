#  🌦 weather-temperature-prediction-in-RNN
Weather Temperature Prediction using SimpleRNN and TensorFlow. The model forecasts future temperatures from historical weather data using sequence-based deep learning.


## Project Overview

This project uses a Recurrent Neural Network (SimpleRNN) to forecast the next day's temperature based on historical weather conditions. The model learns patterns from previous weather observations and predicts future temperatures.

---

## Objective

To design, implement, and evaluate a SimpleRNN model for weather temperature forecasting using historical weather data.

---

## Dataset

Daily Weather Dataset

### Features Used

- Temperature (C) (Target Variable)
- Humidity
- Wind Speed (km/h)

Optional features available:

- Pressure (millibars)
- Visibility (km)
- Cloud Cover

---

## Project Workflow

### 1. Data Understanding

- Load dataset
- Display first 10 rows
- Check missing values
- Plot temperature trend

### 2. Data Preprocessing

- Handle missing values
- Normalize data using MinMaxScaler
- Create sequential data (7 previous days)
- Split into training, validation and test sets

### 3. Model Development

SimpleRNN Architecture:

Input Layer
↓
SimpleRNN (64 units)
↓
Dropout (0.2)
↓
Dense Layer (1 unit)
↓
Temperature Prediction

---

## Model Configuration

| Parameter | Value |
|------------|-------|
| Sequence Length | 7 Days |
| RNN Units | 64 |
| Dropout | 0.2 |
| Optimizer | Adam |
| Loss Function | Mean Squared Error |
| Metric | Mean Absolute Error |
| Epochs | 50 |
| Batch Size | 32 |

---

## Evaluation Metrics

The model performance is evaluated using:

- RMSE (Root Mean Square Error)
- MAE (Mean Absolute Error)
- R² Score

---

## Forecasting

The trained model predicts the temperature for the next 7 days and visualizes the forecast against recent historical temperatures.

---

## Technologies Used

- Python
- Google Colab
- TensorFlow/Keras
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn

---

## Results

The model successfully learns temporal patterns in weather data and provides reliable temperature predictions using SimpleRNN.

---

## Repository Structure

```
RNN-Weather-Temperature-Prediction
│
├── README.md
├── RNN_Weather_Temperature_Prediction.ipynb
├── daily_weather.csv
├── requirements.txt
└── images/
```

---

## Future Improvements

- LSTM Networks
- GRU Networks
- Hyperparameter Tuning
- Multivariate Forecasting
- Longer-term Weather Prediction

---

## Author

Suhaila P T

B.Sc Computer Science

Skills:
Python | Machine Learning | SQL | TensorFlow | Pandas | Flask | Power BI

GitHub:
https://github.com/suhailazubair
