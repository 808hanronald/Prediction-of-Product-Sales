# Uncovering properties of product and outlets to increase sales output
---
### Analyizing popular products and outlets to increase sales
Author: Ronald Han
---
#### Knowing what products to order for a small outlet let alone a large supermarket can be a daunting task, but is crucial for the success of the business.  Understanding why certain products sell well at a particular store can not only stream line your ordering process but also help make infromed decision to guide the way to a higher profit. 

### Data Source:
---
https://drive.google.com/file/d/1oA8uMVhONvSH30dmeNfFDewMQSI51DO_/view?usp=drive_link

### Data Dictionary:
---
**Item_Fat_Content:**  *Whether the product is low-fat or regular*

**Item_Visibility:**  *The percentage of total display area of all products in a store allocated to the particular product*

**Item_Type:**  *The category to which the product belongs*

**Item_MRP:**  *Maximum Retail Price (list price) of the product*

**Outlet_Identifier:**  	*Store ID*

**Outlet_Establishment_Year:**  *The year in which store was established*

**Outlet_Size:**  *The size of the store in terms of ground area covered*

**Outlet_Location_Type:**  *The type of area in which the store is locate*

**Outlet_Type:**  *Whether the outlet is a grocery store or some sort of supermarket*

**Item_Outlet_Sales:**  *Sales of the product in the particular store. This is the target variable to be predicted.*

## The data has been cleaned and processed to view the relationship it has with output sales.  

##### Exploring the Data
---
  - Barplots for items we sell
  - Scatter plots for numerical features correlation's to sales

![item](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/95dc87c6-dfb1-44b2-8fba-1c61d9fe1ad7)
  - Count for item we sell

![msrp](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/d50902fd-057b-4dc3-a03c-a0ef8091cfbb)
  - Numeric Scatter plot to view the relationship's postive correlation between item MSRP and sales

##### Explaing the Data
---
![outlet_identifer](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/1679027d-ff2e-4ba9-a105-ef03fb64192b)
  - This barplot with a stipplot added for clarity show outlet 27 has the highest out put sales
  - Outlet 10 and 19 have the lowest

![outlet type](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/080bd1b4-4442-4e6c-8533-4a6444b595db)
  - Supermarket Type 3 has the higest sales
  - Grocery Stores have the lowest sales




#### ML models used:
 ---
  - Random Forest Regressor
  - Tuned Random Forese Regressor
  - Linear Regression

#### Model Evaluated and Results
---
![importances](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/974eaa9f-2e57-4173-a54b-3d6744d8db0a)
  - What feature were important in our Random Tree model
  - Item_MRP had profound effect on our target

![top 15 coeffs](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/23c885c6-f29d-4f6e-b0e2-eab2d95cd755)
  - What features were important in our Linear Regressor
  - Outlet 27 and supermarket type 3 were equally importent
  - Size and items sold seem to be factors 
--- 
  - Random Forest Regressor Test
    - MAE = 815.029
    - MSE = 1,349,902.7
    - RMSE = 1,161.853
    - R^2 = .562

  - Tuned Random Forest Regressor Test
    - MAE = 789.85
    - MSE = 1,257.251.652
    - RMSE = 1.121.272
    - R^2 = .592

  - Linear Regressor
    - MAE = 859.968
    - MSE = 1,355,840.595
    - RMSE = 1,164,406
    - R^2 = .560
---
  - The final model chose was the Random Forest Regressor Model with
    - max_dept: 5
    - max_features: None
    - n_estimators: 947
  - R^2 was test was 56.2% and train was 61.3%
  - Mean Absolute Error was off by $815.02
  - Mean Squared Error was $1,349,902.7
  - Root Mean Squared Error was $1.161.85
This was the best fitting model.  It a low bias but the higest variance. 

## Recommendations
---
  - We have shown what properties help item outlet sales, item MRP and outlet type seem to have the most say in what drives sales.
  - Larger supermarket type outlets with more complete inventory (food and household) rather than smaller grocery store limipted to food have higher sales.

### Limitations and Next steps
---
More data is needed to make better decision on output sales.  Where and what type of outlet would be the next interesting question to look at

#### For Further Information
---
For any additional questions, please contact:
  - Ronald Han (Data Analyst)
  - 312superK@gmail.com

##### Releases
 No releases published

##### Packages 
No packages published






