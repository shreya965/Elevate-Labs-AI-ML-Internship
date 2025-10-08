# Breast_Cancer_detection_with_SVM

This Jupyter notebook demonstrates the process of detecting breast cancer using Support Vector Machines (SVM). The dataset used in this project is from the UCI Machine Learning Repository
 and contains features related to cell characteristics, including radius, texture, smoothness, compactness, and concavity of breast cancer tumors.

The project follows the steps of data preprocessing, training and evaluating an SVM classifier, and visualizing the decision boundaries of the model. Additionally, hyperparameter tuning and cross-validation are performed to optimize the model's performance.

# Table of Contents

Data Preprocessing

Model Training and Evaluation

Decision Boundary Visualization

Hyperparameter Tuning

Cross-validation

Results


## Data Preprocessing

Loading the Data: The dataset is loaded using Pandas and consists of various features such as radius_mean, texture_mean, area_mean, etc., along with the diagnosis column which indicates whether the tumor is malignant ('M') or benign ('B').

Cleaning the Data:

Missing values are handled by removing columns with all null values.

The diagnosis column is mapped to a binary label (1 for malignant, 0 for benign).

The id and diagnosis columns are dropped as they are not needed for the model.

### Feature Scaling:

The features are scaled using StandardScaler to standardize the input data, ensuring better performance for the SVM model.

### Model Training and Evaluation

The dataset is split into training and testing sets using an 80-20 split, with stratified sampling to maintain the proportion of labels.

Two types of SVM kernels are evaluated:

Linear Kernel: A basic linear classifier.

Radial Basis Function (RBF) Kernel: A non-linear kernel that can handle more complex relationships.

The performance of the models is evaluated using accuracy score.

### Results:

Linear SVM Accuracy: 96.49%

RBF SVM Accuracy: 97.37%

### Decision Boundary Visualization

To visualize how the model is making its predictions, we use Principal Component Analysis (PCA) to reduce the dataset to 2D. The decision boundary is then plotted for both the Linear SVM and RBF SVM.

The Linear SVM decision boundary shows a straight line dividing the classes.

The RBF SVM decision boundary is more complex and curved, which is expected due to the kernel’s ability to handle non-linear relationships.

### Hyperparameter Tuning

Using GridSearchCV, we tune the hyperparameters for both SVM models. The parameters being tuned are:

C (Regularization parameter)

gamma (Kernel coefficient for the RBF kernel)

After running the grid search, the best hyperparameters for each kernel are:

RBF Kernel: C = 1, gamma = 'scale'

Linear Kernel: C = 0.1, gamma = 0.001

The models are retrained with these optimized hyperparameters, and the accuracy is re-evaluated.

Optimized RBF SVM Accuracy: 97.37%

Optimized Linear SVM Accuracy: 98.25%

### Cross-validation

To further evaluate the models, cross-validation is performed on both the optimized RBF and Linear SVM models. The results for each model are as follows:

Cross-validation for RBF SVM: Mean score: 97.58%

Cross-validation for Linear SVM: Mean score: 96.92%

### Results

The final results indicate that the Linear SVM with tuned hyperparameters achieved an accuracy of 98.25%, while the RBF SVM achieved an accuracy of 97.37%.

Both models performed well, with the Linear SVM showing slightly better results after hyperparameter tuning.

### Installation and Requirements

To run this notebook, you need to have the following Python libraries installed:

pandas

scikit-learn

matplotlib

numpy

You can install the required libraries using pip:

pip install pandas scikit-learn matplotlib numpy

### Conclusion

This notebook demonstrates how to use SVM for breast cancer detection, showcasing the power of both linear and non-linear kernels. Through hyperparameter tuning and cross-validation, the model's performance is optimized to achieve high accuracy.


