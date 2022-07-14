# KKBox Churn Rate Prediction Capstone Project

:notes: Hello! :wave: This repository contains my machine learning capstone project on Churn Rate Prediction for KKBox :notes:

**The datasets used for this project can be found here:**

- https://www.kaggle.com/competitions/kkbox-churn-prediction-challenge/data

### Run Notebooks in the following order:

1. KKBox_EDA
2. KKBox_Feature_Engineering
3. KKBox_Correcting_Imbalance_with_Sampling_Techniques_and_Logistic_Modelling
4. KKBox_Random_Forest_Model_Feature_Importance

https://www.appbrain.com/app/kkbox-%7C-music-and-podcasts/com.skysoft.kkbox.android![image](https://user-images.githubusercontent.com/50337807/179073301-4e8a5315-daad-4687-b791-9504a7d8d6c7.png)


### Data Dictionary

**train_v2.csv**
The train set, containing the user ids and whether they have churned:

- msno: user id
- is_churn: This is the target variable. Churn is defined as whether the user did not continue the subscription within 30 days of expiration. is_churn = 1 means churn,is_churn = 0 means renewal.

**transactions.csv**
Transactions of users up until 2/28/2017.

- msno: user id
- payment_method_id: payment method
- payment_plan_days: length of membership plan in days
- plan_list_price: in New Taiwan Dollar (NTD)
- actual_amount_paid: in New Taiwan Dollar (NTD)
- is_auto_renew
- transaction_date: format %Y%m%d
- membership_expire_date: format %Y%m%d
- is_cancel: whether or not the user canceled the membership in this transaction.

**transactions_v2.csv**
Same format as transactions.csv, refreshed 11/06/2017, contains the transactions data until 3/31/2017.

**user_logs_v2.csv**
Daily user logs describing listening behaviors of a user. Data collected until 3/31/2017.
- msno: user id
- date: format %Y%m%d
- num_25: # of songs played less than 25% of the song length
- num_50: # of songs played between 25% to 50% of the song length
- num_75: # of songs played between 50% to 75% of the song length
- num_985: # of songs played between 75% to 98.5% of the song length
- num_100: # of songs played over 98.5% of the song length
- num_unq: # of unique songs played
- total_secs: total seconds played

**members_v3.csv**
User information. Note that not every user in the dataset is available.
- msno: user id
- city
- bd: age
- gender
- registered_via: registration method
- registration_init_time: format %Y%m%d
