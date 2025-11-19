# ds_shivangi
Data Science Assignment

# 📘 Web3 Trading – Data Science Assignment  

This project explores the relationship between **market sentiment (Fear vs Greed)** and **Hyperliquid trader behavior**.  
The analysis uses two datasets: historical trades and the Bitcoin Fear & Greed Index.

----

## 📊 Objective

Analyze how trader behavior changes with market sentiment by studying:

- Profitability  
- Win-rate  
- Trade size / volume  
- Risk behavior  
- Response to Fear vs Greed periods

---
## 📂 Datasets

### **1. Hyperliquid Trader Dataset**
Key columns:
- `Account`
- `Coin`
- `Execution Price`
- `Size Tokens`
- `Size USD`
- `Side`
- `Timestamp`
- `Start Position`
- `Direction`
- `Closed PnL`
- `Fee`
- `Trade ID`

### **2. Fear & Greed Index**
- `timestamp`
- `value` (0–100)
- `classification` (Fear / Extreme Fear / Greed / Extreme Greed)
- `date`

Sentiment was simplified into:
- **Fear**  
- **Greed**  
- **Unknown**

---
## 🛠️ Methodology

### ✔ Data Cleaning
- Parsed timestamps into datetime  
- Standardized numeric fields  
- Removed invalid rows  
- Created `date` column to match with sentiment dataset  

### ✔ Feature Engineering
- `profit_flag = 1 if Closed PnL > 0`  
- `trade_value = Size USD`  
- `risk_proxy = trade_value` (proxy since leverage was not provided)  

### ✔ Analysis Performed
- Sentiment-wise PnL comparisons  
- Win-rate distribution  
- Trading volume behavior  
- Account-level profitability  
- Visualizations exported to `/outputs` folder  

---







