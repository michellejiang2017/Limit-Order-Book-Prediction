# Limit Order Book Price Prediction

This project predicts whether AAPL’s midpoint price will move up, down, or remain approximately flat over the next 20 limit-order-book events.

I engineered features including spread, market depth, order-book imbalance, returns, volatility, execution volume, signed order flow, and depth changes. I compared logistic regression, random forest, and XGBoost using chronological train, validation, and test splits.

Adding order-flow features improved XGBoost macro AUC from about 0.58 to 0.64 on the final test set.

## Results

- Test macro AUC: 0.642
- Test balanced accuracy: 0.465
- Test accuracy: 0.407

## Technologies

Python, pandas, NumPy, Matplotlib, scikit-learn, and XGBoost.

## Limitations

The analysis uses one stock and one trading day and does not model transaction costs, latency, queue position, or realistic fills.

## Running the Project

Open `limit_order_book_prediction.ipynb` in Google Colab or Jupyter Notebook and run the cells from top to bottom.

This project is for educational purposes only and is not a live trading strategy.
