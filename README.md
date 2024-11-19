# Predicting-Credit-Card-Eligibility-by-Using-Supervised-Machine-Learning-Techniques
<h3>Applied Machine Learning Assignment</h3>

<p>Dataset source: https://www.kaggle.com/datasets/rohit265/credit-card-eligibility-data-determining-factors/data</p>

<h4>Model Evaluation Insights</h4> 
<h5>1. Logistic Regression</h5> 
<p>After hyperparameter tuning, there is only a minor improvement in accuracy, recall for class 0, and F-score for class 0. The model is still biased toward class 0 (not eligible) as there is no change after tuning for class 1. The class 1 prediction remains low, although there is some improvement in the confusion matrix. This might be mainly due to extreme imbalance in class from the dataset, even after class balancing.</p> 

<h5>2. Gradient Boosting Classifier</h5> 
<p>Overall, the classification report shows the model is good at predicting class 0 but performs poorly for class 1. The confusion matrix also indicates that the model is biased towards predicting class 0 as it has a quite large number of false negatives.</p> 

<h5>3. Ada Boost Classifier</h5> 
<p>Although the accuracy improved after hyperparameter tuning, the accuracy mainly improved due to better predictions for class 0. The model is biased towards class 0 and still struggles to identify class 1.</p> 

<h5>4. Summary</h5> 
<p>All the selected models perform well in identifying the majority class 0 but perform poorly in identifying the minority class 1. The Gradient Boosting Classifier is the best model in predicting the majority class amongst the three models selected, followed by the Ada Boost Classifier and Logistic Regression. However, Logistic Regression is slightly better at identifying the minority class compared to GBC and Ada Boost Classifier.</p> 

<h5>5. Suggestions for Further Improvement</h5> 
<ul> 
  <li>Use different over-sampling methods such as SMOTENC and ADASYN for class balancing purposes.</li> 
  <li>Use other machine learning models such as SVM and K-Nearest Neighbors.</li> 
  <li>Change the outlier detection techniques to other methods such as the Z-score method.</li> 
  <li>Find another dataset with similar features and a better balance between classes to combine it with this dataset.</li> 
  <li>Add more feature engineering to the dataset as new features might help the model capture important patterns in the data.</li>
</ul>
