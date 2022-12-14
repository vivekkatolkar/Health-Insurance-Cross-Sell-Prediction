# Health-Insurance-Cross-Sell-Prediction

analysis for dataset in Health Insurance Cross Sell Prediction
Health-Insurance-Cross-Sell-Prediction
Predict Health Insurance Owners' who will be interested in Vehicle Insurance

# Problem Statement

Your client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the customers from past year will also be interested in Vehicle Insurance provided by the company.

# Business Goal

Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

# Feature Engineering 

* The binary features ‘Gender’ and ‘Vehicle Damage’ are encoded  in the form of 0 and 1 for the response No and Yes respectively.

* One Hot Encoding is performed on the ‘Vehicle_Age’ Feature.

* The columns ‘Vehicle_Age_1-2 Year’ and ‘Vehicle_Age_> 2 Years’  have been merged as follows:
 
x ['Vehicle_Age > 1 Year'] = x ['Vehicle_Age_1-2 Year'] + x ['Vehicle_Age_> 2 Years']

* The multicollinearity from the features is removed by keeping the VIF value as low  as possible.

* The data has been scaled to improve the model performance  using MinMaxScaler.

* Some of the features in our dataset are highly imbalanced,hence to avoid this error, the dataset is balanced using technique called SMOTE(Synthetic Minority Oversampling Technique)


# Machine Learning Models Used 

1. Logistic Regression
 
2. Random Forest Classifier
 
3. XGBoost Classifier
 
4. Naïve-Bayes Classifier


# Hyper-Parameter Tuning metod used:

1. GridSearch CV


# Conclusion

* After loading the dataset, cleaning the data, performing EDA,

* Feature Engineering and after feature selection, Models are built.

* In terms Training and Testing Accuracy and ROC-AUC score, XGBoost Classifier gave  the best results.

* Vehicle_damage and Previously_Insured came out as the most important features for  the model.

* We will choose in this case is XGBoost Machine Learning. This model is able to predict the label of the target customer who is response and not response at an recall model with value 93% and AUC score at 85%.

* This means our model can improve our response rate for predicting customers who interested in subscribing vehicle insurance

