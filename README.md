# 📊 Trader Performance vs Market Sentiment Analysis
 
> Analyzing how Bitcoin market sentiment (Fear vs Greed) impacts trader behavior and profitability using real Hyperliquid trading data.
 
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-1D9E75?style=flat)
 
---
 
## 📌 Objective
 
Understand whether market sentiment **Fear, Neutral, or Greed** has a measurable impact on trader PnL, win rate, and trade size. The goal is to extract actionable strategy insights from real trading data.
 
---
 
## 📂 Dataset
 
| Dataset | Source | Description |
|---|---|---|
| Historical Trader Data | Hyperliquid | Trade-level data with PnL, size, direction |
| Bitcoin Fear & Greed Index | Alternative.me | Daily sentiment score (0–100) |
 
---
 
## ⚙️ Methodology
 
1. **Data Cleaning & Preprocessing** — handled nulls, fixed data types, removed outliers
2. **Timestamp Alignment** — converted Unix timestamps, aligned both datasets on date
3. **Dataset Merging** — joined trader data with daily sentiment scores
4. **Feature Engineering** — derived PnL buckets, win/loss flags, trade size categories
5. **Sentiment Grouping** — classified days as Fear (0–45), Neutral (46–55), Greed (56–100)
6. **EDA** — boxplots, distribution plots, group-level comparisons across sentiment categories
7. **Power BI Dashboard** — interactive visual exploration of all key metrics
---
 
## 📈 Key Insights
 
- 📈 **Greed periods** → higher average PnL and win probability
- 📉 **Fear periods** → higher losses, lower win rate, elevated risk
- 💰 **Large trades** generate significantly higher returns than small trades
- ⚖️ **Neutral markets** → stable but moderate performance
- ⚠️ Losses dominate during Fear sentiment — risk management is critical
---
 
## 🖥️ Power BI Dashboard
 
An interactive dashboard built in Power BI for visual exploration of:
- PnL distribution across Fear / Neutral / Greed
- Win rate comparison by sentiment
- Trade size vs returns analysis
- Daily sentiment trend overlay
> 📁 File: `trader_sentiment_analysis.pbix`
> 🔧 Requires [Power BI Desktop](https://www.microsoft.com/en-us/download/details.aspx?id=58494) to open
 
---
 
## 🚀 Strategy Recommendations
 
| Sentiment | Recommended Action |
|---|---|
| 😨 Fear | Reduce exposure, avoid aggressive positions |
| 😐 Neutral | Trade cautiously with moderate sizing |
| 🤑 Greed | Trade actively with proper risk management |
 
> **Key takeaway:** Focus on high-quality, larger position trades during Greed periods. Sentiment-aware strategies can significantly improve profitability and risk control.
 
---
 
## 🛠️ Tools & Technologies
 
| Category | Tools |
|---|---|
| Language | Python 3.x |
| Data Manipulation | Pandas, NumPy |
| Visualization | Seaborn, Matplotlib |
| BI Dashboard | Power BI Desktop |
| Environment | Jupyter Notebook |
 
---
 
## 📁 Project Structure
 
```
trader_sentiment_analysis/
│
├── trader_sentiment_analysis.ipynb   # Main analysis notebook
├── change_date_format.ipynb          # Date preprocessing utility
├── trader_sentiment_analysis.pbix    # Power BI dashboard
├── compressed_data.csv.gz            # Historical trader data
├── fear_greed_index.csv              # Bitcoin Fear & Greed Index
├── requirements.txt                  # Python dependencies
└── README.md
```
 
---
 
## 🔧 Requirements
 
**Python dependencies:**
```bash
pip install -r requirements.txt
```
 
**Power BI Dashboard:**
Download [Power BI Desktop](https://www.microsoft.com/en-us/download/details.aspx?id=58494) (free) to open the `.pbix` file.
 
---
##screenshot of dasboard
<img width="1138" height="662" alt="Screenshot 2026-05-24 155632" src="https://github.com/user-attachments/assets/4576b082-8bc9-4902-9e31-16b905671e5f" />

 
## 🧠 Conclusion
 
Market sentiment has a **strong and measurable influence** on trader performance and risk behavior. Traders who align their strategy with the prevailing sentiment — scaling up during Greed and pulling back during Fear — show significantly better risk-adjusted returns.
 
---
 
## 👤 Author
 
**Akshay Pal**
 
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/akshaypal912)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/akshaypal912)
 
---
 
*⭐ If you found this project useful, consider giving it a star!*
