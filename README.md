# Cryptocurrencies
Unsupervised Machine Learning

- Resources
    - Python3.7
    - Jupyter Notebook
    - Scikit-learn: KMeans, PCA
    - Visualizations: hvplot, plotly
    - Modeling
        - KMeans Clustering
        - Principal Component Analysis (PCA)

## Overview

Often, new investors in cryptocurrencies are overcome with indecision and may feel transfixed by the plethera of options to chose from.  With the implementation of the K-Means Clustering unsupervised machine learning model, we hope to classify all coins in our database to provide an enhanced understanding for investors.  

## Procedure

First, I preprocessed the data by selecting features relevant to this analysis, selected rows for all cryptocurrencies that are actively trading, encoded strings by assigning them a numeric value (too many to fit in screenshot below), and generally cleaned up the database by dropping null values (that would effect the modeling process).
![Screen Shot 2022-07-22 at 11 13 57 AM](https://user-images.githubusercontent.com/100544761/180481655-cf071c83-d6f8-48ae-80d6-47ad6a8afa5c.png)

Next, features were standardized using scikit-learn's StandardScaler().  Then, Principal Component Analysis (PCA) was administered to reduce dimensionality by essentially converging our relevant features into a smaller number, retaining helpful information while improving performance. 
![Screen Shot 2022-07-22 at 11 15 46 AM](https://user-images.githubusercontent.com/100544761/180482357-8de002e5-ba1a-49a5-9176-75d28c48b924.png)

An Elbow Curve was created to discover optimal number of clusters to provide the KMeans model.
![Screen Shot 2022-07-22 at 11 25 00 AM](https://user-images.githubusercontent.com/100544761/180482747-47edd9f6-395b-4bbb-b63b-a180d67e8d00.png)</br>
![Screen Shot 2022-07-22 at 11 25 39 AM](https://user-images.githubusercontent.com/100544761/180482848-5bfae95b-91aa-4dc7-a8d2-7e83e91e79fe.png)

KMeans Clustering classified the data.
![Screen Shot 2022-07-22 at 11 16 44 AM](https://user-images.githubusercontent.com/100544761/180482984-eb94561f-0a4a-4f45-9a13-77ea4c081b7f.png)
 
Joined the DataFrames into one to display clustered data.
![Screen Shot 2022-07-22 at 11 27 11 AM](https://user-images.githubusercontent.com/100544761/180483129-fb671ff2-e913-452d-9710-2da5b102d407.png)

Most cryptocurrencies fell within 2 classes.
![Screen Shot 2022-07-22 at 11 28 07 AM](https://user-images.githubusercontent.com/100544761/180483214-b009d222-0ddc-49a3-81f9-873b1bbd0018.png)

3D view of our clusters.
![Screen Shot 2022-07-22 at 11 17 37 AM](https://user-images.githubusercontent.com/100544761/180483305-68701c56-6cfb-4c7a-84f5-227298cc9a11.png)

MinMaxScaler() to better view the relationship between coin supply and mined.
![Screen Shot 2022-07-22 at 11 29 35 AM](https://user-images.githubusercontent.com/100544761/180483582-ba627cee-64bf-410d-bd98-e28c44dbce5d.png)

2D representation of relationship.
![Screen Shot 2022-07-22 at 11 18 28 AM](https://user-images.githubusercontent.com/100544761/180483650-0fb4c015-d46c-430d-ba01-469cc3faa3ff.png)

## Results

We can see clear classification of our data in the 3D graph.  Our model will be able to predict with new data which class each coin will fall into.  Further analysis is needed before suggesting currencies for our clients to invest in, however, this is a decent first step in better understanding our data.  

### Contact

[Email](mrmileyy@gmail.com)</br>
[LinkedIn](https://www.linkedin.com/in/mileymarshall)