# Cryptocurrencies

For this analysis(CHALLENGE) I am slated to use machine learning models in order to group cryptocurrencies.  I will use custering algorithms(upsupervised - non-labeled data) with the cryptocurrency data csv that is provided/cleansed.

# Results:

## Deliverable 1: Preprocessing the Data for PCA(Principal Component Analysis)

Preprocessing the data, we removed unnecessary columns.  The column "IsTrading" was dropped, and the "Unnamed: 0" column was renamed with a blank name, and also used as an index.  "DROPNA" function was used on all columns.

![image](https://user-images.githubusercontent.com/8845050/184172367-fdeb029d-b4f8-4624-935d-722c6efadc1f.png)

We also wanted to see any rows where "Total Coins Mined" were greater than ZERO, and identified the "CoinName" of those filtered rows.  We dropped that column from the cluster table, moving forward.

![image](https://user-images.githubusercontent.com/8845050/184172793-0425715a-4270-46be-bf86-a07642a49b10.png)

We added dummy data, using the pd.get_dummies function to the columns "ALGORITHM" and "PROOFTYPE", applied the fit_transform to SCALE the data into a more fungible number.  

![image](https://user-images.githubusercontent.com/8845050/184172894-1dac494f-23be-4fcf-aa2f-119180759d34.png)

![image](https://user-images.githubusercontent.com/8845050/184173009-9f999711-c007-4ecb-877b-d3a48be96511.png)

![image](https://user-images.githubusercontent.com/8845050/184173106-5b4eadc6-6c95-40dc-9fbe-59f046ab8ca0.png)

## Deliverable 2:  Reducting the Data Dimensions Using PCA


## Deliverable 3: Clustering CryptoCurrencies Using k-Means


## Deliverable 4:  Visualizing Cryptocurrencies Results


