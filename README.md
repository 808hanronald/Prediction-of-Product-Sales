# Uncovering properties of product and outlets to increase sales output

### Analyizing popular products and outlets to increase sales
Ronald Han

#### Knowing what products to order for a small outlet let alone a large supermarket can be a daunting task, but is crucial for the success of the business.  Understanding why certain products sell well at a particular store can not only stream line your ordering process but also help make infromed decision to guide the way to a higher profit. 

### Data Source:
https://drive.google.com/file/d/1oA8uMVhONvSH30dmeNfFDewMQSI51DO_/view?usp=drive_link

### Data Dictionary:
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

  - Barplots to view the most infuacal features and higest output sales
  - Scatter plots for numerical features correlation to sales
  - And finally which models give us the best R2 score

![outlet_identifer](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/1679027d-ff2e-4ba9-a105-ef03fb64192b)
  - This barplot with a stipplot added for clarity show outlet 27 has the highest out put sales
  - Outlet 10 and 19 have the lowest

![outlet type](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/080bd1b4-4442-4e6c-8533-4a6444b595db)
  - Supermarket Type 3 has the higest sales
  - Grocery Stores have the lowest sales

![item](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/95dc87c6-dfb1-44b2-8fba-1c61d9fe1ad7)
  - Count for item we sell

![importances](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/974eaa9f-2e57-4173-a54b-3d6744d8db0a)
  - What featurse were important in our Random Tree model
  - Item_MRP had profound effect on our target

![msrp](https://github.com/808hanronald/Prediction-of-Product-Sales/assets/140451609/d50902fd-057b-4dc3-a03c-a0ef8091cfbb)
  - Numeric Scatter plot to view the relationship
  - Postive correlation between item MSRP and sales

## Results    

 





https://colab.research.google.com/drive/1p_SwURwFqPGkEK-9YVAWyBgTjcGeDxiL#scrollTo=tbVExVfPTopp&line=1&uniqifier=1
## Model
Describe your final model
Report the most important metrics
Refer to the metrics to describe how well the model would solve the business problems

## Recommendations
---

### Limitations and Next steps
#### For furthe information










