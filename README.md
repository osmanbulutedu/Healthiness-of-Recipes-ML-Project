# Healthiness-of-Recipes-ML-Project
beta, (will be updated)

OB: 

1. ingredients_v1.ipynb : This code takes the recipes.csv file as input and find out the ingredients usage amount in descending order. It'll output the result as ingredients_v1.csvfile
2. ingredients_v2.ipynb : This code converts all the upper cases to lower case. And also apply "Porter Stemmer" to the data. It'll output the result as ingredients_v2.csvfile
3. ingredients_v3.csv: Both recipes and ingredients are stemmed and converted to lower case. No truncation was applied yet.
4. ingredients_v4.csv: Ingredients which counts less than 25 can be truncated.
Then these ingredients can be found in recipes and deleted from there. (Only ingredients not recipes)
Then recipes which have less than 5 ingredients can be truncated as well.
5.Hot Encoding and Binary Classification (1).ipynb: After adding USDA and FSA score and binary labeling, hot encoding will be applied to recipes.
Then, different ML methods will be applied on the CSR Matrix.
6. multiclass-hot encoding1x.ipynb: Mulitclass classification using hot encoding of ingredients and nutrions. ingredients_v4.csv and recipes-properties.csv are used. 
