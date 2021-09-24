# Cryptocurrencies

## Overview
Using Pandas, the challenge was to preprocess a dataset in order to perform Principle Component Analysis (PCA). This method is often used in order to reduce the dimentionality of larger datasets, while still containing most of the information in that numerical value. But what exactly are we doing PCA on? Glad you asked, we are performing tihs on crypto currencies in order to cluster the data to find meaningful insights. 

## Summary
The data had a lot of columns, so the first step was to reduct the columns by cleaning the ones that were not going to be providing any value like the "IsTrading" column as an example. Removing rows that had null values was also part of the preprocessing step so there was no missing information in any row. We also used GetDummies in order to transform the string names of the "ProofType" column into numerical values that the PCA model could then read/quantify. "StandardScaler" was used to standardize the data and this is an important part because we do not want certain columns outweighing other variables so everything could be evenly distributed. Once the data was processed, I diluted the number of variables into 3 different PCs titled "PC 1" "PC 2" "PC 3".
The image below shows the end result with 3 different clusters. 
![image](https://user-images.githubusercontent.com/80786853/134734916-ed7ecce0-179a-4506-a603-acf4017ab768.png)
