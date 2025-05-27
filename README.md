# Breast Cancer Classification with Decision Tree and Random Forest

 This project focuses on classifying tumors as benign or malignant using machine learning techniques applied to the Wisconsin Breast Cancer Dataset. The primary goal is to compare the performance of two popular classification algorithms: Decision Tree and Random Forest.

Dataset Description

The dataset contains 10 continuous numerical attributes describing characteristics of cell nuclei present in breast cancer biopsies, along with a target class attribute named diagnosis. This attribute indicates whether the tumor is benign (non-cancerous) or malignant (cancerous). The dataset also includes an ID column, which is not relevant to modeling and is dropped during preprocessing.

Project Workflow

1. Data Loading and Inspection
   
    The dataset is loaded and the first few records are examined to understand its structure. Data types of each column and statistical summaries (mean, standard deviation,      etc.) are reviewed. The distribution of the target variable diagnosis is also checked to understand class balance.

2. Data Preprocessing
   
    The ID column is dropped as it does not contribute to prediction.
   
    Features and the target variable are separated.
   
    Feature values are standardized using z-score normalization to ensure that all features contribute equally to model training.

3. Splitting Data

    The dataset is split into training and testing sets in a 70:30 ratio. This allows the models to be trained on a majority of the data while reserving a portion for            unbiased evaluation.

4. Model Building

    Two classification models are used:

      Decision Tree Classifier

      Random Forest Classifier

    These models are trained on the training data using the same random seed for reproducibility.

5. Model Evaluation

    Both models are evaluated on the test set using accuracy as the performance metric. Accuracy indicates the proportion of correct predictions out of total predictions.

6. Results

    Decision Tree achieved an accuracy of approximately 91.2%.

    Random Forest achieved a much higher accuracy of approximately 98.8%.

7. Performance Comparison

    A boxplot is used to visually compare the accuracy of the two models. It clearly shows the superior performance of the Random Forest classifier.

Conclusion

The Random Forest algorithm significantly outperformed the Decision Tree in this classification task. This improvement is largely due to the ensemble nature of Random Forests, which reduces overfitting and improves generalization. Standardizing features and using robust evaluation methods further contributed to reliable model comparison.

Notes

Proper feature scaling and data preparation are crucial for good model performance.

Random Forest provides better accuracy and robustness in this medical classification task.

Future work could include hyperparameter tuning and exploring other models like SVM or Gradient Boosting.

