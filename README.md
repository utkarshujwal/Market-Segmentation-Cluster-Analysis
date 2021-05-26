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


 
 
