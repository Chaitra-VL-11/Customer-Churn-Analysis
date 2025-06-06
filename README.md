# Customer-Churn-Analysis
## Online Retail Customer Segmentation for Targeted Marketing

### Business collect customer data but struggle to use if effectively for marketing.

### 📌 Business Problem:
Businesses often collect large amounts of customer data but struggle to convert it into actionable marketing strategies. A one-size-fits-all approach leads to low engagement and poor conversion. By segmenting customers based on behavior, companies can personalize marketing efforts, improving retention, engagement, and revenue.

### 🎯 Project Goal:
This project focuses on customer segmentation and churn analysis using Python, with the following objectives:

* Segment customers based on their purchasing behavior using RFM Analysis.
* Identify churned customers and develop effective re-engagement strategies.

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
   * Grouped customers based on:
     1) Recency: Days since last purchase
     2) Frequency: Number of unique purchase.
     3) Monetary: Total spend
   * High RFM scores indicate loyal/high-value customers.

5. Customer Churn Analysis
   * Defined churn as customers with no purchase in the last 90 days.
   * Churn Rate: 33.61%
   * Visualized churn distribution to understand customer retention patterns.
   * Insight: 1 in 3 customers are at risk of churning — highlighting the need for proactive retention strategies.
   * If the recency or Invoice date count is high, it means they haven't made a purchase in a long time, which indicates that customer is likely to churn.
  
## When a customer is identified as churned(i.e., they haven't made a purchase in a long time), we should take strategic actions to re-engage them.

### Re-Engagement Strategies:

🎯 Personalized Email & SMS Campaigns
* Offer discounts or product suggestions based on previous purchases
* Use A/B testing to optimize messaging

🎁 Loyalty & Reward Programs
* Offer bonus points, limited-time deals, or a “Win Back” offer

🛒 Personalized Product Recommendations & Upselling
* Showcase new arrivals and trending products aligned with customer interests

### 🛠️ Tech Stack:
* Language: Python (Pandas, NumPy, Matplotlib, Seaborn)
* Analysis: RFM modeling, churn logic
* Output: Cleaned dataset, customer segments, churn insights, actionable marketing strategies

### 💡 Business Impact:
* Enables targeted marketing over mass outreach
* Improves customer retention through timely intervention
* Helps prioritize high-value customers and reduce revenue leakage from churn
