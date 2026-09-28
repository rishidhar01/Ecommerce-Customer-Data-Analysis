# **📊 Customer Shopping Behavior Analysis | SQL • Python • PostgreSQL • Power BI** 

An end-to-end **Customer Shopping Behavior Analytics project** that uses Python, Pandas, NumPy, PostgreSQL, SQL, and Microsoft Power BI to analyze 3,900 customer transactions and transform raw shopping data into meaningful business insights.

The project follows a complete data analytics workflow — from data exploration and cleaning to database integration, SQL-based business analysis, interactive Power BI visualization, and business recommendations.

Understanding customer shopping behavior is important for businesses because customer purchasing patterns can influence marketing strategies, product positioning, subscription programs, discounts, and customer retention.

This project analyzes a customer shopping dataset containing **3,900 records and 18 attributes** to understand how customers purchase products, how much revenue different customer groups contribute, which products perform well, how discounts influence purchases, and how subscription status relates to customer behavior.

The project was designed as a practical end-to-end analytics workflow:

**Raw Dataset → Python/Pandas → Data Cleaning → Feature Engineering → PostgreSQL → SQL Analysis → Power BI → Business Insights**

The main goal was not only to analyze the data but also to communicate the results through an interactive dashboard that can be easily understood from a business perspective.

# Business Problem

Businesses collect large amounts of customer transaction data, but raw data alone does not provide useful business value.

The key challenge is to convert transactional data into information that can help answer questions such as:

- Which customer groups contribute the most revenue?
- What products and categories perform well?
- Do subscribers behave differently from non-subscribers?
- How does customer age relate to revenue?
- Which products depend heavily on discounts?
- What payment methods are commonly used?
- Which customers can be classified as new, returning, or loyal?
- Does repeat purchasing behavior relate to subscription adoption?
- Which products receive the highest customer ratings?
- How can businesses use these insights for targeted marketing?

This project addresses these questions using Python, PostgreSQL, SQL, and Power BI.

# Project Objectives

The main objectives of the project are:

1. Explore and understand the customer shopping dataset.
2. Clean and preprocess the raw data using Python.
3. Handle missing values and improve data consistency.
4. Create additional analytical features.
5. Store the cleaned dataset in PostgreSQL.
6. Use SQL to answer business-oriented questions.
7. Segment customers based on purchasing behavior.
8. Analyze revenue across customer groups and age groups.
9. Analyze product, category, discount, shipping, and subscription behavior.
10. Build an interactive Power BI dashboard.
11. Present the findings through clear visualizations.
12. Generate business recommendations based on the analysis.

#Dataset

The project uses a customer shopping behavior dataset containing:

- **3,900 customer transaction records**
- **18 columns**
- Customer demographic information
- Product information
- Purchase information
- Shopping behavior
- Subscription information
- Review ratings
- Shipping preferences

### Dataset Categories

### Customer Information

- Customer ID
- Age
- Gender
- Location
- Subscription Status

### Product & Purchase Information

- Item Purchased
- Category
- Purchase Amount
- Season
- Size
- Color

### Customer Shopping Behavior

- Discount Applied
- Promo Code Used
- Previous Purchases
- Frequency of Purchases
- Review Rating
- Shipping Type
- Payment Method

The dataset contained **37 missing values in the Review Rating column**, which were handled during preprocessing.


# python Data Preparation

Python was used as the first stage of the analytics workflow.

The data was loaded into a Pandas DataFrame and explored to understand its structure, data types, statistical characteristics, and missing values.

### Main Python Activities

- Imported the CSV dataset using Pandas
- Examined dataset structure
- Used `df.info()` for structural analysis
- Used `df.describe()` for statistical summaries
- Checked for missing values
- Cleaned column names
- Handled missing review ratings
- Checked data consistency
- Created analytical features
- Prepared the dataset for PostgreSQL
- Connected the cleaned DataFrame to PostgreSQL


# Data Cleaning

Data cleaning was an important part of the project because reliable analysis depends on consistent and complete data.

The dataset contained **37 missing Review Rating values**.

Instead of removing these records, the missing ratings were handled using the **median review rating of the corresponding product category**.

This helped preserve the available customer transaction records while providing a reasonable value for further analysis.

Other preprocessing activities included standardizing column names and checking relationships between related fields.


#Feature Engineering

Additional features were created to make the dataset more useful for business analysis.

### Age Group

Customer ages were grouped into meaningful categories to analyze purchasing behavior and revenue contribution across different demographic segments.

### Purchase Frequency Days

The purchase frequency information was converted into a numerical representation that could be used for analysis.

Feature engineering helped transform raw customer information into more useful analytical variables.

# PostgreSQL Integration

After data cleaning and feature engineering, the processed customer dataset was loaded into **PostgreSQL**.

PostgreSQL was used as the structured database layer for the project.

        ↓
PostgreSQL
        ↓
SQL Business Analysis
        ↓
Power BI
