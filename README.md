# 🚀 Project Title: Trader Performance vs. Market Sentiment Analysis

## 📌 Project Overview
This repository contains a data science assignment for **Primetrade.ai** focused on analyzing the relationship between cryptocurrency market sentiment (Bitcoin Fear & Greed Index) and real-time trader behavior on the **Hyperliquid** exchange.

The goal is to determine if market "fear" or "greed" fundamentally changes how traders execute positions, their risk tolerance (leverage/size), and their ultimate profitability (PnL).

## 📊 Key Datasets
1.  **Bitcoin Market Sentiment**: Daily classification of market mood (Fear, Extreme Fear, Greed, Extreme Greed, Neutral).
2.  **Historical Trader Data**: High-frequency execution data including `Account`, `Closed PnL`, `Size USD`, `Side`, and `Direction`.

## 🛠️ Technical Stack
* **Language**: Python 3.x
* **Environment**: Google Colab / Jupyter Notebook
* **Libraries**: 
    * `Pandas`: For high-performance data manipulation and merging of 200k+ rows.
    * `NumPy`: For complex metric calculations.
    * `Matplotlib` & `Seaborn`: For behavioral trend visualization and statistical plotting.

## 📈 Analysis & Methodology
The project follows a rigorous data pipeline:
1.  **Data Preparation**: Cleaned timestamps, handled duplicates, and performed a normalized inner join on a daily level.
2.  **Feature Engineering**: Created custom metrics including Daily PnL per account, Win Rate, and Long/Short bias ratios.
3.  **Segmentation**: Classified traders into "Frequent vs. Infrequent" and "Consistent Winners vs. Losers" to see how different archetypes react to market stress.

## 💡 Top Insights & Strategies
* **Contrarian Behavior**: Analysis revealed a significantly higher Long/Short ratio during "Fear" days, suggesting Hyperliquid traders are aggressive "dip buyers."
* **Volatility Paradox**: While average PnL is higher during Fear, the standard deviation of returns increases by ~15%, indicating a much higher risk of liquidation.
* **Strategy Proposed**: 
    * *Dynamic Leverage Cap*: Reduce max leverage during Extreme Fear to protect capital.
    * *Greed Incentives*: Increase frequency-based rewards during Greed regimes where win rates are historically more stable.

## 📂 Repository Contents
* `analysis.ipynb`: The complete Python source code and visualizations.
* `data/`: Raw datasets used for the analysis.
* `outputs/`: High-resolution charts showing PnL distribution and behavioral shifts.
* `requirements.txt`: Dependencies required to run the notebook locally.



### How to Run
1. Clone the repo: `git clone https://github.com/your-username/your-repo-name.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the `analysis.ipynb` in Jupyter or upload it to Google Colab.



### Personal Suggestion:
When you upload this to GitHub, make sure to **add a screenshot** of your best chart (like the PnL boxplot) directly into the README. It makes the repository look much more "data-driven" the moment the recruiter opens the page!
