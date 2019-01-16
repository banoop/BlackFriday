# BlackFriday
This project uses data visualization and a Decision Tree classifier to predict purchasing amount based on consumer and product variables.

## Data Information: BlackFriday.csv was obtained from Kaggle, however many of the product and consumer categories remain undefined. Here is a list of all columns and key attributes to handle in data preprocessing: 


Column Names: User_ID, Product_ID, Gender, Age, Occupation, City_Category, Stay_In_Current_City_Years,
Marital_Status, Product_Category_1,Product_Category_2, Product_Category_3,Purchase
Things to note: 
1. there are NaN values in Product_Category_2, and Product_Category_3
2. Marital Status: 0 is Male
3. City Category: can be converted to a numerical
4. Age: Are number ranges stored as strings
5. Gender: is recorded as binary
6. Stay_In_Current_City: Handle + symbol
7. Occupation: There are about 16 values
8. There is no definition for what product categories, occupations, or city categories coresspond to
     
