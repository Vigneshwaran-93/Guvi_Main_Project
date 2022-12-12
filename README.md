## Project Title: **E-Commerce Customer Segmentation**

# **Business Problem Statement:**

As an e-commerce platform, it is very important to profile your customers, dividing your clientele base into groups based on their needs and expectations. Grouping will help us come up with dedicated marketing strategies and will aid us in recommending products to different user bases. In this project, we are interested in analysing the content of an E-commerce database that lists purchases made by 4000 customers over a period of one year (1/12/2010 to 9/12/2011). Based on this analysis, we would like to develop models to group the 4000 customers into different buckets.
Such a model must take into account the similarity between the products purchased between the users (i.e. a user might purchase 2 different products which are very similar to each other), the spending patterns of a user, their meta information, etc.

# **Data:**

 **The Given Data had the following information's.**

1. **Invoice No – Invoice Number**
2. **Stock Code – Product Stock Code**
3. **Description – Product Description**
4. **Quantity – Product Purchased Quantity**
5. **Invoice Date – Invoice Date**
6. **Unit Price – Product Unit Price**
7. **Customer ID – Customer ID**
8. **Country – Customer Country**

# **Data Interpolation:**

By interpolating the given data, we can use most of the features and build Machine learning models to segment customers and find other key points which would help the business owner to decide the product recommendations and promotional offers.

# **Machine Learning Problem Statement:**

From the given data we come up with a Machine Learning model to Segment the Users and also perform data analytics to help the business owner to better serve the customers.

# **My Approach:**

By analyzing the data I found 24% null values in the Customer Id column. So in order to maintain the integrity of the data I have taken an approach where I have separated the Description from the original dataframe and carried out the NLP process. Following this I have build a model to classify this unique Description into groups.

Then I used pandas to filter each user's full transactions. I formed a matrix having each row as user id, and columns as product group Id's and then I added the cumulative products purchased by the customer to their respective groups. The same way I have added a column " Total\_expence" made by each user. Then again, I have done grouping of users by the matrix formed above.
