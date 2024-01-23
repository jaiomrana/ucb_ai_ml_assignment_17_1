### Assignment for UC Berkeley Professional Certificate in Machine Learning and Artificial Intelligence.

**Overview**

The goal of this assignment is to compare the performance of the classifiers namely **K Nearest Neighbor, Logistic Regression, Decision Trees, and Support Vector Machines**. The dataset is related to marketing bank products over the telephone. The objective is to build a predictive model that could predict if a bank's customer would likely subscribe to long term deposit product or not. It's going to be a binary classification model with target class label of 'yes' or 'no'.

**Data**

Our dataset comes from the UCI Machine Learning repository [link](https://archive.ics.uci.edu/ml/datasets/bank+marketing). The data is from a Portugese banking institution and is a collection of the results of multiple marketing campaigns. We will make use of the article accompanying the dataset [here](references/CRISP-DM-BANK.pdf) for more information on the data and features.

**Deliverables**

After understanding, preparing, and modeling your data, build a Jupyter Notebook that includes a clear statement demonstrating your understanding of the business problem, a correct and concise interpretation of descriptive and inferential statistics, your findings (including actionable insights), and next steps and recommendations.

### Conclusion on Comparing Classifiers

* Tree based models had the best ROC Scores with Decision Tree Classifier at the top with 0.74 and Random Forest Classifier next at 0.72.
* All tuned models had the Training and Test accuracy of at least 90%.
* SVM took the longest to train and fit the model.
* Overall Decision Tree Classifier model performed the best out of all tuned models.


### Recommendations to the Bank Marketing Business

* Call duration ('duration') played the most important role with ~52% which means if customers are engaged longer during the marketing calls then it increases the chance of subscribing to term deposit products.
* Number of employees ('nr.employed') was the next important feature which means customer trust the larger banks more than the smaller banks for the long term deposit products.
* Customer's committment to term deposit product was also found to be dependent on social and economic contextual features like Consumer Price Index (cons.conf.idx), Europe's Short Term Libor Rate ('euribor3m') etc.
* Customer are more likely to subscribe during month of October compared to other months.
* If customers had agreed to subscribe to a term deposit in past then they more likely to subscribe again during next marketing campaign. This is evident due to Previous Outcome ('poutcome') feature importance.


### Next Steps

* Due to personal computer constraints, hyperparameter tuning for all models were limited to return in reasonable amount of time so there's a possibility that models can be further tuned with better parameters.
* Data transformation and cleaning can be revisited to improve training and test data quality.


**The jupyter notebook can be located in this repository here - https://github.com/jaiomrana/ucb_ai_ml_assignment_17_1/blob/main/bank_marketing_campaigns_model.ipynb**
