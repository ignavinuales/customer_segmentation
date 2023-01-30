# Customer segmentation with KMeans to help define marketing strategies

Market segmentation is the process of breaking a large consumer or company market into smaller consumer groups based on similar characteristics. 

This project aims at segmenting some active credit card holders to help the marketing department to build different strategies for each customer segment. Furthermore, after performing clustering, it is important to identify the customer profile of each cluster. Then, 

*Objectives*: perform customer segmentation and identify customer profiles.

*Methodology*:
1. Explore and understand the data. 
2. Data preprocessing and explanatory data analysis.
3. Perform clustering using KMeans.
4. Analyze the results and create customer profiles.

## Brief description of the data

The dataset contains information on about 9,000 customers during the last six months. Among the 17 features, we find: 
- Balance: balance in the account
- Purchases: the amount of money spent from the account. 
- Installment purchases: purchases done in installment
- Cash advance: purchases made upfront.
- Purchases frequency: how frequently the purchases are made.

## Results
After trying different number of clusters, the customers were segmented into *three groups*. The figure below shows how the clusters are sparse on a 3-dimensional space using PCA:

<img src="https://github.com/ignavinuales/customer_segmentation/blob/main/clusterPCA.png"  width="350" height="350">

### Customer profiles
The three clusters were given names as part of the process of building profiles. They were named *spenders*, *average*, and *savers*. Along with other plots, a radar chart was one of the tools used to find those customer profiles, which shows the mean value of the features for each cluster: 

<img src="https://github.com/ignavinuales/customer_segmentation/blob/main/radar_chart.png"  width="550" height="450">

*The spenders*:
 - These customers are by far the ones who spend the most, as the mean of *purchases* is way bigger than the rest of the clusters. 
 - They not only spend more but also more often.
 - Most of the purchases are one-time purchases. 
 - They mostly make purchases in installments, with almost no cash in advance. 
 - They also have a bigger credit limit, and their percentage of full payments is the highest among all clusters. 

*The average*:
 - These customers have much lower balance overall. 
 - They show a more restrained or moderate consumption, in accordance with their balance.
 - Their spendings are slightly higher on installments, but relatively balanced with upfront payments.
 - They have a low credit limit.

*The savers*:
- They have the biggest balance of all. However, these are the ones who spend the least money.
- They pay upfront and barely in installments.
- They have the lowest purchase frequency.

### Conclusion
The clustering model and further analysis helped to cluster the customers into three categories: savers, average, and spenders. Each segment presents common characteristics that should help develop different marketing strategies. 

---
Dataset source: [Link to data source](https://www.kaggle.com/datasets/shivamb/machine-predictive-maintenance-classification)
