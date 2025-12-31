\# Walmart Weekly Sales Forecasting (Time Series Regression)



\## Objective

The objective of this project is to forecast weekly sales for Walmart stores using time-series regression techniques. The model leverages historical sales patterns along with external economic indicators to improve short-term forecasting accuracy.



\## Dataset

The dataset contains historical weekly sales data for Walmart stores.  

Key columns include:



\- Weekly\_Sales (Target variable)

\- Holiday\_Flag

\- Temperature

\- Fuel\_Price

\- CPI

\- Unemployment

\- Store

\- Date



\## Project Workflow

1\. Data loading and preprocessing  

2\. Date parsing and time-based sorting  

3\. Store-level analysis (Store 1)  

4\. Exploratory Data Analysis (EDA)  

5\. Feature engineering:

&nbsp;  - Lag features (1, 2, 4 weeks)

&nbsp;  - Rolling averages (4-week and 8-week)

&nbsp;  - Time features (Year, Month, Week)

6\. Time-ordered train–test split

7\. Model training using Linear Regression

8\. Baseline comparison using naïve lag-1 model



\## Models Evaluated

\- Baseline Linear Regression\*\* using lag and macroeconomic features  

\- Naïve baseline model\*\* using previous week’s sales  

\- Feature-engineered Linear Regression using lag and rolling features  



\## Results

\- Naïve baseline MAPE: ~5.7%  

\- Feature-engineered regression MAPE: ~5.4%  



The feature-engineered regression model achieved the best performance by capturing short-term sales momentum and smoothing volatility.



\## Key Insights

\- Weekly sales exhibit strong temporal dependency.

\- Simple lag-based baselines are strong competitors in time-series forecasting.

\- Rolling averages help stabilize noise and improve prediction accuracy.

\- Time-based validation is critical for realistic evaluation.



\## Tools \& Libraries

\- Python

\- Pandas

\- NumPy

\- Scikit-learn

\- Matplotlib



\## Files in This Repository

\- `walmart\_sales\_forecasting.ipynb` – Main analysis and modeling notebook  

\- `Walmart.csv` – Dataset used for forecasting  

\- `README.md` – Project documentation



