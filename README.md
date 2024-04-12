# ml_credit_scoring
 
Predicting Credit Risk with Machine Learning

- Dataset Overview: Analysed a dataset of 1000 bank customers with 20 variables to predict credit risk based on attributes like credit history, employment status, and marital status. The target variable was highly imbalanced, with only 12.2% posing a credit risk.

- Data Cleaning: Removed entries with "X" in the purpose column and split the dataset based on the status of checking accounts into two samples for analysis.

- Data Splitting: Used an 80-10-10 split for training, validation, and testing sets. Due to data scarcity, applied a 90-10 split for training and testing, employing cross-validation for hyperparameter tuning.

- Feature Selection: Conducted Chi-Square tests to identify statistically significant variables for building scorecards. Selected four variables for each subset and handled multicollinearity by dropping one variable from one-hot encoded attributes.

- Model Training: Trained logistic and linear regression models on the training set and evaluated them on the test set. Logistic regression showed a weighted F1 score of 0.72 and linear regression slightly outperformed it.

- Handling Imbalances: Addressed class imbalances in sample 2 by downsampling the majority class, which did not significantly improve the model's performance on the test set.

- Model Evaluation: Compared logistic and linear regression models using ROC curves. The performance was decent for sample 1 but not ideal for sample 2 due to class imbalances.
