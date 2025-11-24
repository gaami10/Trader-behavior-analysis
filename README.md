Trader Behavior Analysis
Analyzing trader sentiment, fear–greed behavior, and profitability using data science.

This project explores how sentiment and fear–greed behavior influence trader performance.
Using large-scale trading data and sentiment indices, we merge, clean, analyze, and visualize patterns to understand the relationship between trader decisions and market psychology.

 Project Overview

This repository contains:

Cleaned & merged datasets

Data preprocessing notebook

Visualizations of sentiment-based behavior

Final ML-ready dataset

Report (PDF + Markdown)

Google Colab code workflow

The analysis answers:

> How does sentiment affect profitability?
> Do traders buy more in greed or fear?
> Which accounts consistently profit?
> What does the distribution of sentiment look like across trades?

 Repository Structure
Trader-behavior-analysis/
│
├── csv_files/
│   ├── final_ml_dataset.csv        # Cleaned ML-ready dataset
│   ├── merged_trades.csv           # Merged trades + sentiment
│   └── top_accounts_sample.csv     # Sample of high-performing accounts
│
├── outputs/
│   ├── profitability_by_sentiment.png
│   ├── avg_profit_by_sentiment.png
│   ├── buy_ratio_by_sentiment.png
│   ├── sentiment_distribution.png
│   └── top15_accounts_avg_profit.png
│
├── notebook_1.ipynb               # Complete data cleaning + analysis notebook
├── ds_report.pdf                  # Final detailed analysis report
├── ds_report.md                   # Markdown version of the report
└── README.md                      # Project documentation

 Key Steps in Analysis
 Loading the Data

Historical trading data

Fear–Greed sentiment index

Cleaned, filtered, and merged using timestamps

 Preprocessing

Removed duplicates

Filtered invalid rows

Feature engineering:

Profit percentage

Buy/Sell ratios

Sentiment mapping

Rolling averages

 Merging

Trades were merged with the sentiment index based on datetimes, resulting in a 211k+ row dataset.

 Visualizations

Generated several insightful plots:

 Profitability by sentiment

 Average profit by sentiment

 Buy ratio across sentiment

 Sentiment distribution in trades

 Top 15 accounts by average profit

5️ Final ML Dataset

Prepared a dataset suitable for:

Classification models

Regression models

Behavioral prediction tasks

 Key Insights (Summary)

Greed sentiment correlates with higher volume buys, but not always higher profit.

Fear sentiment often triggers early exits leading to losses.

A small group of accounts consistently outperform the market regardless of sentiment.

Average profits differ significantly across sentiment buckets.

A detailed explanation is provided in the PDF report.

 How to Run the Notebook

Upload files to Google Drive

Open notebook_1.ipynb in Google Colab

Update the paths:

PROJECT_DIR = "/content/drive/MyDrive/datascience/ds_aditya_sawant"


Run all cells

Outputs will be saved automatically in /outputs/

 Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Google Colab

Git + GitHub
