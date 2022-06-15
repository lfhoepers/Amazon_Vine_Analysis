# Challenge 16 Amazon Vine Analysis

## Overview of the Project 
The project consists in pick one of the amazon review datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, we’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members on the dataset.


## Deliverable 1

[Amazon_Reviews_ETL.ipynb](https://github.com/lfhoepers/Amazon_Vine_Analysis/blob/6ab49a0d519bb434c787b6fd0f7f1f4b77e675e6/Amazon_Reviews_ETL.ipynb)

- An Amazon Review dataset is extracted as a DataFrame

![image](https://user-images.githubusercontent.com/100812079/173956478-08477bc3-6939-4409-bab6-873ff8fc0a2a.png)


- The extracted dataset is transformed into four DataFrames with the correct columns

![image](https://user-images.githubusercontent.com/100812079/173956594-ae4448b2-fd51-46da-aace-17e79dd59ba7.png)

![image](https://user-images.githubusercontent.com/100812079/173956627-21d34da9-4427-409e-a7ec-49bba1ef6249.png)

![image](https://user-images.githubusercontent.com/100812079/173956658-be80348c-1ecc-4ddd-bf91-fbd5b65418f0.png)

![image](https://user-images.githubusercontent.com/100812079/173956685-576c2372-def0-4687-afed-4ee2ab85410d.png)


- All four DataFrames are loaded into their respective tables in pgAdmin
  
![image](https://user-images.githubusercontent.com/100812079/173957000-636818eb-3c06-4473-8d07-a8096bc968d8.png)

![image](https://user-images.githubusercontent.com/100812079/173957148-348373a2-6378-41c9-b84a-577f09a8aee4.png)

![image](https://user-images.githubusercontent.com/100812079/173957181-2e6ec3bf-45d9-46f5-a308-0eca5ef0f8cc.png)

![image](https://user-images.githubusercontent.com/100812079/173957212-756b66e2-1780-4270-8ba5-33b34f133938.png)


## Deliverable 2

[Vine_Review_Analysis.ipynb](https://github.com/lfhoepers/Amazon_Vine_Analysis/blob/de8df6ba81bdd5ab1a75c8cb4beb7f4b13635c9f/Vine_Review_Analysis.ipynb)

- There is a DataFrame or table for the vine_table data using one of three methods

![image](https://user-images.githubusercontent.com/100812079/173958466-deaf9550-abd0-49ed-85a9-3cc8dd26a28e.png)

![image](https://user-images.githubusercontent.com/100812079/173958524-162c6429-90e0-4cb6-ab17-793191496994.png)


- The data is filtered to create a DataFrame or table where there are 20 or more total votes 

![image](https://user-images.githubusercontent.com/100812079/173958536-fb47e61c-04cf-49a6-bd3f-9ee54b6b9887.png)


- The data is filtered to create a DataFrame or table where the percentage of helpful_votes is equal to or greater than 50% 

![image](https://user-images.githubusercontent.com/100812079/173958637-fe6bb430-43ef-4d95-bc2a-45d453d57384.png)


- The data is filtered to create a DataFrame or table where there is a Vine review

![image](https://user-images.githubusercontent.com/100812079/173958558-12decba2-6eb8-4297-a79c-4a047c903e8e.png)


- The data is filtered to create a DataFrame or table where there isn’t a Vine review 

![image](https://user-images.githubusercontent.com/100812079/173958587-e6c9c44f-2693-4bed-a09b-cc621dd86211.png)


- The total number of reviews, the number of 5-star reviews, and the percentage 5-star reviews are calculated for all Vine and non-Vine reviews

![image](https://user-images.githubusercontent.com/100812079/173960113-2ad5d016-7d1b-400e-ac77-5a81334a2753.png)


## Deliverable 3

**Results**

- How many Vine reviews and non-Vine reviews were there?

Vine 94

Non-Vine 40471

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?


Vine - 48

Non Vine 15663

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?


Vine 51.06%

Non Vine 38.7%


**Summary**

Based on the results, we can conclude that there was no bias found in the reviews of the vine members for the Video game dataset. 
We have only 51% of the paid members provided 5 star ratings, and non-paid members providing 5 star raings is much higher at 38.7%. the difference is too low.

For me the numbers of paid is too low to have any decision.
Following a list of paid vine for each star.

![image](https://user-images.githubusercontent.com/100812079/173960487-038a69a9-1848-4ac8-b01f-8cc963de0188.png)


I appreciate the opportunity to present this project, I am available for any clarification.

**Luiz Fernando Hoepers**

**UofT SCS Data Analytics Boot Camp**
