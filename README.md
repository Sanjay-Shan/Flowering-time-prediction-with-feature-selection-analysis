# Flowering-time-prediction-with-feature-selection-analysis

The project was a part of my academic curriculum and involved working towards the variable selection for large dataset namely Maize Flowering time dataset.The motive behind the collection of this dataset was to see the flowering patterns of around 200x25 breeds of the maize plant.

## Dataset Description
There are around 5000 observations and 7393 variables in this dataset, which is what makes it challenging to train a model. 2 of the variables in the dataset namely Entry and Pop define the breedtype of the dataset and the varibles m1-m7393 define the genetic struture of the dataset. DtoA is the target variable and is nothing but the time taken to flower.  

## Design Structure
The main idea was to get the variables that are very well correlated with the target variables and hence a variable selection was given prominence in this project.Here are few of the methods that were tried to accomplish the task:
1. Pearson's Correlation
2. Spearman's Correlation
3. Lasso Regression
4. Ridge Regression
5. Elastic net Regression
6. Linear Regression
7. Random Forest Regression

## Result and Analysis
On training the model using the above methods it was realized that Pearson's correlation with Random Forest Regressor worked the best. On carefully examining the result, it was also found out that the when the top K features were selected from K=20 - K=4000 , the R2 kept increasing , but started decreasing after that point. This gave a sense that there were only 4000 variables that made sense to the prediction variable.
   The best model gave a MSE below 4.0 and a R2 Statistic of 76% which definitely shows the goodness of fit on the dataset.
