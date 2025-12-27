# Vanguard ETF Performance Analysis (2020–2025)

## 📊 Project Overview
This project evaluates the historical performance of two Vanguard ETFs—**Large-Cap (VV)** and **Small-Cap (VB)**—to determine which yielded a superior profit margin and risk-adjusted return over a five-year period. The analysis follows the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) methodology to provide an empirical, data-driven framework for inexperienced investors.

## ❓ Research Question
> "Between Vanguard’s Large-Cap ETF (VV) and Small-Cap ETF (VB), which asset class yields a larger profit margin (ROI) and lower volatility over a five-year investment horizon?"

## 🛠️ Technologies Used
* **Language**: Python 3
* **Libraries**: 
    * `Pandas`: Data manipulation and time-series analysis.
    * `Matplotlib` & `Seaborn`: Financial data visualization.
    * `Requests`: API communication with Alpha Vantage.
    * `Time`: Managing API governance and rate limits.

## 📈 Key Findings
Based on the analysis of weekly data from Jan 2020 to Dec 2025:
* **Large-Cap (VV)**: Total ROI of **~115.17%** | Annualized Volatility: **0.198**
* **Small-Cap (VB)**: Total ROI of **~59.24%** | Annualized Volatility: **0.249**
* **Conclusion**: Large-Cap ETFs significantly outperformed Small-Cap ETFs in both total profit and risk-adjusted stability during this specific window, refuting the "Small-Cap Premium" theory for this timeframe.

## 🔌 Data Sourcing
The primary data for this analysis was programmatically retrieved from the **Alpha Vantage API**.

* [12/22/25]**Data Source**: Alpha Vantage (Financial Market Data API) 
* [12/22/25]**Endpoint Used**: `TIME_SERIES_WEEKLY` [cite: 3]
* **Data Granularity**: Weekly closing prices for the 5-year period (2020–2025) [cite: 3]
* **Tickers Analyzed**: 
    * `VV` (Vanguard Large-Cap ETF)
    * `VB` (Vanguard Small-Cap ETF)
* **Extraction Strategy**: To ensure compliance with the API’s free tier (5 calls per minute), a 15-second time delay (`time.sleep`) was implemented between requests to guarantee data integrity and ethical usage.

## 🚀 How to Use
1. **Clone the Repository**
2. **Obtain API Key from Alpha Vantage**
3. **Run the Notebook: Open the Jupyter Notebook and replace the API_KEY placeholder with your own key.

## Legal Disclaimer
This project is for educational purposes only as part of a Data Analytics Capstone. The findings do not constitute professional financial advice. Past performance is not indicative of future results
