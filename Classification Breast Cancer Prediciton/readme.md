# Classification Model:

## Notebook :
  [Notebook link](https://www.kaggle.com/somya25/breast-cancer-prediction)
  
## Dataset : 
  [Dataset link](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data)
  
## EDA :
   Used boxplots and correlation matrix to view the data distribution and to visualise how 
   the features are related to each other and how much they contribute to the result.
  
## Models :

   During EDA, we noticed that there are many correlated features which need to be removed, so we dropped such columns.
   Secondly, we applied various models on the dataset like **KNN Classifier, Decision Tree Classifier, Random Forest Classifier, 
   Stochastic Gradient Descent Classifier, Logistic Regression and AdaBoost Classifier** 
   and noticed that *Logistic regression* works the best on our dataset giving us an accuracy of 98.05%

## Results :

|Sl.No. |        Model               |    Accuracy         |
|-----	|----------------------------|---------------------|
|   0	  |     KNN Classifier         |  0.9708  	         |  
|   1	  |  Decision Tree Classifier  |  0.8932 	           |  
|   2	  |Random Forest Classifier    |  0.9514         	   |  
|   3   |Stochastic GD Classifier    |  0.8932             |
|   4   | Logistic Regression        |  0.9805             |
|   5   | AdaBoost Classifier        |  0.9611             |

#### The table shows that Logistic Regression gives us the best result.****
