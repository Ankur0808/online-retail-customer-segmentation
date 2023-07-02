# online-retail-customer-segmentation


# Problem Description:
In this project, your task is to identify major customer segments on a transnational data set that contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

# Attribute Information:
* Invoice No: Invoice number. Nominal, is a 6-digit integral number uniquely assigned to each transaction. If this code starts with the letter 'c', it indicates a cancellation.
* StockCode: Product (item) code. Nominal, is a 5-digit integral number uniquely assigned to each distinct product.
* Description: Product (item) name. Nominal.
* Quantity: The quantities of each product (item) per transaction. Numeric.
* InvoiceDate: Invoice Date and time. Numeric, the day and time when each transaction was generated.
* UnitPrice: Unit price. Numeric, Product price per unit in sterling.
* CustomerID: Customer number. Nominal, is a 5-digit integral number uniquely assigned to each customer.
* Country: Country name. Nominal, is the name of the country where each customer resides.

# Summary:
In this project, our task was to identify major customer segments on a transnational data set that contained one-year historical transactions for a UK-based online retail store. This would help the company segregate its customers based on transaction data and help them in marketing decisions and strategy.

After basic exploration and cleaning of the data, we found relationships between features in EDA and then jumped into the analysis part. RFM analysis helped us to identify the Platinum and Gold Customers who bring more profit for the Online retail stores as well helped to focus on Silver and Bronze type of customers by organizing some attractive offers for them.

We implemented various unsupervised machine learning algorithms such as KMeans Clustering, DBSCAN Algorithm, and Hierarchical Clustering(Agglomerative Clustering). Here to find the Optimal number of clusters we used the Elbow method as well as using Elbow Visulizers by Yellow bricks from the Scikit Learn library. Also, we used Silhouette Score and Silhouette Plot to visualize the clusters with different numbers of clusters. For Agglomerative Clustering, we used Dendogram to find the optimal number of clusters.


# Challenges:
* Data cleaning
* RFM analysis
* Deciding the optimal number of clusters

# Conlcusions:
* We got an optimal number of clusters=2 with the help of the Elbow method and Silhouette score.
* Cluster 0 has a high recency rate but very low frequency and monetary. Cluster 0 contains 2414 customers.
* Cluster 1 has a low recency rate but they are frequent buyers and spend very high money than other customers as the mean monetary value is very high. Thus generating more revenue for the retail business.

With this, we are done. Also, we can use a more robust analysis for the clustering, using not only RFM but other metrics such as demographics or product features.
