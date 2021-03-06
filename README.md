# BlackFriday
This project uses data visualization and a Decision Tree classifier to predict purchasing amount based on consumer and product variables.

## Data Information/Preprocessing: 

BlackFriday.csv was obtained from Kaggle, however many of the product and consumer categories remain undefined. Here is a list of all columns and key attributes to handle in data preprocessing: 


##### Column Names: User_ID, Product_ID, Gender, Age, Occupation, City_Category, Stay_In_Current_City_Years,
Marital_Status, Product_Category_1,Product_Category_2, Product_Category_3,Purchase

#### Things to note: 
1. there are NaN values in Product_Category_2, and Product_Category_3
2. Marital Status: 0 is Male
3. City Category: can be converted to a numerical
4. Age: Are number ranges stored as strings
5. Gender: is recorded as binary
6. Stay_In_Current_City: Handle + symbol
7. Occupation: There are about 16 values
8. There is no definition for what product categories, occupations, or city categories coresspond to

Here is a description of the data: 
![Description of Data](https://github.com/banoop/BlackFriday/blob/master/DataVisualizations/Data%20Breakdown.png)

Furthermore, all visualizations of each target variable distribution and plots of these target variables' relationships to the purchase amount can be found in the data visualizations folder or in the actual program. Important visualizations include the following:
![Product Category 1 vs. Purchase Amount](https://github.com/banoop/BlackFriday/blob/master/DataVisualizations/PC1VP.png)
![Product Category 2 vs. Purchase Amount](https://github.com/banoop/BlackFriday/blob/master/DataVisualizations/PC2VP.png)
![Product Category 3 vs. Purchase Amount](https://github.com/banoop/BlackFriday/blob/master/DataVisualizations/PC3vP.png)

As seen here, it's clear that the type of product category significantly impacts the purchasing amount of a consumer.

Finally, before constructing the model, I had to use a label encoder for all the features that were defined categorically rather than numerically to create numerical representations for these categories. This allowed for the model to handle these values since the model can't read objects.

## Model: 
For this project, I used a Decision Tree Classifier, passing in all the feature's available, and using a training proportion of 0.2. The results of this model versus the actual test values can be seen below: 

![DT Classifier- Predicted vs. Actual Purchase](https://github.com/banoop/BlackFriday/blob/master/DataVisualizations/Predictedvactual.png)




