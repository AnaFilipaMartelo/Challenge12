# Credit Risk Analysis Report

## Overview of the Analysis

* In this analysis, the purpose was to build and evaluate machine learning models to identify the model with the best overall performance to tackle the classification problem of credit risk.

* The dataset used for the analysis contained historical lending activity from a peer-to-peer lending services company. It contain information such as loan size, interest rate, borrower income, debt to income, number of accounts, derogatory marks, total debt, and loan status. The main goal was to predict the creditworthiness of borrowers, where the target variable was a binary classification of healthy loans (0) and high-risk loans (1).

* The dataset was imbalanced, with a significantly higher number of healthy loans (0) compared to high-risk loans (1). There were 75,036 healthy loans and only 2,500 high-risk loans in the original dataset. This class imbalance presented a challenge as it could lead to biased model predictions.

* To address the imbalanced nature of the data, two versions of the dataset were created for comparison:
    - **Original Dataset**: The first version used the unmodified dataset with its class imbalance.
    - **Resampled Dataset**: The second version involved resampling the data using the RandomOverSampler module from the imbalanced-learn library. This technique artificially increased the number of high-risk loan instances to balance the classes and mitigate the impact of class imbalance.
    
* The machine learning process involved the following stages:

    - **Data Preparation**: The dataset was preprocessed to handle missing values, encode categorical variables, and split into training and testing sets.
    - **Model Training**: Logistic Regression models were trained on both the original and resampled datasets to classify credit risk.
    - **Model Prediction**: After training, the models were used to predict the credit risk labels for the testing set. 
    - **Model Evaluation**: The balanced accuracy score, precision, recall, and F1-score were computed to assess the performance of each model.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  - The balanced accuracy score for Model 1 is 0.95, which indicates how well the model performs on imbalanced data by taking into account both true positive and true negative rates. 
  - The precision is 0.85, which means that when the model predicts a loan as "high-risk," it is correct 85% of the time.
  - The recall is 0.91, which means that the model correctly identifies 91% of the actual "high-risk" loans.


* Machine Learning Model 2:
  * The balanced accuracy score for Model 2 is 0.99, which indicates how well the model performs on imbalanced data by taking into account both true positive and true negative rates.
  * The precision score of 0.84 indicates that there were some false positives (instances where the model predicted high-risk loans incorrectly). 
  - The high recall score of 0.99 means that the model correctly identified a large portion of high-risk loans.

## Summary

Machine Learning Model 2 outperforms Model 1 in terms of balanced accuracy, with a score of 0.99 compared to 0.95. This indicates that Model 2 is better at handling imbalanced data and considering both true positive and true negative rates.

Model 2 also has a higher recall score of 0.99, meaning it correctly identifies a larger portion of the actual "high-risk" loans, compared to Model 1's recall score of 0.91.

However, Model 2 has a lower precision score of 0.84, suggesting that it has more false positives (instances where it predicts loans as "high-risk" incorrectly) compared to Model 1's precision score of 0.85.

Considering the problem of predicting credit risk, both precision and recall are crucial factors to consider. A higher recall is desirable as it ensures that more high-risk loans are correctly identified, reducing potential losses. However, a higher precision is also essential to avoid approving too many loans as "high-risk" falsely, which could lead to lost opportunities.

In this case, it depends on the specific objectives and risk tolerance of the lending company. If the company prioritizes reducing losses due to high-risk loans, Model 2's high recall score might be more appealing. On the other hand, if the company wants to minimize the number of false positives and avoid overly cautious loan rejections, Model 1's balanced performance could be preferred.

Ultimately, the decision on which model to use should be made based on the company's specific risk management strategy and goals. However, based on the analysis and considering that Model 2's precision is not significantly lower than Model 1's precision value (0.84 compared to 0.85), I recommend using Model 2 for the credit risk prediction task.

Model 2 achieves a higher balanced accuracy score (0.99) and a higher recall score (0.99), indicating its better performance in handling imbalanced data and correctly identifying a larger portion of the actual "high-risk" loans. While Model 2 may have slightly more false positives compared to Model 1, its overall performance is more balanced and effective in identifying risky loans.
