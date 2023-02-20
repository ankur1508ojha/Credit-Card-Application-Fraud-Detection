Identity fraud, also known as identity theft, is a type of fraud in which a suspect deliberately uses another person's personal identifying information such as name, Social Security number, driver's license or other ID, credit card or bank account information without their permission or knowledge for financial gain or other illegal purposes. This type of fraud usually happens in the financial sector, mainly in the banking industry.


The overall goal of the project is to develop a supervised machine-learning model that can be used to detect and predict fraud in identification applications. It aims to develop an efficient and effective statistical analysis model that can be applied in practice to predict fraud and identify fraudulent identity applications.


This report aims to document the process of creating and completing a supervised machine-learning algorithm that can detect and prevent fraud in real-time.

• Data cleaning: examine the dataset and remove any inaccuracies

• Feature Engineering: generate new and insightful features from the existing data

• Feature selection: select the most relevant features from the dataset.

• Modeling: build and test multiple machine learning models, to determine the most efficient and effective
  model for detecting and predicting fraud in real-time.
  
• Conclusion: Analyze the results of the machine learning models and draw conclusions.


After testing different algorithms to fit the data, such as Logistic Regression, Random Forest, XGBoost, Light GBM, and Neural Network experimented with various hyperparameters combinations for each model & compared their performance based on FDR at a 3% rejection rate.
The LightGBM Classifier with parameters: max_depth=6, n_estimators=1000, num_leaves=10, and learning_rate=0.05, was the best and final model. The FDR scores for this model on training, testing, and OOT data were 53.00%, 52.80%, and 50.07%, respectively. (Taking number of variables =20)


Final model shows that we are not overfitting and getting good performance and we can catch 53.43 % of all the Fraud by rejecting the top 3% of the application.
