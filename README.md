# Binance Trade Data Analysis Task 🧮💹

This repository contains the code and report for analyzing Binance account trade data. The objective of this project was to calculate financial metrics such as ROI, PnL, Sharpe Ratio, Win Rate, and more to rank trading accounts. The top 20 accounts are ranked based on their performance metrics.

## 🚀 Project Overview

This project involves analyzing 90 days of trade data from multiple Binance accounts. Key steps include data cleaning, feature engineering, and ranking the accounts based on calculated metrics. The aim was to evaluate and rank accounts using financial metrics.

### 📂 Repository Structure
- **[Report_Details.pdf](Report_Details.pdf)**: A detailed report documenting the methodology, assumptions, and key findings of the analysis.
- **[Trade_Data_Analyst_Task.ipynb](Trade_Data_Analyst_Task.ipynb)**: The Jupyter Notebook containing the complete Python code for data exploration, cleaning, feature engineering, and metric calculation.
- **[final_metrics.csv](final_metrics.csv)**: The CSV file containing all calculated financial metrics for each Binance account.
- **[top_20_accounts.csv](top_20_accounts.csv)**: A CSV file listing the top 20 Binance accounts ranked by performance based on key metrics.

## 📊 Key Metrics Calculated

Here are the important financial metrics calculated for each account:
- **ROI (Return on Investment)**: Measures the return relative to the investment.
- **PnL (Profit and Loss)**: The net profit or loss from trading activity.
- **Sharpe Ratio**: Risk-adjusted return metric.
- **Maximum Drawdown (MDD)**: The largest drop from peak equity.
- **Win Rate**: Percentage of profitable trades.
- **Win Positions**: Number of profitable trades.
- **Total Positions**: Total number of trades executed.

## 🛠️ Project Steps

### 1. **Data Exploration and Cleaning**
   - Loading and inspecting the dataset.
   - Handling missing values and anomalies.
   - Parsing and converting complex trade history data.

### 2. **Feature Engineering**
   - Identifying and extracting relevant features (e.g., `side`, `positionSide`).
   - Calculating metrics like ROI, PnL, Sharpe Ratio, MDD, Win Rate.
   - Creating new features such as position identification (e.g., long/short).

### 3. **Ranking Algorithm**
   - Creating a weighted scoring system for ranking accounts.
   - Ranking accounts based on their performance using calculated metrics.
   - Outputting the **Top 20 Accounts** based on the final score.

### 4. **Documentation**
   - Detailed report covering methodology, assumptions, and key findings (found in [Report_Details.pdf](Report_Details.pdf)).

## 📈 Top 20 Accounts

The top 20 Binance accounts based on the ranking algorithm can be found in the **[top_20_accounts.csv](top_20_accounts.csv)** file.

### 🔑 Key Insights from the Analysis:
- Accounts with consistent win rates and balanced risk-to-reward ratios perform better in the long run.
- The Sharpe Ratio proved to be a significant metric for ranking accounts as it adjusts returns based on risk.
- Accounts with lower maximum drawdowns tended to rank higher in overall performance.

## 📜 Methodology and Assumptions

1. **Data Cleaning**: Handled missing values and ensured correct data types for processing.
2. **Risk-Free Rate**: Assumed a risk-free rate of 0% for calculating the Sharpe Ratio.
3. **Position Identification**: Combined `side` and `positionSide` fields to categorize trades (e.g., long_open, long_close).

More detailed assumptions and methodology can be found in the **[Report_Details.pdf](Report_Details.pdf)**.

## 📂 Files Included
- **Jupyter Notebook**: [Trade_Data_Analyst_Task.ipynb](Trade_Data_Analyst_Task.ipynb)
- **CSV Files**: 
  - [final_metrics.csv](final_metrics.csv): All calculated metrics.
  - [top_20_accounts.csv](top_20_accounts.csv): Ranked top 20 accounts.
- **Report**: [Report_Details.pdf](Report_Details.pdf)

## 🚀 How to Run the Code

1. Clone this repository:
   ```bash
   git clone https://github.com/VIJAY626404/Primetrade.ai_Task.git
   ```
2. Install the required libraries:
 ``` bash
   pip install pandas numpy matplotlib sklearn
   ```
3. Open the Jupyter Notebook:
 ``` bash
   jupyter notebook Trade_Data_Analyst_Task.ipynb
 ```
4. Run all the cells to reproduce the analysis and metrics calculation

# 👨‍💻 Tech Stack
- *Python:* Data analysis and feature engineering.
- *Pandas:* Data manipulation and analysis.
- *NumPy:* Numerical computations.
- *Matplotlib:* Visualization of account performance.
# 💡 Future Enhancements
- Adding more robust error handling for missing or erroneous trade data.
- Automating the entire process with API-based data fetching for real-time account ranking.
- Extending the analysis to include more advanced performance metrics like Sortino Ratio.

If you have any questions or suggestions, feel free to raise an issue or contact me!

🌟 Don't forget to give this repository a star if you found it useful!

