
# Cryptocurrency Clustering Analysis

This project applies clustering techniques on a dataset of cryptocurrency market data to explore patterns and group similar cryptocurrencies based on their price change percentages over various timeframes. The notebook uses standard clustering methods such as K-Means and PCA for dimensionality reduction.

## Project Structure

The project follows these main steps:

1. **Data Loading**:
   - The dataset is loaded from a CSV file (`crypto_market_data.csv`), with each cryptocurrency identified by its `coin_id`.
   - The dataset contains features like percentage price changes over timeframes such as 24 hours, 7 days, 30 days, etc.

2. **Data Preprocessing**:
   - The data is normalized using the `StandardScaler` from the scikit-learn library.
   - Features such as price change percentages over various timeframes are scaled to have zero mean and unit variance for optimal clustering performance.

3. **Clustering Analysis**:
   - The K-Means clustering algorithm is applied to the normalized data to group cryptocurrencies into clusters.
   - Principal Component Analysis (PCA) is used to reduce the dimensionality of the data and visualize the clusters in 2D.

4. **Visualization**:
   - Visualizations are generated using `hvplot.pandas` to display the clustered data and provide insights into the grouping of cryptocurrencies.

## Requirements

- Python 3.x
- Google Colab (or Jupyter Notebook for local runs)
- Required Python libraries:
  - `pandas`
  - `sklearn`
  - `hvplot`

## How to Run

1. Clone this repository or download the notebook file.
2. Upload the notebook to Google Colab or run it locally in a Jupyter environment.
3. Ensure the `crypto_market_data.csv` file is available and properly referenced in the notebook.
4. Install the required Python libraries (if necessary).
   ```bash
   pip install pandas scikit-learn hvplot
   ```
5. Follow the steps in the notebook to perform the clustering analysis.

## Dataset

- The dataset used for this analysis contains historical price data and percentage price changes for various cryptocurrencies.
- The dataset is expected to have the following columns:
  - `coin_id`: Identifier for each cryptocurrency.
  - `price_change_percentage_24h`, `price_change_percentage_7d`, etc.: Features representing percentage changes over different time periods.

## Results

- The analysis produces clusters of cryptocurrencies that show similar price change behaviors over time.
- PCA allows for 2D visualization of these clusters, providing insights into the grouping of different cryptocurrencies based on their price trends.

