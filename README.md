# Ensemble-Methods

# Bagging And Boosting

Understanding the Business Problem.

TalkingData is a Chinese big data company, and one of their areas of expertise is mobile advertisements.

In mobile advertisements, click fraud is a major source of losses. Click fraud is the practice of repeatedly clicking on an advertisement hosted on a website with the intention of generating revenue for the host website or draining revenue from the advertiser.

In this case, TalkingData happens to be serving the advertisers (their clients). TalkingData cover a whopping approx. 70% of the active mobile devices in China, of which 90% are potentially fraudulent (i.e. the user is actually not going to download the app after clicking).

You can imagine the amount of money they can help clients save if they are able to predict whether a given click is fraudulent (or equivalently, whether a given click will result in a download).

Their current approach to solve this problem is that they've generated a blacklist of IP addresses - those IPs which produce lots of clicks, but never install any apps. Now, they want to try some advanced techniques to predict the probability of a click being genuine/fraud.

In this problem, we will use the features associated with clicks, such as IP address, operating system, device type, time of click etc. to predict the probability of a click being fraud.

# Bagging and Boosting ensemble model:

1. Explore the dataset for anomalies and missing values and take corrective actions if necessary.

2. Which column has maximum number of unique values present among all the available columns.

3. Use an appropriate technique to get rid of all the apps that are very rare (say which comprise of less than 20% clicks) and plot the rest.

4. Divide the data into training and testing subsets into 80:20 ratio(Train_data = 80% , Testing_data = 20%).

5. Apply XGBoostClassifier.

6. Apply BaggingClassifier.

7. What is the accuracy for BaggingClassifier and XGBoostClassifier?.
