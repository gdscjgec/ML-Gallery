# Classification : [Supervised Learning] 

## Notebook :
  
  [Notebook link](https://www.kaggle.com/tishajhabak/wine-quality-testing?scriptVersionId=76296125)

## Dataset : 
  
  [Portugal Wine Data](https://www.kaggle.com/mpwolke/cusersmarildownloadswinecsv?select=wine.csv)  dataset by Marília Prata

## EDA :

  Boxplots and scatterplots used to visualise the data !! Boxplots show us the spread of the data and also shows us the outliers present in each feature of the dataset. 
The scatterplot gives us the idea of the distribution of particular feature with respect to another. The correlation heatmap helps us select the best features to be used in the training. It gives us the dependencies of each feature on other.

## Models :

  We have normalised the data because there were many outliers according to the EDA , we have used PCA for best feature selection and also categorised the dependent variable to three classes as **"low"** , **"medium"** and **"high"**.
Then we have used five different classification algorithms and compared each of their results to select the best model and also the best hyperparameter through hyperparameter tuning.
The different algorithms are :
* **Support Vector Machine**
* **Decision Tree**
* **Random Forest**
* **Naive Bayes**
* **Logistic Regression**
* **AdaBoost**
* **Gradient Boosting**

## Results :

|Sl.No. |        Model        |  Best_Score 	| Best_Params  	                          |
|-----	|---------------------|---------------|-----------------------------------------|
|   0	  |         svm         |  0.948148  	  | {'C': 1, 'kernel': 'rbf'}  	            |  
|   1	  |    decision_tree    |  0.943827 	  | {'criterion': 'gini', 'max_depth': 5}  	|  
|   2	  |    random_forest    |  0.952469   	| {'max_depth': 10, 'n_estimators': 10}  	|  
|   3   |     naive_bayes     |  0.944444     | {}                                      |
|   4   | logistic_regression |  0.948148     | {'C': 1}                                |
|   5   |       AdaBoost      |  0.954938     | {'base_estimator': ExtraTreesClassifier(n_estimators=10, random_state=0),'learning_rate': 0.5,'n_estimators': 5} |
|   6   |  Gradient Boosting  |  0.945062     | {'learning_rate': 0.1, 'max_depth': 5, 'n_estimators': 15} |

### The table given above shows that AdaBoost gives us the best result , so we have used the model to check the cross-validation accuracy.
```
  cross_val_score_by_rf = 94.876969224016
```
```
  cross_val_score_by_ada = 95.4320987654321
```

### The test accuracy for the model :
```
  test_acc_by_rf = 93.33333333333333
```
```
  test_acc_by_ada = 93.58024691358024
```