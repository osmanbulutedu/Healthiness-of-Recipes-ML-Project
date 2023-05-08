# Healthiness-of-Recipes-ML-Project
# Introduction
People frequently turn to the internet for food-related choices. However, popular recipe websites have been found to contain a high number of unhealthy recipes. To address this, researchers have proposed healthy food recommendation systems. Determining recipe healthiness and finding suitable substitutions pose challenges for these recommendation systems. To address this issue, this study aims to develop a machine learning model for determining the healthiness of recipes.

This study is based on a publicly available dataset [RecipeKG](https://github.com/IDIASLab/RecipeKG) of 77, 835 recipes published on the main site of Allrecipes.com between the years 1997 and 2021.


## Quick Overview

The initial step of the research involved acquiring the dataset from a SPARQL endpoint. Subsequently, the necessary information, including recipes, ingredients, and their health scores, was filtered. Different digitization methods, such as One-Hot Encoding, Word2Vec, and FastText, were then applied to process the data. The digitized data underwent binary classification, followed by multiclass classification using various machine learning methods.


### How to use




### Prerequisites
Python 3.8 or above and the following libraries

```
- request, json, BeautifulSoup
- nltk, glob, difflib
- rdflib
```



### Files
```
  Code:
   
      Hot Encoding and Binary Classification (1).ipynb: After adding USDA and FSA score and binary labeling, hot encoding will be applied to recipes.
      Then, different ML methods will be applied on the CSR Matrix.

      Word2Vec-Pyspark.ipynb : 

      ing and recipes v3.zip : 

      ingredients_v1.ipynb:  This code takes the recipes.csv file as input and find out the ingredients usage amount in descending order. It'll output the          result as ingredients_v1.csvfile

      ingredients_v2.ipynb : This code converts all the upper cases to lower case. And also apply "Porter Stemmer" to the data. It'll output the result as ingredients_v2.csvfile

      multiclass-hot encoding1x.ipynb: Mulitclass classification using hot encoding of ingredients and nutrions. ingredients_v4.csv and recipes-properties.csv are used. 

      spark-multiclass-prediction-2-withproperties.ipynb : 

      spark-multiclass-prediction.ipynb :

      Digitization-Examples.ipynb : takes in the recipe-to-ingredient dataset and FDA/USDA labels to perform several methods of digitization to better clarify relations between ingredients. The two types of digitization methods utilized were fasttext and word2vec. These methods were then fed into binary and multinomial logistic regression models. Prerequisites: NLP and Preprocessing should be applied first to derive the ingredients_v4.csv file. Once performed, the Digitization-Examples script can be run. Expected Output: For binary logistic regression, expect the accuracy, ROC curve and AUC to be logged for each test case. For multinomail, expect the accuracy along with a confusion matrix to be logged.

   Data: 
   
      ingredients_v1.csv : 

      ingredients_v2.csv: 

      ingredients_v3.csv: Both recipes and ingredients are stemmed and converted to lower case. No truncation was applied yet.

      ingredients_v4.csv: Ingredients which counts less than 25 can be truncated.
      Then these ingredients can be found in recipes and deleted from there. (Only ingredients not recipes)
      Then recipes which have less than 5 ingredients can be truncated as well.

      recipes-properties.csv : 

      recipes-scores.csv :

      recipes_v3.csv :

      recipes_v4.csv : 

      fast_text_input.txt : 
          
       
```


### Contributions 
We encourage the collaborative extention of our work. To simplify the process we monitor this repository's Issue tracker for requests of new terms/classes. We also check for reported errors or specific concerns related to the data.
