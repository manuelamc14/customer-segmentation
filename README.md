# customer-segmentation

### 1. Problem Statement and Motivation:

The primary goal of this project is to perform customer segmentation on a data set that includes 2,240 rows representing unique customers. Identify the main characteristics of customers to design new strategies that boost the company's sales.

The motivation to work on this project is the challenges the data involves as:

- Inaccurate or messy customer data
- Feature Engineering
- Unsupervised learning methods exploration

###  2. Description of Data:

**2.1 Data Source:**

Customer Personality Analysis. The data set was obtained in Kaggle (https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis). There are 2240 observations with 29 variables.

**2.2 Data Understanding:**

The 29 columns of data are classified into five domains. The five categories in the domain
include Customer, Demographic, Product, Promotion and Place.

- Customer: The customer information includes a unique customer ID that identifies the
2240 unique customers in the sample. Also, the date of the customer’s enrollment with
the company (Dt_Customer), the number of the days since the last purchase (Recency)
and the information if the customer has complained in the last two years (Complain)
- Demographic: Customer demographic information includes year of birth, level of
education, marital status, income, and number of children and teenagers living at home.
- Products: The amount spent on products like wines, fruits, meat, fish, sweets and gold.
- Promotion: Includes the number of purchases made with a discount, and information about the customer decision regarding the last five campaigns.
- Place: The number of purchases made by the customer in the web, catalog and store. It also includes information about the number of visits to the company’s website in the last month.
    

### 3. Methodology

**3.1 Clusters number determination**

To perform unsupervised partition learning,  Kmeans() was selected as base model to decide the most convenient number of groups and the best algorithm for the data. Two main methods for determining the number of clusters were used: the elbow method and the silhouette score.

**3.2 Algorithm Selection**

Four algorithms to test which would provide the best result were selected. KMeans(), KMedoids(), KModes() and Fanny().

### 4. Results and Analysis

The final model obtained is based on Kmeans( ). After clustering the customers, three main groups similarly distributed were identified. The main characteristics of each group are:

- Demographics: Education, Marital Status, Dependents, Age
- Income
- Products
- Shipping Method
- Promotion Response

### 5. Conclusions, Recommendations, and Future Search

The project was considered successful after three large customer groups and the similarities and differentiators between them were identified.

The first group of clients (Cluster 0) is made up of people, mostly with postgraduate studies. With an average income of $56,906.56 and an average expense of $715.63, this group ranks second in the ranking of customers who spend the most. Most of the purchases are related to wines and meat products. Also, compared to the other two cluster groups, this group made the most commercial purchases.

The second group (Cluster 1) is the largest group of clients. This group has the lowest average income ($34,353.62) and the lowest average expense ($80.20) among the groups. Unexpectedly, the response of this group to offers and promotions is poor.

The last group (Cluster 2) has the highest average income ($76,633.81) and average spending ($1,403.23). Clients in this group are characterized by having a postgraduate degree. Most have no dependents, and the average age is 53 years. This cluster contains a smaller number of customers, who mainly consume wine and food products. The response of this group to the campaigns and agreements was not overwhelming.

The average spending of the groups was mainly influenced by the average income. However, variables such as marital status, age, and purchase method had no impact on the total amount spent by customers.

After this study, the main recommendation to the company is to define the objective of the strategies that it would like to implement, for example, reduce the abandonment rate, increase sales of a specific group of products, attract more customers, define what type of customers contribute more to revenue, etc. Based on this decision, the company could use the results of the consumer segmentation study to design the best approach for its objective. It is important to mention that to guarantee the success of such strategies, future research will be necessary to identify more specific patterns in customer behavior and to explain the reasons behind customer behavior. For example, why the acceptance rate of the promotion is low, or why the customer prefers to buy meat instead of fish. In this way, the strategies could be more oriented to specific objectives instead of generalized plans.
