# Food sales for next year.
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
The final Decision Tree model used is tuned to predict sales of food items in each outlet.  R2 and RMSE was calculated and compared between both a Linear Regression model and Decision Tree model where the Decision Tree model was able to produce better predictive results based on its minimal tuning.

Minimal tuning of the Decision Tree produced an R2 score of 60.18% I believe is high enough to invest more time towards increasing its score by further model tuning.  RMSE gives us a resonably low dollar amount of variance of predicting sales that are 1,170.18 dollars over or under of actual real world values of our training data.  The goal is to have the lowest RMSE possible. In this case, RMSE represents a predicted sales. With the tested Decision Tree R2 being at 60.18%, this tells me that my tested RMSE of 1170.18 will be in this range about 60.18% of the time. Meaning there is another 40% chance RMSE will be some value higher. This overall is not a good result. Ideally I would aim to tune models where test data produces the lowest RMSE possible and the highest R2 possible. Where R2 is as close to 1 as possible.

### Limitations & Next Steps
Overall the Decision Tree model looks to have good enough baseline performace to invest more time into further tuning the model to further increase its overall predictive accuracy.  If the Decision Tree model can be brought to an minimal R2 score of 80%, I believe this would be good as a starting baseline target.  An R2 score of 90% would be ideal.

### For further information:
For any additional questions, please contact the author at **chicagovt@gmail.com**
