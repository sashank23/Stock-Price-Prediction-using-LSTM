# 📈 Stock Price Prediction Using LSTM

## 🚀 Project Overview
This project leverages **Long Short-Term Memory (LSTM)** neural networks to predict stock prices based on historical market data. By analyzing past trends, we aim to forecast future closing prices with enhanced accuracy.

---
## 📊 Dataset Details
The dataset used is **'stock_price_data_of_last_5_year.csv'**, containing:
✅ **Date** - The date of the stock entry.
✅ **Open** - Opening price of the stock.
✅ **Close** - Closing price of the stock.
✅ **Volume** - The trading volume.
✅ **Name** - Stock ticker symbol.

---
## 🔄 Workflow

### 1️⃣ Data Loading & Preprocessing
- Import the dataset using `pandas`.
- Convert `date` to datetime format.
- Filter stock data for a specific company (e.g., **'INFO'**).

### 2️⃣ Data Visualization 📉
- Plot **Date vs Open/Close Prices** for trends.
- Plot **Date vs Volume** to assess trading activity.

### 3️⃣ Data Preparation 🏗️
- Extract `close` price data.
- Normalize the dataset using `MinMaxScaler`.
- Create **time-series sequences** using a **60-day** window.

### 4️⃣ Model Implementation 🤖
- **LSTM-based Neural Network** using TensorFlow/Keras.
- Model Architecture:
  - 🔹 **LSTM Layer 1** (64 units, return sequences enabled)
  - 🔹 **LSTM Layer 2** (64 units)
  - 🔹 **Dense Layer** (32 units)
  - 🔹 **Dropout Layer** (0.5 for regularization)
  - 🔹 **Final Dense Layer** (1 unit) for prediction
- Optimizer: **Adam** 🛠️
- Loss Function: **Mean Squared Error (MSE)** 📏

### 5️⃣ Model Testing & Evaluation 🏁
- Prepare test data sequences.
- Generate predictions with the trained model.
- **Inverse transform** predictions to actual price scale.
- Performance Metrics:
  - 📌 **Mean Squared Error (MSE)**
  - 📌 **Root Mean Squared Error (RMSE)**

### 6️⃣ Results & Visualization 📊
- Compare **Actual vs Predicted** closing prices.
- Graphical representation of training, testing, and predicted values.

---
## 🔧 Dependencies
Ensure you have the following installed:
```bash
pip install pandas matplotlib numpy tensorflow keras seaborn scikit-learn
```

---
## ▶️ How to Run the Project
1. Place the dataset (`stock_price_data_of_last_5_year.csv`) in the project directory.
2. Run the Python script.
3. View visualizations and performance metrics.

---
## 🎯 Results & Observations
✅ The **LSTM model** effectively captures stock price trends.
✅ **RMSE metric** evaluates model performance.
✅ Further improvements can be made using:
   - 🔹 **Hyperparameter tuning**
   - 🔹 **Increased training epochs**
   - 🔹 **Additional stock indicators**

---
## ✍️ Author
[Sashank Garg]

## 📜 License
This project is for **educational purposes only**. Feel free to modify and enhance it! 🚀

