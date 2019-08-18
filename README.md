# churn-prediction-with-comperhensve-cleaning-and-diffrent-ML-models
# Introduction :
Strong competition in the field of telecommunication market has lead to a significant drop in the revenues for some companies. Many operators tend to use a large investment to keep their current customers to maintain a beneficial competition. One of the risks is customer jumping to another competitors which is known as customer loss or churn.this project done with the cooapration of my team: eman, hajer and malak.
# Churn prediction :
In machine learning, churn prediction considered as supervised problem where the dataset has a label for each customer instance whether churn or not. To solve this problem we need a customers historical profile and this dataset obtained from IBM Sample Data Sets for customer retention programs
# ML model used :
scikit-learn in Python:
Random forest, SVM, Logistic regression, Decision tree, Naive Bayesian, KNN, Voting (Random forest, SVM, Decision tree, KNN) and XGboost.
# Data cleaning :
- Data quality : we deal with, Missing values , Irregular Cardinality and Outliers.
- Data processing : we deal with, Measuring Correlation, Normalization, Binnig and Sampling.
# feature selection :
features selection applied in weka using Information Gain (IG) and SubsEval classifier are the algorithms 
# parameter tuning :
we use grid search method: in random forest the best parameters are {'bootstrap': True, 'criterion': 'gini', 'max_depth': 5, 'n_estimators': 1000}. Secondly, in KNN the best parameters are {'algorithm': 'auto', 'n_neighbors': 50}.Thirdly, in decision tree the best parameters are {'criterion': 'gini', 'max_depth': 8}. Fourthly, In SVM the best parameters are {'Kernal': ‘poly’, ‘C’: 10}. Fifthly, after applied grid search with boosting with some parameters it gives less accuracy than default. Finally, we integrate the best parameters in voting algorithm.
# Result :
Model	Accuracy :
- Random forest	0.794
- SVM	0.799
- Logistic regression	0.797
- Decision tree	0.776
- Naive Bayes	0.727
- KNN	0.797
- Voting	0.794
- XGboost	0.802
# interpretation :
One factor behind the success of XGBoost is the algorithmic optimizations, it uses a novel tree learning algorithm . Additionally, SVM gives similar accuracy to XGboost due to its power in dealing with high-dimensional feature space and kernel trick. 
Additional view point, the company may build an expensive retention program such hiring sales reps to contact each possible churner, they may go with logistic regression model which gives a relative high accuracy with 79 %, so the company could deal only with the customers who have high probability to churn since the logistic regression gives a probabilistic interpretation prediction for each customer.
