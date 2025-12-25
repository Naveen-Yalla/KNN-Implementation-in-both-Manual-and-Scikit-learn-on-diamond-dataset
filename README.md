# KNN Implementation on Diamonds Dataset
This project contains an end‑to‑end implementation of K‑Nearest Neighbors(KNN) for diamond price prediction using the diamonds dataset. This project covers both a from‑scratch KNN implementation and a Scikit‑learn KNN model.
​
## Project Objectives

- Predict the price of a diamond using its physical and categorical attributes.

- Implement the KNN algorithm from scratch (no Scikit‑learn KNN in this part).

- Build a second model using Scikit‑learn’s KNN and compare performance with the manual implementation.
​
## Dataset Contains:​
**Target variable:** price.

**Numerical Features:** carat, depth, table, x, y, z.

**Categorical Features:** cut, color, clarity.
​

## Project Workflow:
The project closely follows the following steps.
1. Load the data
2. Identify input and output variables​

3. Train–test-split 75% as train data 25%  of data is used as test data using train_test_split.
​
4. Preprocess X_train
    - Categorical encoding such as Ordinal Encoding for the features cut, color, clarity.
    - Numerical rescaling such as MinMaxScaler for Numerical Features.
​
5. Preprocess X_test
    - Applied the same encoders and scalers fitted on X_train to X_test.
​
6. Manual KNN implementation and prediction from scratch:
    - Compute distances such as Euclidean between a test point and all training points.
    - Selecting the k nearest neighbors.
    - Predict price as the average of neighbors’s prices(KNN regression).
​
7. Model evaluation for scratch KNN:
    - Evaluated predictions using metrics such as R² score.
​
8. Scikit‑learn KNN model:
    - Built KNeighborsRegressor model from Scikit‑learn using the same preprocessed data.
    - Selected the same no.of k nearest neighbors considered for the KNN Implementation.
    - Evaluated on X_test using the same metrics as the scratch model.

9. Comparing performance metrics between manual and Scikit‑learn implementations:
    - Finally, Compared the performance scores of both manual and Scikit‑learn implementations and got the same score, that is 95% for both implementations.
