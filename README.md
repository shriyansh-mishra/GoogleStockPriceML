# GoogleStockPriceML

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)

</div>

A machine learning project to predict Google stock prices using both classical ML (Random Forest) and deep learning (LSTM) models. Includes data preprocessing, feature engineering, model training, evaluation, and investment simulation.

## Workflow Overview

1. **Data Loading**
   - Historical Google stock price data (2015–2024) is loaded from a CSV file using pandas, with dates parsed and sorted chronologically.

2. **Data Preprocessing**
   - Missing values are handled and date features (year, month, day) are extracted to help the model learn seasonal patterns.

3. **Feature Engineering**
   - Additional features such as lagged closing prices and moving averages are created to provide more context about recent trends.

4. **Train-Test Split**
   - The dataset is split chronologically: the first 80% for training, the last 20% for testing, ensuring evaluation on unseen future data.

5. **Model Building and Training**
   - Two approaches are explored:
     - **Classical ML:** Random Forest Regressor trained on engineered features.
     - **Deep Learning:** LSTM (Long Short-Term Memory) neural network built with TensorFlow/Keras, using sequential data for time series prediction.

6. **Model Evaluation**
   - Predictions are compared to actual prices using RMSE, MAE, and R² metrics, calculated after inverse-transforming scaled predictions.

7. **Visualization**
   - Plots show actual vs. predicted prices over time.
   - An investment simulation visualizes how an initial investment would grow over a chosen period based on model predictions.

---

*For educational and research purposes only. Not financial advice.* 
