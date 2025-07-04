### DSA-Capstone-Project


Hello there, I am Oghenetejiri Ede Favour 👋

I am a passionate and highly analytical and insight-focused with a strong focus on transforming raw data into actionable insights and compelling narratives. I thrive on leveraging data to solve real-world business problems, optimize processes, and support strategic decision-making.

With hands-on experience in data modeling, dashboard development, and statistical analysis, I specialize in turning complex datasets into clear visual stories that empower stakeholders. I am proficient in tools such as SQL, Power BI, and Excel and have a keen understanding of data warehousing and ETL processes.

### 📊 My Data Analytics Portfolio
Here are some of my recent data analysis case studies:

📁 Case Study 1: Amazon Product Review Analysis
Description: An in-depth analysis of Amazon product and customer review data to uncover insights for product improvement, marketing strategies, and customer engagement. Features a comprehensive Excel dashboard.The goal is to extract key insights from product details such as prices, ratings, reviews, and discounts to help stakeholders understand performance by category and at the product level


## 1. Data Set Description

The dataset contains information about products listed on Amazon Dataset that scraped from Amazon product page, with columns such as: 
• Product ID 
• Product Name 
• Category 
• Actual Price 
• Discounted Price 
• Discount % 
• Rating 
• Rating Count 



#### 🧩 Step 1: Data Cleaning

Performed initial data preparation to ensure consistency and reliability:


✅ Removed Duplicates
Used Product ID as a unique identifier.


Removed duplicates using Excel’s Remove Duplicates function.

✅ Handled Missing & Error Values
Replaced blank or incorrect ratings with the average rating.


Filled missing values in rating_count, discount_price, and actual_price.


✅ Removed Special Characters
Cleaned actual_price and discount_price by removing commas and pipe (|) symbols.


✅ Text-to-Columns
Used Excel’s Text to Columns to split combined values (e.g., categories separated by & or other delimiters).



#### ⚙️ Step 2: Feature Engineering


Created custom calculated columns to enable deeper insights:


Rating Bucket
=IF(Rating<3,"Low",IF(Rating<4,"Medium","High"))


Discount Value
=Actual Price - Discounted Price


Review Impact Score
=Rating × Rating Count


Price Range Bucket
=IF(ActualPrice<200,"<₹200",IF(ActualPrice<=500,"₹200–₹500",">₹500"))


High Discount Flag
=IF(Discount%>=50,"Yes","No")



#### 📊 Step 3: Key Metrics (Dashboard Cards)


Calculated using Excel formulas for quick KPI visibility:


Metric	Formula

Total Products	=COUNTA(ProductID)

Average Rating	=AVERAGE(Rating)

Total Reviews	=SUM(Rating Count)

Average Discount (%)	=AVERAGE(Discount%)

Top Rating	=MAX(Rating)



#### ❓ Step 4: Business Questions & Pivot Analysis


Answered 14 business questions using Pivot Tables and custom calculations:

Question	Method	Output


Avg discount % by category	Pivot Table	Category vs Avg Discount

Product count per category	Pivot Table	Bar Chart

Total reviews per category	Pivot Table	Column Chart

Highest average rated products	Pivot + Sorting	Table

Avg actual vs discounted price	Pivot Table	Clustered Column Chart

Most reviewed products	Pivot + Sorting	Table

Products with ≥50% discount	Formula / Filter	Metric

Rating distribution	Pivot (Rating Bucket)	Pie/Bar Chart

Potential revenue (Actual × Count)	Calculated Field	Column Chart

Products per price range	Pivot Table	Stacked Column

Rating vs Discount trend	Scatter Plot	Correlation Chart

Products with <1,000 reviews	Filter	Table

Categories with highest discounts	Pivot Table	Bar Chart

Top 5 by Review Impact Score	Pivot + Sorting	Table



#### 📈 Step 5: Dashboard Creation


Built an interactive Excel dashboard with the following components:



🔹 Key Metrics Cards:

Total Products

Avg Rating

Total Reviews

Avg Discount %

Top Rating



🔹 Category-Level Insigh


Products by Category

Avg Discount % by Category

Total Reviews per Category

Avg Actual vs Discounted Price



🔹 Product-Level Insights:


Top Rated Products

Most Reviewed Products

Top 5 Products by Review Impact Score



🔹 Distribution Insights:



Rating Bucket Distribution

Price Range Buckets

Rating vs Discount Correlation



#### 🧰 Tools Used



Microsoft Excel (Desktop & Mobile)

Pivot Tables

Charts (Column, Bar, Pie, Scatter)

Excel Formulas: IF, COUNTIF, AVERAGE, SUM, TEXTBEFORE, etc.




#### 🔍 Key Insights



High Discounts Drive Visibility

20%+ of products offer ≥50% discount – indicating price strategy.

Positive Customer Sentiment

Most products fall in the 4.0–5.0 rating range.

Electronics Dominate Listings

Mobile & computer-related accessories make up a significant chunk.

Uneven Review Distribution

A few products generate the majority of user reviews.

Top-Performing Products Are Rare

Very few products have both high ratings and high review counts.




#### ✅ Recommendations




Promote High-Rated Products

Prioritize visibility for items with ratings ≥4.5 and high review volumes.

Leverage 50% Discount Band

Consider promotional campaigns around this effective pricing point.

Boost Engagement for Low-Review Products

Incentivize reviews to increase credibility for new or overlooked products.

Optimize Price Tier Strategy

Focus offers in the ₹200–₹500 range where product volume is highest.




#### Category-Level Focus




Prioritize optimization in high-performing categories like Electronics.

#### 📂 Files Included



📁 /Amazon-Product-Analysis/
├── 📄 Amazon case study.xlsx (Cleaned dataset)
├── 📄 Amazon Dashboard.xlsx (Interactive dashboard)
├── 📄 Pivot Tables Reference Guide.xlsx
├── 📄 README.md (This file)




#### 🚀 About





This project was completed as part of a Data Analysis portfolio while taking a class with The Incubator Hub. It demonstrates the ability to clean, analyze, and visualize business data using Microsoft Excel.

