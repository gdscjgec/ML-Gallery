# Regression Model:

## Notebook :
  [Notebook link](https://www.kaggle.com/somya25/medical-cost-prediction)
  
## Dataset : 
  [Dataset link](https://www.kaggle.com/mirichoi0218/insurance) Dataset by Miri Choi
  
## EDA :
   Used histrograms, scatterplot to view the data distribution and on the other hand, used correlation matrix and pairplot to visualise how 
   the features are related to each other and how much they contribute to the result.
  
## Models :

   During EDA, we noticed that the charges were skewed a lot, and to reduce that, we applied log transformation.
   Secondly, we applied various models on the datasetlike **Linear Regression, Ridge regression, Random Forest Regression,
   Gradient Boosting Regression, Extra Trees Regression** and noticed that Gradient Boosting regressor
   suits the most on our dataset as the mean absolute error given by it came out to be minimum (0.245)

## Results :

|Sl.No. |        Model               | Mean Absolute error |
|-----	|----------------------------|---------------------|
|   0	  |     Linear Regression      |  0.3845  	         |  
|   1	  |     Ridge Regression       |  0.3840 	           |  
|   2	  |Random Forest Regression    |  0.2814         	   |  
|   3   |Gradient Boosting Regression|  0.2452             |
|   4   | Extra Trees Regression     |  0.2705             |

#### The table shows that Gradient Boosting gives us the best result.
