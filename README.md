# Grocery Item sales Predictions and EDA-Revisted.
## “Best Paper Towel in town or Best Paper Towel Around?”
## Discovering the relationship between various properties of a grocery store item and how well it sells.

**Author**: Joseph Tulani Aytch

### Business problem:

Understanding the properties of products and outlets that play crucial roles in increasing sales. The goal is to find out what features affect the sales numbers of a product the most, whether good or bad, based on the available data. After that, we will look to see if we can make a machine learning model that can accurately determine which features have the biggest impact on sales overall, that way it can predict how an item will fare based on the available data. 


### Data:
[Data (e.g. # obs)](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/)

A food sales dataset with 12 features/properties and 8500+ instances/foods.


## Methods
- Item weights were removed as it seemed irrelevant, but Outlet Size could become a relevant datatype with more information. Outlet size could be approximated when more patterns or data is discerned. 

## Results

#### Item sales by type:

![sample image](https://user-images.githubusercontent.com/112998617/199860669-bde68d87-aea4-4ef6-904a-572ffc84244f.png)

According to the data, Fruits and Vegetables or Snack Foods make up the majority of item types. 

#### How Item MRP affects the sales of an Item:

![sample image](https://user-images.githubusercontent.com/112998617/199860456-47a6bf9a-a953-459d-a56d-009ae66252cb.png)

The data marks an interesting trend, as MRP (Maximum retail price) increases, sales increases as well. Though there are many items and instances of data, this shows that, in general, the overall price of the item does not negatively affect the sale of the item. 

## Model

I recommend the regression tree model as it has the potential to become a fairly accurate model. Further testing and tuning would be needed but it shows promise. 

The r^2 score was much higher than the other models. 

While not a perfect metric, the regression tree model's fairly high r^2 means that it was learning from the data well and making judgments based on the data, rather than just guessing or copying the data exactly. 

## Recommendations:

I would recommend tuning the regression tree model to produce the most accurate results. I would also recommend figuring out the outlet size of more of the markets, as I believe that could help produce further insight. 


## LinearRegression coefficients plot

![sample image](https://raw.githubusercontent.com/JTAytch/Project-1-Revisted/main/LinReg%20Coeffs.PNG)

Outlet Location type seems to have the biggest impact on sales in general.

## RegressionTree Feature Importances

![sample image](https://github.com/JTAytch/Project-1-Revisted/blob/main/RegTree%20Importances.PNG)

### Are they the same features in both? If not, what's different?

The values are the same, but the visibility and supermarket type are flipped.

![sample image](https://raw.githubusercontent.com/JTAytch/Project-1-Revisted/main/SHAp%20summary%20plot%20bar.png)

### The top 3 most important features and how they influence the model's predictions.

Item_MRP - The higher this is, the more likely the model is to give a high sale price.

Outlet_Type - the higher this is, the less likely the model is to give a high sale price.

Supermarket type 3 - type 3 Supermarkets tend to be predicted to have higher sale prices. 

![sample image](https://raw.githubusercontent.com/JTAytch/Project-1-Revisted/main/SHAP%20summary%20plot%20dot.png)

## Local Explanations

### High value target 

![sample image](https://raw.githubusercontent.com/JTAytch/Project-1-Revisted/main/High%20value%20LIME%20plot.PNG)

![sample image](https://raw.githubusercontent.com/JTAytch/Project-1-Revisted/main/High%20value%20force%20plot.PNG)

According to both explainations, the outlet not being a grocery store, being supermarket type 3, and a high MRP influenced the predicted value the most, in a positive manner. 

### Low value target 

![sample image](https://raw.githubusercontent.com/JTAytch/Project-1-Revisted/main/Low%20value%20LIME%20plot.PNG)

![sample image](https://raw.githubusercontent.com/JTAytch/Project-1-Revisted/main/Low%20value%20force%20plot.PNG)

The features for this sample was the same as the previous one, except since the outlet was a grocery store and not a supermarket type 3, those values affected the predicted value negatively. MRP was still positive and still a high influence.

### For further information


For any additional questions, please contact **tulan94@gmail.com**
