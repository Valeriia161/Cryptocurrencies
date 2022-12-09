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


