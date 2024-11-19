# Predicting-Credit-Card-Eligibility-by-Using-Supervised-Machine-Learning-Techniques
<h3>Applied Machine Learning Assignment</h3>

<p>Dataset source: https://www.kaggle.com/datasets/rohit265/credit-card-eligibility-data-determining-factors/data</p>

Some insights:
1. Logistic Regression
After hyperparameter tuning, there is only minor improvement on accuracy, recall for class 0 and F-score for class 0. The model is still biased toward class 0 (not eligible) as there is no change after tuning for class 1. The class 1 prediction still low although there is some improvement in confusion matrix, this might mainly due to extreme imbalance in class from the dataset even after class balancing.

2. Gradient Boosting Classifier
Overall, the classification report shows the model is good in predicting class 0 but poor performance in class 1. Confusion matrix also indicates that the model is biased towards predicting class 0 as it is having a quite large number in false negative part.

3. Ada Boost Classifier
Although the accuracy improved after hyperparameter tuning, but the accuracy is mainly improved due to improved in predicting class 0. The model is biases towards class 0 and still struggle to identify class 1.

4. Summary
All the selected models perform well in identifying majority class 0 but perform poorly in identifying minority class 1. Gradient Boosting Classifier is the best model in predicting majority class amongst the 3 models selected, following by Ada Boost Classifier and Logistic Regression. However, Logistic Regression is slightly better in identifying minority class compared to GBC and Ada Boost Classifier.  

5. Suggestions for further improvement
-use different over-sampling methods such as SMOTENC and ADASYN for class balancing purposes
-use other machine learning models such as SVM and K-Nearest Neighbors
-change the outlier detection techniques to other technique such as Z-score method
-find another dataset with similar features and a better balance between classes to combine it into this dataset
-add more feature engineering into the dataset as new features might help the model to capture important patterns in the data
