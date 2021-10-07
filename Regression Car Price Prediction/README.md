# Regression Model:

## Notebook:
  [Notebook_link](https://www.kaggle.com/neerajanandcoder/car-price-prediction?scriptVersionId=76569384)
  
## Dataset:
  [Dataset_link](https://www.kaggle.com/hellbuoy/car-price-prediction)

## Exploratory Data Analysis
  In EDA, used histogram to see the distribution of data and pairplot and correlation matrix to visualize the realtion between differnet features 
  and also the feaature importance.

## Data Preprocessing:
  Histogram of the target variable indicates the skewedness in it, so used log transformation to reduce the skewedness and also the names of car model are misspelled
  so, corrected them and replace the column 'CarName' with 'CarModel'. Features 'citympg' and 'highwaympg' are highly correlated so, deleted the 'citympg' feature to
  improve model performance.
  
## Model:
  Used **Linear Regression, LassoCV, Ridge Regression, XGB Regression, Random Forest Regression** and found that lassoCV outperforms the other model.

## Results:
  
|Sl.No. |        Model               | R2_score            |
|-----	|----------------------------|---------------------|
|   0	  |     Linear Regression      |  0.906225  	       |  
|   1	  |       LassoCV              |  0.924641	         |  
|   2	  |       Ridge  Regression    |  0.916993         	 |  
|   3   |      XGB Regression        |  0.911463           |
|   4   | Random Forest Regression   |  0.921890           |


### LassoCV is the best Model.
