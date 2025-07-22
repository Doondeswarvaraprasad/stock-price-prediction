
# 📈 Stock Price Prediction using GRU, LSTM, and ARIMA

This repository presents a complete project on time series stock price forecasting using both traditional statistical and deep learning approaches. The aim is to explore and compare the performance of ARIMA, LSTM, and GRU models on historical stock price data.

---

## 📚 Project Overview

Stock market forecasting is a crucial financial task, and this project addresses it using various methods:

- **ARIMA**: A classic time series forecasting model
- **LSTM**: A deep learning model capable of learning long-term dependencies
- **GRU**: A lighter and often faster alternative to LSTM

The notebook includes:
- Data preprocessing & scaling
- Time series sequence generation
- Model training and evaluation
- Visualization of predictions
- Model comparison

---

## 🔧 Models Used

| Model | Description                    | MSE (Test)   |
|--------|-------------------------------|--------------|
| ARIMA  | Traditional statistical model | **0.2541** 📉 |
| LSTM   | Deep learning RNN model       | **0.1427** ✅ |
| GRU    | Efficient RNN variant         | **0.1729** ✅ |

> ✅ Lower MSE indicates better performance. LSTM performed best.

---

## 📁 Folder Structure

```
stock-price-prediction/
├── Stock_price_prediction.ipynb  # Main colab notebook
├── README.md                     # Project description and instructions
├── requirements.txt              # Python dependencies
├── .gitignore                    # Files to exclude from Git tracking
└── data/                         # (Optional) Dataset folder
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Doondeswarvaraprasad/stock-price-prediction
cd stock-price-prediction
```

### 2. Install Requirements

```bash
pip install -r requirements.txt
```

### 3. Launch the Notebook

```bash
COLAB notebook Stock_price_prediction.ipynb
```

> You can also use Google Colab by uploading the notebook.

---

## 📊 Sample Output

Each model's performance is visualized with matplotlib/seaborn to show how well predicted values match actual stock prices.

> Add your own output images or graphs if needed.

---

## 📥 Data Source

This project assumes historical stock data is sourced from:

- **Yahoo Finance** using `yfinance`
- OR a pre-downloaded CSV file with columns like `Date`, `Open`, `Close`, etc.

Make sure the dataset is properly scaled using `MinMaxScaler` before training models.

---

## 🧪 Dependencies

The project uses the following libraries:

```
numpy
pandas
matplotlib
seaborn
scikit-learn
tensorflow
statsmodels
notebook
```

Install them via:

```bash
pip install -r requirements.txt
```

---

## 📜 License

This project is licensed under the **MIT License** — feel free to use, modify, and distribute.

---

## 🙋‍♂️ Author

**Doondeswara Vara Prasad**  
GitHub: [Dondeswarvaraprasad](https://github.com/Doondeswarvaraprasad)

---

## ✅ Future Improvements

- Hyperparameter tuning for all models
- Add early stopping & cross-validation
- Try other models like Prophet, XGBoost, or CNNs
- Deploy predictions via Streamlit or Flask
