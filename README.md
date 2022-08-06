# Segment clients of an e-commerce platform

### Overview: Clustering of customers of an e-commerce database for the marketing team. 
### Definition of a maintenance contract for the trained algorithm.

The provided data set is relatively clean (one only has to do typical table joins with aggregations to avoid the duplication of individuals). The dataset allows the engineering of many possible features (sensibility to events, urban density, etc.). 

Several metrics can be helpful in the determination of clusters (Inertie, Silhouette), but the need for marketing actionability of the segments is prioritized here. Therefore, a parallel plot is extensively used to visualize the discriminational power of the models. 

Several unsupervised models (Kmeans, DBSCAN, Hierarchical Clustering) are compared over different feature selections (with a marketing's RFM feature selection as a baseline). A Kmeans with eight components allows defining eight segments that discriminate over hapiness, recency, cost sensitivity, delay of shipping, size of the basket, and sensitivity to events. 

To define the maintenance contract, one can compare the predictions of the same model fitted with different amounts of data and study the evolution of the ARI score over time.
