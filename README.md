Trader Behavior Analysis

This project analyzes how trader behavior changes with market sentiment (Fear–Greed Index) and how it impacts profitability.
It includes data cleaning, merging, visualization, and creation of a final machine-learning–ready dataset.

* Project Structure
csv_files/
    merged_trades.csv
    final_ml_dataset.csv
    top_accounts_sample.csv

outputs/
    profitability_by_sentiment.png
    avg_profit_by_sentiment.png
    buy_ratio_by_sentiment.png
    sentiment_distribution.png
    top15_accounts_avg_profit.png

notebook_1.ipynb
ds_report.pdf
ds_report.md
README.md

* What This Project Does
Loads historical trading data
Loads Fear–Greed sentiment data
Cleans and preprocesses both datasets
Merges them on the basis of timestamps
Creates new features (profit %, sentiment bucket, buy/sell ratios, etc.)
Generates visual insights
Produces an ML-ready dataset

* Visualizations Included
Profitability vs Sentiment
Average Profit by Sentiment
Buy Ratio by Sentiment
Sentiment Distribution in Trades
Top 15 Accounts by Average Profit
All images are saved in the outputs/ folder.

* How to Use
Open notebook_1.ipynb in Google Colab
Update project path
Run cells step-by-step
Processed CSVs and plots are saved automatically

* Tools Used
Python
Pandas
NumPy
Matplotlib / Seaborn
Google Colab
GitHub
