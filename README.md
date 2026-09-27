This notebook predicts daily sales for Corporacion Favorita (Ecuadorian grocery retailer) stores, using store info, oil prices, holidays, and promotions as extra features.

Approach:

Load all provided datasets (train, test, stores, oil, holidays, transactions)
Merge them into one feature-rich table
Engineer simple date-based and categorical features
Train a fast LightGBM regression model (log-transformed sales, since the competition metric is RMSLE)
Predict on the test set and generate submission.csv with id and sales
