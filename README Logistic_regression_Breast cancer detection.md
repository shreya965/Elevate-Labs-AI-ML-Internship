# Logistic-Regression-Breast-Cancer-model
Logistic Regression Breast Cancer model
This notebook demonstrates how to apply Logistic Regression to the Breast Cancer Wisconsin dataset, with a focus on threshold tuning. Threshold tuning is used to adjust the decision boundary that determines whether an observation is classified as malignant or benign based on the predicted probabilities from the logistic regression model.

## Steps in the Notebook:

### Data Preprocessing:

Scaling of the features using StandardScaler to normalize the data.

Splitting the dataset into training and test sets.

### Model Training:

Logistic Regression is used to model the relationship between the features and the target variable (diagnosis).
Balanced weight class is used to reduce the impact of imbalanced dataset.
Regularization such as Ridege and Lasso are used to evaluate the model  as well to find the feature coefficients .


### Threshold Tuning:

The threshold for classifying an observation as malignant (class 1) or benign (class 0) is adjusted.

The model's performance (Precision, Recall, and F1-score) is evaluated at various threshold values ranging from 0 to 1.

The best threshold is selected based on the F1-score.

### Evaluation Metrics:

Precision, Recall, and F1-Score are calculated for each threshold.

The ROC curve is plotted to visualize the trade-off between the True Positive Rate (Recall) and False Positive Rate at different thresholds.
Best Threshold:

Based on the evaluation, the best threshold was found to be 0.47. This threshold gave the best balance between precision and recall, as measured by the F1-score.
## Conclusion:

This notebook demonstrates how to optimize a Logistic Regression model's performance using threshold tuning. By adjusting the classification threshold, you can balance precision and recall, depending on the problem's needs, such as minimizing false negatives or false positives.
