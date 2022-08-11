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

## Deliverable 2:  Reducting the Data Dimensions Using PCA

In Dleiverable 2, I applied the PCA algorithm(Principal Component Analysis) to reduce the dimensions of the Dataframe to support THREE components, and places these in a new DataFrame.

![image](https://user-images.githubusercontent.com/8845050/184173527-f0aa7d6e-d3cf-4fe3-9f7b-20528504268f.png)


## Deliverable 3: Clustering CryptoCurrencies Using k-Means

Here, I created an elbow curve using HVPLOT to find where the best value for K.  Where the BEND is created, thats your optimal K value.

![image](https://user-images.githubusercontent.com/8845050/184174462-2a62be72-4f07-499d-a456-5d91004fcbfe.png)

Initialize the model:

![image](https://user-images.githubusercontent.com/8845050/184174940-c642fb69-fb0f-41b1-ba39-38f126496244.png)

Created new dataframe, concatenating original DF with PCA DF, and added column "CoinName" to the new dataframe.

![image](https://user-images.githubusercontent.com/8845050/184175887-f2e860ee-44a1-4842-89c5-e0c92e0b0b6e.png)

## Deliverable 4:  Visualizing Cryptocurrencies Results


