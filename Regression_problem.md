# Regression Problem: Predict Monthly Store Sales

## 1. Context
In the competitive retail landscape, accurate sales forecasting is critical for operational efficiency. Retailers need to anticipate sales variability across different store locations and formats to optimize inventory planning, staffing levels, and marketing strategies. By understanding which factors drive sales—whether it's the store's size, its location type, competitive density, or specific promotional activities—businesses can make data-driven decisions to maximize profitability.

## 2. Problem Statement
The business wants to understand **what drives monthly sales** and needs a model to **predict total monthly sales** for any given store.

You have been given access to the raw data ecosystem (Transactions, Stores, Promotions). Your task is to mine this data, extract relevant features, and build a predictive model.


## 3. Input Data
You are provided with the following raw CSV files in the `raw_data/` directory:

1.  **`TRANSACTIONS.csv`**: Transaction-level sales data.
2.  **`STORES.csv`**: Metadata for each store (Size, City, Format, etc.).
3.  **`PROMOTIONS.csv`**: Master list of promotion types.
4.  **`STORE_PROMOTIONS.csv`**: Mapping of active promotions per store with start/end dates.
5.  **`CALENDAR.csv`** (Optional): Date reference.

## 4. Expectations
The business is interested in the following:

1.  **Data Processing**: Convert the raw, scattered data into a clean, usable format for modeling.
2.  **Key Drivers**: Which factors matter most? Is it the store size? specific promotions? locations? or **seasonality/year-over-year trends**?
3.  **Prediction Accuracy**: How close can your model get to the actual monthly sales numbers? (Metric: RMSE).

*Note: Since you have data spanning multiple years, your evaluation strategy should account for the **time-series nature** of the data (e.g., using a time-based split instead of a random shuffle).*
