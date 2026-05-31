<!-- ============================================================ -->
<!-- 🔮  SafeStock AI — Intelligent Stock Forecasting System       -->
<!-- ============================================================ -->

<div align="center">

# 🔮 SafeStock AI
### Intelligent Stock Forecasting System

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-App-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

> AI-powered 5-day stock price prediction using LSTM deep learning,
> real-time Yahoo Finance data, and an interactive Streamlit dashboard.

</div>

---

## 📌 Overview

**SafeStock AI** predicts the closing prices of 7 major US tech stocks for the
next 5 trading days using pre-trained LSTM (Long Short-Term Memory) neural networks.
It fetches live market data, engineers financial indicators, and serves everything
through a clean two-tab Streamlit interface — forecast + technical dashboard.

> ⚠️ **Disclaimer:** For research and educational purposes only.
> Not financial advice.

---

## ✨ Features

| Feature | Details |
|---|---|
| 🤖 Deep Learning | LSTM models trained per stock (TensorFlow / Keras) |
| 📡 Live Data | Yahoo Finance via `yfinance` — last 3 months |
| 🧮 Feature Engineering | OBV, MACD, EMA, Garman-Klass Volatility, Dollar Volume |
| 📈 5-Day Forecast | Predicted adjusted closing prices + % change insight |
| 📊 Dashboard | Interactive Plotly charts — SMA, EMA, RSI, OBV, Bollinger Bands |
| 🎯 9 Tickers | AAPL, AMZN, GOOG, INTC, META, MSFT, TSLA, AMD, NVDA |

---

## 🗂️ Project Structure

```
Intelligent-Stock-Forecasting-System/
│
├── models/                          # Pre-trained LSTM model files (.h5)
│   ├── Apple_Model.h5
│   ├── Google_Model.h5
│   ├── 3rd-Tesla-LSTM-Model.h5
│   ├── Amazon-LSTM-Model.h5
│   ├── Intel-2nd-LSTM-Model.h5
│   ├── Meta-LSTM-Model.h5
│   └── Microsoft-LSTM-Model.h5
│
├── streamlit_app.py                 # Main application
├── requirements.txt                 # Python dependencies
└── .streamlit/                      # Streamlit config
```

---

## 🛠️ Tech Stack

```
Deep Learning  →  TensorFlow 2.x + Keras (LSTM)
Data Source    →  Yahoo Finance (yfinance)
Features       →  NumPy · Pandas · Scikit-learn
Web App        →  Streamlit
Visualization  →  Plotly
```

---

## ⚙️ Setup

```bash
# 1. Clone the repo
git clone https://github.com/NEDESH-KUMAR-M/Intelligent-Stock-Forecasting-System.git
cd Intelligent-Stock-Forecasting-System

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the app
streamlit run streamlit_app.py
```

---

## 🔍 How It Works

```
1. Fetch       →  Last 3 months of OHLCV data from Yahoo Finance
2. Engineer    →  Compute OBV, MACD, EMA, volatility & volume features
3. Scale       →  Min-Max normalization (0 → 1)
4. Predict     →  Stock-specific LSTM model (lookback: 15–25 days)
5. Invert      →  Scale predictions back to dollar values
6. Display     →  5-day forecast table + % change insight
```

---

## 📊 Supported Stocks

| Ticker | Company | Lookback | Features |
|--------|---------|----------|---------|
| AAPL | Apple | 21 days | close, GK-vol, dollar_vol, OBV, MA3 |
| AMZN | Amazon | 15 days | close, volume, dollar_vol, OBV, EMA |
| GOOG | Google | 21 days | close, volume, dollar_vol, OBV, MA3, MACD |
| INTC | Intel | 25 days | close, GK-vol, dollar_vol, OBV, MA3 |
| META | Meta | 20 days | close, volume, dollar_vol, OBV, EMA |
| MSFT | Microsoft | 20 days | close, volume, GK-vol, dollar_vol, OBV, MA3 |
| TSLA | Tesla | 15 days | close, dollar_vol, OBV, EMA, MA3 |

---

## 📄 License

MIT © [NEDESH KUMAR M](https://github.com/NEDESH-KUMAR-M)

---
## 🙋‍♂️ Built By

**Nedesh Kumar M**

[![GitHub](https://img.shields.io/badge/GitHub-NEDESH--KUMAR--M-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/NEDESH-KUMAR-M)

---

## ⭐ Support

If you found this project useful or interesting, consider leaving a **star** — it keeps the momentum going!

[![Star this repo](https://img.shields.io/github/stars/NEDESH-KUMAR-M/Intelligent-Stock-Forecasting-System?style=social)](https://github.com/NEDESH-KUMAR-M/Intelligent-Stock-Forecasting-System/stargazers)

---

<div align="center">
Made with ❤️ using Python · TensorFlow · Streamlit
</div>
