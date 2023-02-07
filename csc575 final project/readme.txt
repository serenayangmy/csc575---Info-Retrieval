- EDA.ipynb
Data Exploration

- collaborative_based.ipynb
Collaborative based for Recommendation:
1. Place the following files in a same folder:
	i. transactions_train_data.csv
	ii. customers_train_data
	iii. articles
	iv. collaborative_based.ipynb
2. Run the collaborative_based.ipynb jupyter notebook except the very last line of the code.
3. To initiate the system, use predict_error to test and review the system's accuracy report.
4. predict function required to know the customer's ID to run, therefore, you should check the train_data dictionary for a customer_id to run the function
5. Same for get_knn function, you are required to have a customer's ID for it to run
6. demo code were included in the notebook 

-content_based & rule_based.ipynb
Content Based for Recommendation:
1. Loading articles and transaction file
2. Transactions dataset train_test_split

*Content based with all categories
3. Select model with all categories and change the transaction table and article_features table from
DataFrame to dictionary for further use
4. create two sets. One set stores all the articles IDs and each article’s features that we want to analyze. Another set stores each user’s ID, and each user purchases articles’ IDs. 
5. to get most K similar articles for each article
6. store the recommended article into a dictionary {'user_id':[recommended list]}
7. set K=50, run the transaction training dataset to get all the recommended articles for all users

*Content based with two categories
3. reload article_feature to select only two categories
4. re-create the same two sets. One set stores all the articles IDs and each article’s features that we want to analyze. Another set stores each user’s ID, and each user purchases articles’ IDs. 
5. set K=50, run the transaction training dataset to get all the recommended articles for all users

*top_50 items in the past three weeks
1. Reload transaction dataset
2. To get the newest date from the entire transaction dataset
3. filter all the transactions before the (newest date-3 weeks), which is ‘2020-09-01’, and then group ‘customer_id’ by the ‘article_id’

*popular_50 items in the past three weeks
4. group ‘customer_id’ by the ‘article_id’

*Get accuracy
1.transactions dataset train_test_split
2.to run the transaction test dataset line by line, to check whether the user purchased article is in the recommended list accuracy = # of failed in items/recommended list size

-FinalReport.pdf
-data folder
inclueds: article.csv, customer.csv, transaction_train.csv
-Final Presentation.pptx
