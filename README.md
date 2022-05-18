# Sales-data-to-identify-product-bundles

I have done a data science project using R, where subjective segmentation techniques are being shown which is actually a clustering method to find out the product bundles in sales data

# Problem Statement

The sales transaction dataset have weekly purchased quantities of 800 products over 52 weeks. Normalised values are provided too. So the main objective of this project is to identify the product bundles which can be put as a whole on sale. In general, Market basket analysis ( **a data mining technique used by retailers to increase sales by better understanding customer purchasing patterns** ) was used to identify those bundles. We will compare the relative importance of time series clustering in identifying product bundles.

# Description and Overview

**DATA PRE-PROCESSING** :
           It is a data mining technique which is used to transform the raw data in useful and efficient format. It usually involves three steps
           
   ![image](https://user-images.githubusercontent.com/86511074/169047761-37a02ef2-7f06-4d4c-a03d-1c9505a1539b.png)

Here we are using clustering for data cleaning of noisy data, There are different techniques for clustering,
* Partition based methods
* Heirarchical methods
* Model based methods

We are using K means clustering ( **a type of unsupervised learning, which is used when you have unlabeled data** ). K means algorithm is available in 3 different R libraries
* Rcmdr - Kmeans
* stats - Kmeans
* AMAP - Kmeans

**STEPS INVOLVED IN K-MEANS ALGORITHM**
* Step 1 : To identify the value of K
* Step 2 : How to select K
* Step 3 : Decide the distance function
* Step 4 : Decide the iterations
* Step 5 : Get clusters
* Step 6 : Make profiling

So to select the value of K, a screenplot approach is being used. Screenplot shows the within group of sum of squares with the corresponding number of clusters. As the number of cluster increases, the within sum of squares(wss) will decrease eventually a point will come where the wss will not drop further that is the optimal scenario when the cluster is giving us best result.

![image](https://user-images.githubusercontent.com/86511074/169051287-14747e6e-32e7-446a-81ab-b6cd4365da1f.png)


