# AI-Driven Short and Medium-Term Crude Oil & Carbon Black Price Forecasting

## 🔍 Overview
This project is a comprehensive solution designed to predict **short- and medium-term prices** of **Crude Oil** and **Carbon Black**, two of the most volatile and industrially significant commodities. Leveraging the power of **machine learning**, **deep learning**, and **hybrid ensemble models**, the system delivers high-accuracy, real-time price forecasts that aid industries in **cost optimization, procurement planning, and risk mitigation**.

The models are built and trained using both **historical and real-time data** on crude oil and natural gas, which are key inputs for carbon black production. This project is particularly beneficial for sectors like **automotive, plastics, rubber, and coatings**, where raw material price stability is crucial.

---

## 🎯 Objectives
- Accurately forecast **Crude Oil** prices using time series and ML-based models.
- Predict **Carbon Black** prices using upstream commodity forecasts (Crude Oil & Natural Gas).
- Enable **real-time forecasting** adaptability.
- Compare and evaluate model performance using metrics like **RMSE**, **MAPE**, and **R-squared**.
- Support industry-level decision-making through robust predictive analytics.

---

## 🤖 Models Implemented
### Individual Models:
- **SVR (Support Vector Regression)**
- **LSTM (Long Short-Term Memory)**
- **GRU (Gated Recurrent Unit)**
- **XGBoost**

### Hybrid Models:
- **GRU + AdaBoost**
- **GRU + XGBoost**
- **LSTM + AdaBoost**
- **LSTM + XGBoost**

### MultiModal Models (for Carbon Black):
- **SVR + LSTM + GRU + XGBoost + AdaBoost (Averaged Output)**
- **LSTM + GRU Ensemble**

All models are evaluated across **weekly** and **monthly** timeframes.

---

## 📈 Dataset & Features
### Datasets Used:
- **Crude Oil Prices**: Historical and real-time (daily, weekly, monthly)
- **Natural Gas Prices**
- **Carbon Black Prices (N330 Grade)**

### Key Features:
- Technical indicators: **ATR**, **EMA**, **RSI**
- Economic indices: **USD Index**, **S&P 500**, **VIX**
- Inventory data: **Crude oil stock levels**, **WTI Futures Ratios**
- Macroeconomic variables and custom-engineered time-windowed features

---

## ⚙️ Installation Instructions
### 1. Clone the Repository
```bash
git clone https://github.com/parth581/Crude_Oil_and_Carbon_Black_Price_Forecasting.git
cd Crude_Oil_and_Carbon_Black_Price_Forecasting
```

### 2. Create a Virtual Environment *(Recommended)*
#### For Windows:
```bash
python -m venv venv
.\venv\Scripts\activate
```
#### For macOS/Linux:
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run Jupyter Notebooks
Open the desired `.ipynb` file in Jupyter or Colab and run the cells to train, test, and visualize model performance.


---

## 📦 Project Structure
```
├── data/                    # Raw and preprocessed datasets
├── notebooks/              # Jupyter Notebooks for model training and evaluation
├── models/                 # Saved model checkpoints (if any)
├── reports/                # Graphs, charts, and exported results
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
```

---

## 🚀 Future Enhancements
- Integrate **Transformer-based models** (e.g., Informer, Temporal Fusion Transformer)
- Build a **web-based dashboard** for real-time price visualization
- Incorporate **geopolitical news sentiment analysis** as a model feature
- Schedule automated data refresh pipelines using tools like **Airflow** or **Prefect**

---

## 📜 License
This project is for academic use only and intended as part of a mini project for Semester VI (2024–25), University of Mumbai.
