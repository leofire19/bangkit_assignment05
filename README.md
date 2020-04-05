# bangkit_assignment05
This is the repository for Bangk!t Assignment 05 - First Machine Learning Project
by : 
1. Aldo Leofiro Irfiansyah
2. Nikita Setyagar
3. Tobias Ivandito Margogo Silalahi.

In this assignment we create Machine Learning Model to predict Dementia. 
The Dataset is available at https://www.kaggle.com/jboysen/mri-and-alzheimers. 
We use scikit-learn and tensorflow for modeling.
## Scikit-Learn
In here we compare several algorithm to find baseline model:
1. Xtreme Gradient Boosting (XGBoost)
2. Naive Bayes
3. Logistic Regression
4. Light Gradient Boosted Machine (LGBM)
5. Random Forest
6. Decision Tree
7. Extra Tree
8. Gradient Boosting

Based on k-fold Cross Validation leaaderboard, XGBoost has the best metrics peformance AUC 0.975610. 
Its performance increase after we try feature selection based on importance and hyperparameter tuning using GridSearchCV. 
(AUC 0.985906). Features = 'CDR','M/F_F','MMSE','SES','Age','ASF','MR Delay','nWBV','EDUC'.

## Tensorflow
Using tensorflow we build a gradient boosted clasifier model.
The model give metrics as follows : 
{'accuracy': 0.96,
 'accuracy_baseline': 0.52,
 'auc': 0.97613966,
 'auc_precision_recall': 0.98089886,
 'average_loss': 0.17375536,
 'global_step': 100,
 'label/mean': 0.48,
 'loss': 0.17375536,
 'precision': 1.0,
 'prediction/mean': 0.44961384,
 'recall': 0.9166667}
 
