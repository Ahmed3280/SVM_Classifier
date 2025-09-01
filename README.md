# SVM_Classifier
SVM Classifier for Pulsar Star Prediction

This project implements a Support Vector Machine (SVM) classifier to predict pulsar stars. The workflow includes data preprocessing, visualization, hyperparameter tuning using GridSearchCV, model evaluation, and cross-validation.

Key Features:

1 - Hyperparameter Tuning with GridSearchCV

  Used GridSearchCV to explore multiple kernels (linear, rbf, sigmoid) and tune parameters such as C, gamma, and degree (for polynomial kernel).
  
  Increased C to handle outliers and improve robustness.
  
  Best model from GridSearch: SVC(C=10, gamma=0.3, kernel='rbf')
  
  GridSearch CV best score: 0.9793
  
  Test set score: 0.9835

2 -Data Preprocessing and Visualization

  Applied standard preprocessing and explored data distributions.
  
  Plotted ROC curves to evaluate performance beyond accuracy.

3 - Evaluation Metrics

  Accuracy on test set: 0.9835
  
  ROC-AUC used to account for class imbalance.
  
  Confusion matrices examined to understand misclassifications.

4 - Cross-Validation

  Performed 10-fold cross-validation to validate model generalization.
  
  Averaged ROC-AUC ensures robustness across different splits.

Conclusion:

  GridSearchCV helped identify the RBF kernel with C=10 and gamma=0.3 as the best-performing model.
  
  The SVM classifier achieves high accuracy and ROC-AUC while effectively handling outliers.
  
  Cross-validation confirms strong generalization on unseen data.
