# Customer Analytics and Churn Prediction (INFO411)

Team project for INFO411 Data Mining and Knowledge Discovery at UOWD (2026). The analysis is an R notebook on the UCI Online Retail dataset.

## What it covers

- Cleaning: 541,909 raw transactions down to 397,884 after removing missing customer IDs, returns and zero prices (4,338 customers, December 2010 to December 2011).
- Customer features: recency, frequency, total spent, average order value, items per order and product diversity.
- Segmentation: K-means with k = 3 (high-value, occasional and at-risk customers), checked with PCA and hierarchical clustering.
- Churn prediction: decision tree, neural network and random forest. The neural network had the best AUC (0.81), and lowering its decision threshold to 0.35 raised recall from 0.49 to 0.78.
- Revenue forecasting: ARIMA, ETS and seasonal naive models on monthly revenue, compared on a holdout period.

## Files

- `notebook/Project_Submission.ipynb`: the full analysis (R kernel)
- `data/dataset.xlsx`: the Online Retail dataset
- `outputs/`: model and forecast comparisons, cluster profiles and the preprocessing summary
- `dashboard_data/`: CSV files exported for the dashboard

## Running it

Open the notebook in Jupyter with IRkernel installed. The first cells install the R packages it uses.
