
# 📈 Cracking the Market Code: AI-Driven Stock Price Prediction Using Time Series Analysis

This project explores AI-driven stock price prediction using Microsoft (MSFT) stock data, focusing on preprocessing techniques and time series modeling to forecast future prices.

---

## 📂 Dataset

- **Source**: [Kaggle - Microsoft Stock Data](https://www.kaggle.com/)
- **File Used**: `MSFT.csv`
- **Cleaned File**: [`MSFT_cleaned_scaled.csv`](MSFT_cleaned_scaled.csv)

---

## 🧹 Preprocessing Steps

1. **Missing Values**  
   - Forward-fill (`ffill`) method  
   - Dropped any remaining nulls

2. **Duplicates**  
   - Identified and removed duplicate rows

3. **Outliers**  
   - Z-score method (threshold = 3)

4. **Scaling**  
   - MinMaxScaler applied to all numeric features

---

## 📊 Features in Cleaned Dataset

| Feature     | Description                    |
|-------------|--------------------------------|
| Date        | Trading date                   |
| Open        | Normalized opening price       |
| High        | Normalized highest price       |
| Low         | Normalized lowest price        |
| Close       | Normalized closing price       |
| Adj Close   | Adjusted closing price         |
| Volume      | Normalized trading volume      |

---

## 💡 Objective

To use this cleaned and normalized data for training time series models like:
- LSTM (Long Short-Term Memory)
- GRU (Gated Recurrent Units)
- ARIMA / SARIMA

---

## 🚀 Getting Started

1. Clone this repository
2. Load `MSFT_cleaned_scaled.csv` in your Python script
3. Use it for exploratory data analysis or model training

```python
import pandas as pd
df = pd.read_csv('MSFT_cleaned_scaled.csv')
```

---

## 📈 Example Visualization

![Price Trend](docs/normalized_close_price.png)

---

## 🔧 Tools Used

- Python, Pandas, NumPy
- Scikit-learn (MinMaxScaler)
- Matplotlib & Seaborn (Visualization)

---

## 📝 License

MIT License - use this project freely for educational or research purposes.
