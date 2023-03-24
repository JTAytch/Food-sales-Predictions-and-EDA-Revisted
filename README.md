# Food sales and MRP
## Discovering the relationship between the MRP of a food and how well it sells.

**Author**: J. Tulani Aytch

### Business problem:

Understanding the properties of products and outlets that play crucial roles in increasing sales.


### Data:
[Data (e.g. # obs)](https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/)

A food sales dataset with 12 features and 8500+ instances.


## Methods
- Item weights were removed but Outlet Size could become a relevant datatype with more information. Outlet size could be approximated when more patterns or data is discerned. 

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

More of your own text here

## RegressionTreee Feature Importances

![sample image](https://github.com/JTAytch/Project-1-Revisted/blob/main/RegTree%20Importances.PNG)


### For further information


For any additional questions, please contact **tulan94@gmail.com**
