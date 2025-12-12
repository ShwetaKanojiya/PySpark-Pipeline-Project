# 📈 Tata Motors Stock Price Analysis using PySpark  

<p align="center">
  <img src="https://miro.medium.com/1*04kNfmxa_YfWtNb4uMvlEg.png" alt="PySpark Stock Analysis" width="780">
</p>

## A Complete End-to-End Big Data Analysis Workflow  

#### This project performs **complete stock market analysis** on **Tata Motors (TATAMOTORS.NS)** using **PySpark**, leveraging big-data processing for cleaning, transforming, and analyzing a **30+ year historical dataset**.

### The analysis includes:
- Data preprocessing  
- Missing value handling  
- Feature engineering  
- Trend & volatility analysis  
- Seasonal insights  
- Correlation study  
- Moving averages & crossover trends  
- Outlier detection  
- Investment suggestions  

This project can serve as a reference for **financial analytics**, **PySpark data engineering**, and **time-series analysis**.

---

## 🚀 Technologies Used  
- PySpark  
- Spark SQL  
- Google Colab  
- Matplotlib / Seaborn  
- Pandas  
- Window Functions / SQL Analytics  

---

## 🔧 Phase 1 — Setup & Data Loading  

**Tasks performed:**
- Installed Java & PySpark  
- Initialized SparkSession  
- Loaded CSV data  
- Removed corrupted header rows  
- Renamed columns  
- Converted data types  
- Handled nulls  
- Ensured date ordering & consistency  

### ✔ Key Outputs
- No duplicate rows  
- No missing values in main price columns  
- Clean formatted schema  

---

## 🧹 Phase 2 — Data Cleaning  

### ✔ Forward Fill for Closing Price  
Used `last()` window function for forward filling.

### ✔ Data Type Casting  
Converted:  
- `Close`, `Open`, `High`, `Low` → **float**  
- `Volume` → **int**

### ✔ Daily Return Feature  
Formula:  

### ✔ Moving Averages  
- SMA-50  
- SMA-200  

---

## 📊 Phase 3 — Statistical Analysis  

### Summary Statistics  
- **Min Close:** 100.06  
- **Max Close:** 999.5  
- **Average Close:** 194.82  
- **Volatility (Std Dev):** 203.50  

### Daily Return Insights  
- **Avg Daily Return:** 0.082%  
- **Std Dev:** 2.88%  
- **Highest Return:** +67.24%  
- **Lowest Return:** –40.51%  

---

## 📈 Phase 4 — Trend, Volume & Seasonal Analysis  

### ✔ Moving Average Trend  
SMA-50 vs SMA-200 used to detect:
- Bullish crossovers  
- Bearish crossovers  

### ✔ Volume Analysis  
Highlighted highest trading-volume days.

### ✔ Seasonal Patterns  
Average close price by month:

| Month | Avg Close |
|------|-----------|
| Highest | September (~200.81) |
| Lowest | December (~187.59) |

### ✔ Volatility Windows  
30-day rolling volatility using Spark window functions.

### ✔ Correlation Matrix  
- **High correlation** among OHLC values (>0.99)  
- **Low correlation** between Price & Volume (~0.06)  

---

## 🚨 Phase 5 — Outlier Detection  

Identified extreme events where:  

These outliers correspond to:
- Market crashes  
- Major news  
- Corporate announcements  
- Economic shocks  

---

## 🧠 Phase 6 — Final Insights & Recommendations  

###  Long-Term Investors  
- Buy when **SMA-50 > SMA-200**  
- Hold during high volatility  
- Accumulate during **December dips**  

###  Short-Term Traders  
Use for swing trades:
- Volatility spikes  
- Positive returns  
- Volume breakouts  
- Closing price above moving averages  

###  Portfolio Strategy  
- Best exit zone: **September–October**  
- Best accumulation zone: **December**  
- Monitor EV-market trends  

---

## 📉 Visualizations Included  
- Missing value heatmap  
- Missing value bar charts  
- Volatility over time  
- Monthly trends  
- Outlier days  
- Trend classification (Uptrend / Downtrend)  

---

##  Conclusion  
This project demonstrates a **complete big-data workflow** for stock market analysis using PySpark.  
It reveals **strong financial insights**, uncovers patterns hidden in **30 years of Tata Motors stock prices**, and builds a solid foundation for **future predictive analytics**.

---
