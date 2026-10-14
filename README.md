# Temperature Forecasting Using RNN

A Deep Learning project that predicts the next day's temperature using a Recurrent Neural Network (RNN) trained on the Daily Delhi Climate dataset from Kaggle.

## Project Overview

Temperature forecasting is a time-series prediction problem because temperature values are related to previous observations.

This project uses a Simple Recurrent Neural Network to learn patterns from the previous 7 days of mean temperature and predict the temperature for the following day.

## Dataset

The project uses the **Daily Delhi Climate Time Series Data** dataset from Kaggle.

The dataset contains daily climate information from Delhi, including:

- Date
- Mean Temperature
- Humidity
- Wind Speed
- Mean Pressure

For this project, the `meantemp` column is used for temperature forecasting.

## Methodology

The project follows these steps:

1. Load the Kaggle climate dataset
2. Preprocess the temperature data
3. Normalize the temperature values using MinMaxScaler
4. Create sequences using the previous 7 days
5. Train a Simple RNN model
6. Evaluate the model on unseen test data
7. Compare actual and predicted temperatures
8. Calculate MAE and RMSE
9. Predict the next day's temperature

## Model Architecture

```text
Input
  ↓
SimpleRNN (50 units)
  ↓
Dense (25 units)
  ↓
Dense (1 unit)
  ↓
Predicted Temperature
```

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Google Colab
- Jupyter Notebook

## Evaluation Metrics

The model is evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

Lower values indicate better prediction performance.

## Project Files

```text
temperature-rnn/
│
├── Temp.ipynb
├── delhi_temperature_rnn.keras
├── temperature_scaler.pkl
├── README.md
└── .gitignore
```

## How to Run

1. Clone this repository.
2. Open `Temp.ipynb` in Google Colab or Jupyter Notebook.
3. Install the required Python libraries.
4. Upload the required dataset.
5. Run the notebook cells sequentially.

## Future Improvements

- Use additional weather features such as humidity and wind speed
- Experiment with LSTM and GRU models
- Add multi-day temperature forecasting
- Build a web-based prediction interface
- Integrate real-time weather data

## Author

**Mriganka Singh**

B.Tech — Cloud Computing and Machine Learning
