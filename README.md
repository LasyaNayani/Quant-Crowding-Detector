# Quant Crowding Risk Monitor

**Overview**

This project builds a real-time crowding risk monitor for quantitative hedge funds using entirely public data.

Crowding happens when multiple quant funds hold the same stocks at the same time. If one fund is forced to sell, others may follow — creating a cascade of losses. This dynamic played out during the quant crisis of 2007 and again during the summer 2025 factor unwind.

The goal of this project is to detect which stocks are most at risk of a crowding-driven unwind before it happens.

**Data Sources**

1. SEC 13F filings from the U.S. Securities and Exchange Commission (fund holdings data)

2. Daily trading volume (used to compute liquidity and Days ADV)

3. Factor returns from the Kenneth R. French Data Library

4. Research papers from arXiv for the AI knowledge base

**What we Did?**

1. Collected and cleaned SEC 13F filings for major quant funds

2. Pulled daily stock trading volume and calculated Days ADV for liquidity stress

3. Integrated factor performance data to track historical unwind events

4. Built an Isolation Forest model to detect anomalously crowded stocks

5. Developed an interactive Streamlit dashboard with:

*(A). Crowding scores and top-risk stocks*

*(B). Exit difficulty vs fund concentration risk map*

*(C). Factor performance charts with historical stress events*

*(D). AI-powered risk brief and Q&A layer*


**🎥 Watch Dashboard Demo**

Watch the full dashboard demo on Google Drive:  
[Open Dashboard Video](https://drive.google.com/file/d/1wkE6GhY76rq9JoyftyVqjJp4ZUBRHFE8/view?usp=sharing)

**Colab Notebook Reference**

The full workflow and experiments are available in our Google Colab notebook:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1FTZo6eLNtcPwXtZNfJsNYkrH_VDztSan?usp=sharing)




