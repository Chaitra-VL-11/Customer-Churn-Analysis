# Customer-Churn-Analysis
## Online Retail Customer Segmentation for Targeted Marketing

### Business collect customer data but struggle to use if effectively for marketing.

By segmenting customers, we can identify patterns and tailor marketing efforts to different groups, increasing engagement and sales. Instead of using one-size-fits-all approach, segmentation allows companies to target specific customer groups with personalized strategies.

### Project Goal:
This project focuses on customer segmentation and churn analysis using python.The goal is to:
1. Segment customer based on their purchasing behavior using RFM analysis.
2. Identify churned customer and develop re-engagement strategies.

### Data Analysis & Modeling steps:

1. Data Cleaning & Perprocessing
   * Removed missing values
   * added most frequent description for stockcode
   * Merging stockcode, freq_description, count columns to the original data.
   * we can't have negative value in the Quantity and Unit Price so we just kept only Unitprice and Quantity which is greater than Zero.
  
2. Feature Engineering: Create New Columns
   * Generated Total Sales Column
   * Generated Month column
     
3. Visualization & EDA
   * Visualize Month-wise Total Sales Distribution
   * Visualize Country-wise Total Sales Distribution
   * Visualize top 5 Countries by percentage contribution to total sales
   * Visualize Product-wise Total price Distribution

4. RFM Analysis
   * Grouped the customer ID based on their recency, frequency, monetary by their purchasing behavior.
   * If the RFM_score is high those customers are considered as loyal customers.

5. Customer Churn Analysis
   * If the recency or Invoice date count is high, it means they haven't made a purchase in a long time, which indicates that customer is likely to churn.
   * Visualize Customer Churn Distribution.
   * we considered 90 days threshold value for each customer, if their purchase history is more than 90 days considered as churned customers.
   * Churn Rate is 33.61%.
  
## When a customer is identified as churned(i.e., they haven't made a purchase in a long time), we should take strategic actions to re-engage them.

### Re-Engagement Strategies:

1. Personalized Email & SMS Campaigns: send a email with a special discount or personalized product recommendations. Use A/B testing to see which messages work best.
   
3. Loyalty & Reward Programs: offer bouns points or exclusive deals for returning customers. Introduce a "Win Back" offer for lapsed customers.
4. Personalized Recommendations & Upselling: Highlight new arrivals or trending items related to their interests.
