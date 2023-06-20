# Project12

# Credit Risk Classification

This repository contains code and data for the Credit Risk Classification project. The project aims to build a model that can identify the creditworthiness of borrowers using historical lending activity data from a peer-to-peer lending services company. The challenge in this project is dealing with imbalanced classes, as healthy loans significantly outnumber risky loans.

## Instructions

The project consists of the following subsections:

### Split the Data into Training and Testing Sets

1. Read the `lending_data.csv` data from the `Resources` folder into a Pandas DataFrame.

2. Create the labels set (`y`) from the “loan_status” column, and create the features (`X`) DataFrame from the remaining columns.

3. Check the balance of the labels variable (`y`) using the `value_counts` function.

4. Split the data into training and testing datasets using `train_test_split`.

### Create a Logistic Regression Model with the Original Data

1. Fit a logistic regression model using the training data (`X_train` and `y_train`).

2. Save the predictions on the testing data labels using the testing feature data (`X_test`) and the fitted model.

3. Evaluate the model’s performance by calculating the accuracy score, generating a confusion matrix, and printing the classification report.

4. Answer the question: How well does the logistic regression model predict both the `0` (healthy loan) and `1` (high-risk loan) labels?

### Predict a Logistic Regression Model with Resampled Training Data

1. Use the `RandomOverSampler` module from the imbalanced-learn library to resample the data, ensuring an equal number of data points for each label.

2. Use the `LogisticRegression` classifier and the resampled data to fit the model and make predictions.

3. Evaluate the model’s performance by calculating the accuracy score, generating a confusion matrix, and printing the classification report.

4. Answer the question: How well does the logistic regression model, fit with oversampled data, predict both the `0` (healthy loan) and `1` (high-risk loan) labels?

## Dependencies

The following dependencies are required to run the code:

- Python 3.x
- Pandas
- Scikit-learn
- imbalanced-learn

Please make sure to install these dependencies before running the code.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/pceworkflow/credit-risk-classification.git
   ```

2. Navigate to the project directory:

   ```bash
   cd credit-risk-classification
   ```

3. Open the starter code notebook and follow the instructions provided in each section.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to modify and use the code as per the license terms.
