# Credit-Card-Fraud-Detection

The problem statement chosen for this project is to predict fraudulent credit card transactions with the help of machine learning models.

 

In this project, you will analyse customer-level data that has been collected and analysed during a research collaboration of Worldline and the Machine Learning Group. 

 

The data set is taken from the Kaggle website and has a total of 2,84,807 transactions; out of these, 492 are fraudulent. Since the data set is highly imbalanced, it needs to be handled before model building.

 

Business problem overview
For many banks, retaining high profitable customers is the number one business goal. Banking fraud, however, poses a significant threat to this goal for different banks. In terms of substantial financial losses, trust and credibility, this is a concerning issue to both banks and customers alike.


It has been estimated by Nilson Report that by 2020, banking frauds would account for $30 billion worldwide. With the rise in digital payment channels, the number of fraudulent transactions is also increasing in new and different ways. 

 

In the banking industry, credit card fraud detection using machine learning is not only a trend but a necessity for them to put proactive monitoring and fraud prevention mechanisms in place. Machine learning is helping these institutions to reduce time-consuming manual reviews, costly chargebacks and fees as well as denials of legitimate transactions.

 

Understanding and defining fraud
Credit card fraud is any dishonest act or behaviour to obtain information without proper authorisation from the account holder for financial gain. Among different ways of committing frauds, skimming is the most common one, which is a way of duplicating information that is located on the magnetic strip of the card. Apart from this, the other ways are as follows:

Manipulation/alteration of genuine cards
Creation of counterfeit cards
Stealing/loss of credit cards
Fraudulent telemarketing
 

Data dictionary
The data set can be downloaded using this link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

 

The data set includes credit card transactions made by European cardholders over a period of two days in September 2013. Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced, with the positive class (frauds) accounting for 0.172% of the total transactions. The data set has also been modified with principal component analysis (PCA) to maintain confidentiality. Apart from ‘time’ and ‘amount’, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature 'time' contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value of 1 in cases of fraud and 0 in others.

 

Project pipeline
The project pipeline can be briefly summarised in the following four steps:

* __Data Understanding:__ Here, we need to load the data and understand the features present in it. This would help us choose the features that you will need for your final model.

* __Exploratory data analytics (EDA):__ Normally, in this step, we need to perform univariate and bivariate analyses of the data, followed by feature transformations, if necessary. For the current data set, because Gaussian variables are used, we need not perform Z-scaling. However, you can check whether there is any skewness in the data and try to mitigate it, as it might cause problems during the model building phase.

* __Train/Test split:__ Now, being familiar with the train/test split that you can perform to check the performance of your models with unseen data. Here, for validation, we use the k-fold cross-validation method. You need to choose an appropriate k value so that the minority class is correctly represented in the test folds.

* __Model building / hyperparameter tuning:__ This is the final step at which we can try different models and fine-tune their hyperparameters until we get the desired level of performance on the given data set. We try and check if you get a better model by various sampling techniques.

* __Model evaluation:__ Evaluate the models using appropriate evaluation metrics. Since the data is imbalanced, it is more important to identify the fraudulent transactions accurately than the non-fraudulent ones. Choosing an appropriate evaluation metric that reflects this is business goal.
