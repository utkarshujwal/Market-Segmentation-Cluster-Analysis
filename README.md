# Market-Segmentation-Cluster-Analysis
## Market Segmentation of consumers on basis of purchase behavior (volume, frequency, and brand loyalty)  and basis of purchase (price, selling proposition)


### Bsuiness Problem Statement:
CRISA is a leading market research agency that specializes in tracking consumer purchase
behavior in consumer goods (both durable and non-durable). In one major project, CRISA tracks
about 30 product categories (e.g. detergents, etc.) and within each category, about 60 – 70 brands.
To track purchase behavior, CRISA has constituted about 50,000 household panels in 105 cities
and towns in India, covering about 80% of the Indian urban market. (In addition to this, there are
25,000 sample households selected in rural areas; however, we are working with only urban
market data). The households are carefully selected using stratified sampling. The strata are
defined on the basis of socio-economic status, and the market (a collection of cities).
CRISA has both transaction data (each row is a transaction) and household data (each row is a
household), and, for the household data, maintains the following information:

• Demographics of the households (updated annually).

• Possession of durable goods (car, washing machine, etc.; updated annually) and a
computed "affluence index" on this basis.

• Purchase data of product categories and brands (updated monthly).

CRISA has two categories of clients: (1) Advertising agencies who subscribe to the database
services; they obtain updated data every month and use it to advise their clients on advertising
and promotion strategies. (2) Consumer goods manufacturers who monitor their market share
using the CRISA database.

### Cluster based on "Purchase Behaviour"

Some thought is needed about brand loyalty. For brand loyalty indicators the variables used are :
1.	Number of brands
2.	Brand runs
3.	total volume
4.	No. of transactions
5.	percent of purchases devoted to major brands (i.e. is a customer a total devotee of brand A/B/C?)


**K-Means clustering using purchase behavior variables:**

 ![image](https://user-images.githubusercontent.com/29014647/119584490-3eb53200-bd8e-11eb-881f-4c0126b0f1a6.png)

 ![image](https://user-images.githubusercontent.com/29014647/119584579-74f2b180-bd8e-11eb-9eec-f5dafe2f5c1f.png)  ![image](https://user-images.githubusercontent.com/29014647/119584593-7ae89280-bd8e-11eb-94d8-9cbd9c0ea334.png)
 
Properties of each cluster:
Cluster 1: In Cluster 1 the maximum number of customers are from SEC2(30%), 95% of them are female customers, have upto high school education, are 45 years or older, there are no children present in their households, have an affluence index of 21% and are 23% loyal to brands they purchase.


**Partitioning Around Mediods using Purchase Behavior variables:**

![image](https://user-images.githubusercontent.com/29014647/119584490-3eb53200-bd8e-11eb-881f-4c0126b0f1a6.png) 
![image](https://user-images.githubusercontent.com/29014647/119587352-234d2580-bd94-11eb-93aa-7e32fc022164.png)

Hierarical Clustering using Purchase Behavior variable (Agglomerative Clustering Using Ward method):
Agglomerative Coefficient using ward method = 97.67%![image](https://user-images.githubusercontent.com/29014647/119587593-9a82b980-bd94-11eb-96bf-dab5957633e0.png)

![image](https://user-images.githubusercontent.com/29014647/119587382-38c24f80-bd94-11eb-999c-5131667471f8.png)

![image](https://user-images.githubusercontent.com/29014647/119587606-a1a9c780-bd94-11eb-8480-a9f01a992117.png) ![image](https://user-images.githubusercontent.com/29014647/119587623-aa020280-bd94-11eb-9b68-ac956338a247.png)

**Kernel k-means using purchase behavior variables:**

![image](https://user-images.githubusercontent.com/29014647/119587729-e6356300-bd94-11eb-85c7-ae1063017970.png)

Cluster size:  
[124 159 317]

Within-cluster sum of squares:  
[2596.089 1574.408 2993.132]


### Cluster based on "Basis of Purchase"
 
We have taken Maximum value of Percentage of volume purchased under different promotions; Percentage of volume purchased under the price category and Percent of volume purchased under the product selling proposition category because when we are trying to segment a particular demographic in any cluster consisting of households we would like to know when and where that household spends the most to capture an essence of their purchase proclivity which helps us to target them and segment them better otherwise there would be a lot of overlap between the cluster demographics.


**K-Means clustering using basis of purchase variables**

![image](https://user-images.githubusercontent.com/29014647/119587988-78d60200-bd95-11eb-8135-346fef7a09e8.png)


![image](https://user-images.githubusercontent.com/29014647/119588002-7e334c80-bd95-11eb-83cc-91d16df4d600.png) ![image](https://user-images.githubusercontent.com/29014647/119588015-82f80080-bd95-11eb-999b-a9a19e580b3e.png)


**Partitioning around medoids using basis of purchase variables**

![image](https://user-images.githubusercontent.com/29014647/119588073-a02ccf00-bd95-11eb-8f51-afbf891e55e1.png)

![image](https://user-images.githubusercontent.com/29014647/119588081-a622b000-bd95-11eb-85e6-860ea6df892d.png)

**Hierarchical Clustering using basis of purchase variables(ward)**

![image](https://user-images.githubusercontent.com/29014647/119588169-dbc79900-bd95-11eb-92b4-10fa75db3e07.png)

![image](https://user-images.githubusercontent.com/29014647/119588175-e08c4d00-bd95-11eb-8b96-26eaa0b0af18.png)

![image](https://user-images.githubusercontent.com/29014647/119588184-e5e99780-bd95-11eb-873b-2718023ec0f2.png)


**Kernel k-means using basis of purchase variables**

![image](https://user-images.githubusercontent.com/29014647/119588222-f6017700-bd95-11eb-93fc-69cde50f7c70.png)

Cluster size:  
[117  37 446]

Within-cluster sum of squares:  
[138.7409 339.9104 922.1055]



### Cluster based on "Basis of Purchase" & "Purchase Behaviour"

**K-Means clustering using both purchase behavior and basis of purchase variables**

![image](https://user-images.githubusercontent.com/29014647/119588457-73c58280-bd96-11eb-84b8-a13ab86bfb94.png)

![image](https://user-images.githubusercontent.com/29014647/119588461-77f1a000-bd96-11eb-98e6-539a87151b75.png) ![image](https://user-images.githubusercontent.com/29014647/119588473-7d4eea80-bd96-11eb-8042-e11ca0696be8.png)

We have taken centers = 6 because, In the elbow plot, the slope (total within clusters sum of squares) is not changing drastically after K = 6.


**Partitioning around medoids using both purchase behavior and basis of purchase variables**

![image](https://user-images.githubusercontent.com/29014647/119588531-a3748a80-bd96-11eb-8a9b-f803bed98b03.png)

![image](https://user-images.githubusercontent.com/29014647/119588543-a8d1d500-bd96-11eb-853b-0ea26415a404.png)

**Hierarchical Clustering using both purchase behavior and basis of purchase variables**
Agglomerative Coefficient using ward method = 96.89%

![image](https://user-images.githubusercontent.com/29014647/119588595-c010c280-bd96-11eb-99b1-0f1e5dac317f.png)

![image](https://user-images.githubusercontent.com/29014647/119588601-c30bb300-bd96-11eb-8598-764c1e9779f9.png) ![image](https://user-images.githubusercontent.com/29014647/119588611-c737d080-bd96-11eb-9154-ac3cca407248.png)

The Clusters obtained from the different methods are different, but the difference is very subtle.
When we talk about segmentation on the basis of purchase behavior (PB) and obtain the clusters based on 3 different approaches namely
•	K means approach gives best result with a total of 3 clusters with least amount of overlap between the clusters compared to PAM or agglomerative approach in which the clusters are not properly segmented.

When we go about segmentation on the basis of basis for purchase (BOP)
•	Still we get the best result when clustered by K means as the 3 clusters obtained are with almost no amount of overlap whereas we observe a significant amount of overlap in clusters in PAM and agglomerative and as we are aware that the best cluster is the one with maximum inter cluster distance. Although the difference between PAM and K means model is significantly small and additionally the clusters in PAM have equal number of data points in each cluster.

When are segment each household on the basis of both on purchase behavior (PB) and basis of purchase (BOP) 
•	Still the K means provides us with the best result compared to other two because it gives the least overlap between the cluster and we can target the more customers based on targeted strategy (i.e. when the overlap will be less).


There are 4 types of market segmentation, but now here we are only focusing on demographic segmentation based on the data for age, gender, educational background, social economic factor (SEC).

So, we have divided the data and segmented them in the clusters based on three criteria:

●	Purchase behavior (PB)
●	Basis of purchase (BOP)
●	Both

Now when we take purchase behavior (PB) criteria we segment our demographic into 3 clusters and the best segmentation was done by using K means

Cluster 1:  In Cluster 1 the maximum number of customers are from SEC_4(37%), 83% of them are female customers, have up to high school education, are 45 years or older, there are no children present in their households, have an affluence index of 13% and are 72% loyal to brands they purchase and 50% of them are buying any popular soap.
Cluster 2: In Cluster 2 the maximum number of customers are from SEC_1(31%), 80% of them are female customers, are literate without formal schooling, are 45 years or older, there are no children present in their households and mostly buying any popular soap.
Cluster 3: The customers are mostly female with SEC_2(30%) who all the college graduate with 20% affluence index.

Now again the on the basis for purchase (BOP) we have segmented our demographic in 3 cluster and best segregated cluster was obtained by K means:
All the clusters have majority customers as females who have done a few years of schooling with most of them above 45 years of age with cluster 2 being most loyal to a brand with least amount of brand runs and buying in bulk at once buying any popular brand either buying health or beauty related products.

When we consider both basis of purchase (BOP) and purchase behavior (PB) the best segmentation was given by k means with 6 clusters:
Cluster 1, 3 belongs to SEC_2 and Cluster 4,6 majority belongs to SEC_4 and cluster 2 to SEC_3. 
Most of these people in the cluster belong to EDU_4 or EDU_5 i.e. they have completed or have done some years of school and majority are females. We find that cluster 6 is the most loyal. Most of the people bought the products when there was no promotion but in cluster 1 and 3 bought when there was promotion 6.  Still we find that these people bought popular soap of any brand. The most purchased category was either health or beauty except for most of the people in cluster 6 (69%) bought carbolic products.






