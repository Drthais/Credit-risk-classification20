Credit Risk Analysis Report (README.md)

Credit Risk Analysis Report

Overview of the Analysis

This report analyzes the performance of machine learning models in predicting credit risk, specifically the likelihood of loan default. The goal is to evaluate the effectiveness of Logistic Regression and Random Forest classifiers in identifying high-risk loan applicants using a dataset containing various financial features. The models' performance is assessed using metrics such as accuracy, precision, recall, and AUC (Area Under the ROC Curve).

Results

 Logistic Regression

* **Accuracy:** 99% (both training and testing sets)
* **Precision (Class 1 - High Risk):** 85% (training), 88% (testing)
* **Recall (Class 1 - High Risk):** 93% (training), 94% (testing)
* **AUC:** 0.994 (training), 0.997 (testing)
* **Confusion Matrix (Test):**
    ```
    [[18675    84]
     [   37   588]]
    ```

 Random Forest Classifier

* **Accuracy:** 100% (training), 99% (testing)
* **Precision (Class 1 - High Risk):** 93% (training), 88% (testing)
* **Recall (Class 1 - High Risk):** 98% (training), 90% (testing)
* **AUC:** 0.999 (training), 0.997 (testing)
* **Confusion Matrix (Test):**
    ```
    [[18683    76]
     [   63   562]]
    ```

Summary

Both the Logistic Regression and Random Forest models demonstrate excellent performance in predicting loan status. The high accuracy and AUC scores indicate that the models are highly effective at distinguishing between low-risk and high-risk loans.

 Logistic Regression:

* Shows a good balance between precision and recall, indicating a reliable model for identifying high-risk loans.
* The model's performance is consistent between the training and testing sets, suggesting minimal overfitting.
* The model shows 37 false negatives in the test set.

 Random Forest Classifier:

* Achieves near-perfect accuracy on the training data, but slightly lower recall on the test data.
* The model also shows high AUC scores.
* The model shows 63 false negatives in the test set.
* The Random Forest model had a slightly higher false negative rate than the Logistic Regression, and also showed signs of overfitting to the training data.

Recommendation:

Given the critical nature of minimizing false negatives in credit risk assessment (i.e., failing to identify high-risk loans), the **Logistic Regression model is recommended** for use by the company. Although the Random Forest model had extremely high accuracy on the training data, the slightly lower number of false negatives in the test set of the Logistic Regression model, and reduced signs of overfitting, make it the safer choice. The model's high AUC and balanced precision and recall demonstrate its ability to effectively identify potential loan defaults while maintaining a low rate of misclassification. The Logistic regression model is also simpler and easier to interpret, which can be useful in a credit risk context.