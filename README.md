# **PROJECTED FOOD SALES FOR Q4 USING PREDICTIVE MODELS**
## Predicting sales in dollars of outlet store food items.
Author:  Rashad N. Campbell

### Business problem:
We need to predict individual item food sales each month to properly manage fixed food storage for each store outlet type.

### DATA:
Individual items are represented by these attributes:
 1)   Item_Identifier
 2)   Item_Weight
 3)   Item_Fat_Content
 4)   Item_Visibility
 5)   Item_Type
 6)   Item_MRP
 7)   Outlet_Identifier
 8)   Outlet_Establishment_Year 
 9)   Outlet_Size
 10)   Outlet_Location_Type
 11)  Outlet_Type 
 12)  Item_Outlet_Sales 

Some attributes may be removed from the model because of their low or non-relevance to the prediction of the total sales of individual items.

### Methods
*  The Item_Identifier attribute was removed from the dataset because it has no relevance towards sales prediction.
*  Outlet_Size value range was changed from Small, Medium, High, to Small, Medium, Large.

### Results
![image](https://user-images.githubusercontent.com/123280849/225897471-df06e5c5-e546-4040-9808-04ddb48cd520.png)
The above represents the footprint of all Outlets by their type.

### Model
Two models used for prediction (Elastic Net Linear Regression and Decision Tree).  From their individual results of tuned parameters (below), the Elastic Net model has a higher percentage R2 (preferred) on the test data, as well as a lower RMSE (preferred) on the test data. As of now both models are producing lower than ideal results.

### Limitations & Next Steps
It's recommended that the metric Mean Absolute Error (MAE) be used to make a better assessment of the model perfomance because of the very large varience in target training data (Item_Outlet_Sales).  MAE will give a better understanding of predictive error for the entire range of sales predictions in the dataset by directly representing predictive error (plus or minus) in the units of our selected target we are attempting to predict.  In this case our target unit of measure is dollars.

### For further information:
For any additional questions, please contact the author at **chicagovt@gmail.com**
