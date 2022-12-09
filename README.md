# `Cryptocurrencies _Analysis`

## `Project Overview ` <br/>

Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. The purpose of Cryptocurrencies _Analysis is  to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. <br/>

#### `Resources` <br/>
• Data Source: [Google](https://www.google.com/), [Starter Code](https://github.com/Valeriia161/Cryptocurrencies/blob/main/Starter_Code/Crypto_clustering_started_code.ipynb) . <br/> 
•	Software: Jupyter Notebook, Pandas ,Git Bash, GitHub. <br/>

# `Result ` <br/>
•	`Deliverable 1: Preprocessing the Data for PCA`   <br/>
Using  knowledge of Pandas, I preprocessed the dataset in order to perform PCA in Deliverable 2. <br/>
Preprocessing was including: <br/>
1.	Reading in the crypto_data.csv to the Pandas DataFrame .  <br/>
2.	Kepting all the cryptocurrencies that are being traded. <br/>
3.	Dropping the IsTrading column. <br/>
4.	Removing rows that have at least one null value. <br/>
5.	Filtering DataFrame so it only has rows where coins have been mined. <br/>
6.	Creating a new DataFrame that holds only the cryptocurrency name. <br/>
7.	Removing the CoinName column since it's not going to be used on the clustering algorithm. <br/>

8.	Creating variables for the two text features, Algorithm and ProofType, and storing the resulting data in a new DataFrame named X. <br/>
9.	Standardizing the features from the X DataFrame. <br/>

![image](https://user-images.githubusercontent.com/110998103/206725177-e2ec86d6-a7c3-4fec-b71f-cbb90556d054.png)


•	`Deliverable 2: Reducing Data Dimensions Using PCA`  <br/>
Using knowledge of how to apply the Principal Component Analysis (PCA) algorithm, I reduced the dimensions of the X DataFrame to three principal components and placed these dimensions in a new DataFrame. <br/>


![image](https://user-images.githubusercontent.com/110998103/206726803-f2396ba1-5f2c-49aa-9427-fed83f963b8c.png)


•	`Deliverable 3: Clustering Cryptocurrencies Using K-means` <br/>
Using knowledge of the K-means algorithm, I created an elbow curve using hvPlot to find the best value for K from the pcs_df DataFrame created in Deliverable 2. <br/>

![image](https://user-images.githubusercontent.com/110998103/206727483-ac2fca37-d33e-4f93-bc73-2c9f8a3c70ef.png)


Then, I ran the K-means algorithm to predict the K clusters for the cryptocurrencies’ data. <br/>

![image](https://user-images.githubusercontent.com/110998103/206727713-6f2cbc5c-d30c-4229-84b8-e86ffe015e2d.png)
![image](https://user-images.githubusercontent.com/110998103/206727859-c669e607-cfc4-4a81-86da-5b335855b475.png)



•	`Deliverable 4: Visualizing Cryptocurrencies Results`  <br/>
Using knowledge of creating scatter plots with Plotly Express and hvplot, I visualized the distinct groups that correspond to the three principal components I created in Deliverable 2. <br/>

![image](https://user-images.githubusercontent.com/110998103/206728826-266d8c4f-7658-42c3-b720-c8efb15a836a.png)


Then I created a table with all the currently tradable cryptocurrencies using the hvplot.table() function. <br/>

![image](https://user-images.githubusercontent.com/110998103/206728977-776c5ede-ab5a-4d02-be67-ccf6235b8eb3.png)

And finaly I created an hvplot scatter plot with x="TotalCoinsMined", y="TotalCoinSupply", and by="Class". <br/>

![image](https://user-images.githubusercontent.com/110998103/206729566-43d73731-24f6-49a2-852d-9affffc43f13.png)

##  `Summary` <br/>



