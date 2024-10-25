# Crypto Price Forecasting with LSTM Neural Networks

A comprehensive deep learning project that leverages Long Short-Term Memory (LSTM) neural networks to forecast cryptocurrency prices. This project focuses on building, training, and evaluating an LSTM model to predict price trends, utilizing historical data and time-series analysis techniques. Ideal for those interested in financial forecasting, machine learning, and time-series prediction models.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Project Structure](#project-structure)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Results](#results)
7. [Limitations and Future Work](#limitations-and-future-work)
8. [Contributing](#contributing)
9. [License](#license)

## Project Overview

This project aims to accurately predict cryptocurrency prices using historical data and deep learning models, specifically LSTM networks known for their effectiveness with time-series data. By leveraging historical data and adjusting hyperparameters, this model predicts trends that could be useful for financial analysis and strategic planning.

## Dataset

The data for this project includes historical closing prices of cryptocurrencies (e.g., Bitcoin, Ethereum). You can download this dataset from financial data sources such as:
- [CoinMarketCap](https://coinmarketcap.com/)
- [Yahoo Finance](https://finance.yahoo.com/)
- [CryptoDataDownload](https://www.cryptodatadownload.com/)

The dataset should be saved as `crypto_prices.csv` with at least a `Date` and `Close` column.

## Project Structure

```
├── data/
│   └── crypto_prices.csv      # Historical price data for cryptocurrencies
├── src/
│   ├── data_preprocessing.py  # Data loading and preprocessing scripts
│   ├── model_training.py      # Model creation, training, and evaluation
│   ├── predictions.py         # Prediction scripts
│   └── visualization.py       # Visualization of results
├── README.md                  # Project README file
└── CRYPTO_CURRENCY_FORECASTING_USING_LSTM.ipynb  # Project notebook
```

## Installation

Clone this repository and install the required dependencies.

```bash
git clone https://github.com/your-username/crypto-price-forecasting-lstm.git
cd crypto-price-forecasting-lstm
pip install -r requirements.txt
```

## Usage

1. **Data Preprocessing**: Run `data_preprocessing.py` to load and scale your data.
2. **Model Training**: Use `model_training.py` to set up and train the LSTM model.
3. **Predictions**: Use `predictions.py` to generate predictions based on the trained model.
4. **Visualization**: Execute `visualization.py` or view the plots in the notebook to visualize predictions.

### Running the Notebook

You can also run the project directly by executing the Jupyter Notebook `CRYPTO_CURRENCY_FORECASTING_USING_LSTM.ipynb` for a structured approach to data preprocessing, model training, and visualization.

## Results

The model's performance was evaluated using Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE). The results were as follows:

* Root Mean Squared Error (RMSE): 1751.87
* Mean Absolute Error (MAE): 1368.44

These metrics indicate that the model can closely approximate cryptocurrency price trends but still has some error, reflecting the inherent volatility of crypto markets. Below is an example plot comparing actual and predicted prices.

## Limitations and Future Work

Although this model achieves a reasonable level of accuracy, certain limitations exist:

* **Data Volatility**: Cryptocurrency prices are highly volatile, which may affect prediction accuracy.
* **Data Availability**: Limited historical data can impact the LSTM model's ability to learn patterns.

Future work may include:

* Experimenting with ensemble models or attention mechanisms
* Integrating external factors like trading volume and market sentiment
* Testing additional architectures, such as GRUs or Transformer models

## Contributing

Feel free to submit pull requests to improve the model, add more features, or enhance documentation. Please follow the Contributor Guidelines.

