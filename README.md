# Machine Learning for Portfolio Construction (MAT4372)

This project explores how machine learning techniques — specifically **Random Forest regression** — can be applied to portfolio optimization. The analysis focuses on two assets, **Tesla (TSLA)** and **Apple (AAPL)**, with the goal of maximizing the **Sharpe ratio** and identifying the **efficient frontier** between risk and return.

---

## 🧠 Objectives
- Build an efficient two-asset portfolio (TSLA & AAPL)
- Use historical data from Yahoo Finance (via `quantmod` in R)
- Train a **Random Forest model** to predict the Sharpe ratio
- Visualize the **efficient frontier** and highlight optimal portfolios

---

## ⚙️ Tools & Packages
- **R**
  - `quantmod` → to fetch stock prices  
  - `TTR` → to compute weekly returns  
  - `PerformanceAnalytics` → to calculate Sharpe ratio and volatility  
  - `randomForest` → to model and predict Sharpe ratios  
  - `ggplot2` → for visualization  

---

## 📊 Methodology
1. Retrieve historical adjusted closing prices for TSLA and AAPL (2020–present).  
2. Compute weekly returns (Wednesday-only data to reduce noise).  
3. Simulate 5,000 random portfolios with different weight combinations.  
4. Train and test a **Random Forest regression model** to predict Sharpe ratios.  
5. Generate 10,000 new simulated portfolios and estimate their Sharpe ratios.  
6. Plot the **efficient frontier** to visualize optimal trade-offs between risk and return.

---

## 🔍 Key Insights
- Portfolios with higher Tesla weight have greater volatility and higher potential returns.  
- Apple-heavy portfolios are more stable but yield lower returns.  
- The optimal Sharpe ratio is achieved with a slightly higher weight on Apple, balancing stability and growth.  
- The Random Forest model effectively captured non-linear risk–return relationships.

---

## 📈 Results
The efficient frontier was successfully reconstructed using machine learning, producing realistic portfolio configurations that align with modern portfolio theory principles while avoiding restrictive assumptions (e.g., normality of returns).

---

## 🧩 Future Work
- Extend to **multi-asset portfolios** (4+ assets).  
- Compare Random Forest performance with **Neural Networks** or **SVMs**.  
- Incorporate macroeconomic indicators or sentiment data for broader predictive insight.

---

## 🧑‍🎓 Academic Context
This project was completed as part of **MAT4372 — Financial Mathematics (University of Ottawa)**.  
It serves as a practical application of both **machine learning** and **portfolio theory (Markowitz framework)** in modern finance.

---

## 📂 Repository Structure
