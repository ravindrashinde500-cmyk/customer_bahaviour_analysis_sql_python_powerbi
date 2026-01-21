## 🧾 Customer Behaviour Analysis Portfolio Project

      This project provides actionable insights into customer shopping behaviour by analysing transactional data from 3,900 purchases across multiple product categories, utilising tools like SQL, Python, and Power BI.

---

## 📌Table of Contents
- <a href="#overview">Overview</a>
- <a href="#business-problem">Business Problem</a>
- <a href="#dataset">Dataset</a>
- <a href="#tools--technologies">Tools & Technologies</a>
- <a href="#project-structure">Project Structure</a>
- <a href="#data-cleaning--preparation">Data Cleaning & Preparation</a>
- <a href="#exploratory-data-analysis-(EDA)">Exploratory Data Analysis (EDA)</a>
- <a href="#dashboard">Dashboard</a>
- <a href="#how-to-run-this-project">How to Run This Project</a>
- <a href="#key-insights">Key Insights</a>
- <a href="#conclusion">Conclusion</a>
- <a href="#future-work--recommendation">Future work & Recommendation</a>
- <a href="#author--contact">Author & Contact</a>

---

<h2><a class="anchor" id="overview"></a>Overview</h2>

- The objective of this project is to simulate a corporate-grade, end-to-end data analytics workflow, showcasing the ability to convert raw data into actionable business intelligence. The project demonstrates the complete analytics lifecycle through the following stages:

- ✅Data Preparation, Modeling & Exploratory Data Analysis (Python)
Cleaned, transformed, and explored raw datasets to ensure data quality and uncover initial patterns and relationships.

- ✅Data Analysis & Business Querying (SQL)
Simulated real-world business transactions and executed analytical SQL queries to derive insights on customer segmentation, loyalty behavior, and key purchase drivers.

- ✅Data Visualization & Insight Generation (Power BI)
Designed an interactive dashboard highlighting critical trends, KPIs, and customer insights to support data-driven decision-making for stakeholders.

- ✅Reporting & Presentation
Developed a structured analytical report summarizing findings and business recommendations, along with a presentation that visually communicates insights and actionable strategies to stakeholders.

---

<h2><a class="anchor" id="business-problem"></a>Business Problem</h2>

- A leading retail company aims to gain deeper insights into customer shopping behavior to improve sales performance, enhance customer satisfaction, and strengthen long-term loyalty.

- Management has observed shifting purchasing patterns across different demographics, product categories, and sales channels (online and offline). They are particularly interested in identifying the key factors such as discounts, customer reviews, seasonal trends, and payment preferences that influence purchasing decisions and repeat behavior.
purchases.

- This project demonstrates a complete, industry-standard end-to-end data analytics workflow, reflecting the real-world responsibilities of data analysts. It covers all key stages, from data preparation and modeling to insight generation, visualization, and reporting.

---

- GitHub Repository Image:
![Project Workflow](https://github.com/user-attachments/assets/8bbd5dc9-eb6c-40c1-8f19-c08b4107f654)

---

<h2><a class="anchor" id="dataset"></a>Dataset</h2>


- CSV file is located in /data/ folder.

- **The database consists of** : Customer details like age, customer id, item purchased, discount, location, shipping type etc.

- This dataset primarily contains information about customer details and the records of various items purchased by them.

- These customer shopping behavioural details which are organised into multiple tables that are interlinked through keys, including primary keys and foreign keys.

---

<h2><a class="anchor" id="tools--technologies"></a>Tools & Technologies</h2>
  
  - SQL (Common Table Expressions, Joins, Filtering)
  - Python (Pandas, Matplotlib, Seaborn)
  - Power BI (Interactive Visualisations)
  - GitHub

---

<h2><a class="anchor" id="project-structure"></a>Project Structure</h2>

```
customer-behaviour-analysis/
│
├── README.md
├── .gitignore
├── requirements.txt
├── customer shopping bahaviour Report.pdf
│
├── notebooks/                  # Jupyter notebooks
│   ├── exploratory_data_analysis(EDA).ipynb
│   
├── scripts/                    # Python scripts for ingestion and processing
│   ├── business_problem_statement.pdf
│   ├── sql_query_q&a.md
│
├── dashboard/                  # Power BI dashboard file
│   └── customer_behaviour_dashboard.pbix


```

<h2><a class="anchor" id="data-cleaning--preparation"></a>Data Cleaning & Preparation</h2>

- **Missing Data Handling** : Identified missing values and filled the Review Rating  column using the median rating of the corresponding product category.

- **Column Standardization**: Renamed columns to snake case for better readability and documentation.

- **Columns creation** :
  - Created age_group column by binning customer ages.
  - Created purchase_frequency_days column from purchase data.

- **Data Consistency Check** : Verified if discount_applied and promo_code_used
were redundant; dropped promo_code_used.

- **Database Integration** : Connected Python script to MySQL and loaded the cleaned DataFrame into the database for SQL analysis.

---

<h2><a class="anchor" id="exploratory-data-analysis-(EDA)"></a>Exploratory Data Analysis (EDA)</h2>

- Exploratory Data Analysis was conducted to understand customer shopping behavior, assess data quality, and identify key patterns driving sales and customer loyalty.

- Reviewed dataset structure, data types, missing values, and duplicates
imputed missing Review Rating values using the median rating by product category

- Analyzed distributions of purchase amounts, product categories, payment methods, and sales channels

- Examined relationships between discounts, review ratings, sales channels, and repeat purchases

- Identified seasonal trends and category-wise performance variations


- **Key Insights**
  - Discounts significantly influence purchase frequency
  - Higher product ratings are associated with increased repeat purchases
  - Online sales show higher average order value than offline
  - Seasonal trends strongly impact category performance
  - EDA insights guided subsequent SQL analysis and Power BI dashboard design.

- Insights from EDA were used to guide SQL analysis and dashboard design.

---

<h2><a class="anchor" id="dashboard"></a>Dashboard</h2>

- The Power BI dashboard provides insights into customer behavior, sales performance, and purchase drivers to support data-driven decisions.

### Objective:
```
To enable data-driven decision-making by visualizing customer trends, purchase drivers, and channel performance, supporting improvements in marketing strategy, customer engagement, and product optimization.
```
- **Key Metrics** : Total Sales, Average Order Value, Purchase Frequency, Repeat Customers, Discounts, Online vs Offline Sales

- **Interactivity** : Filter by date, product category, sales channel, and customer segment

- **Business Impact** : Helps optimize marketing strategies, improve customer engagement, and guide product decisions

---

<h2><a class="anchor" id="how-to-run-this-project"></a>🛠️ How to Run This Project</h2>

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/customer-shopping-behaviour-analysis.git
```

2. **Open Customer_Shopping_Behaviour_Analysis.ipynb notebook**
```
- This file contains:
  - Data Import
  - Data exploration
  - Data cleaning
  - Connection to SQL Database
  ```
3. **Load the data from Python notebook into MySQL/PostgreSQL Server**
```
- Create a database in SQL
- Run Python code to load data into SQL database
- Open -> customer_behaviour_sql_queries.sql
- Answer Business Questions using SQL Queries 
```
4. **Connect the SQL Database to Power BI**
```
- Open -> customer_behaviour_dashboard.pbix
- Create interactive dashboard in Power BI
  ```
5. **Open Power BI Dashboard**
```
- dashboard/customer_behaviour_dashboard.pbix
```
-  Open Power BI Dashboard: 

---

<h2><a class="anchor" id="key-insights"></a>Key Insights</h2> 

- Discounts significantly increase purchase frequency and customer engagement

- Highly rated products show stronger repeat purchase behavior

- Online sales channels generate higher average order value

- Seasonal trends strongly influence category-level sales performance

---

<h2><a class="anchor" id="conclusion"></a>Conclusion</h2>

- This project demonstrates an end-to-end retail data analytics workflow, transforming raw consumer data into actionable business insights. 

- The analysis highlights the impact of discounts, ratings, sales channels, and seasonality on customer behavior and repeat purchases. 

- These insights support data-driven decisions to optimize marketing, customer engagement, and product strategies.

---

<h2><a class="anchor" id="future-work--recommendation"></a>Future work & Recommendation</h2>

- **Boost Subscriptions** – Promote exclusive benefits for subscribers.

- **Customer Loyalty Programs** – Reward repeat buyers to move them into the “Loyal”
segment.

- **Review Discount Policy** – Balance sales boosts with margin control.

- **Product Positioning** – Highlight top-rated and best-selling products in campaigns.

- **Targeted Marketing** – Focus efforts on high-revenue age groups and express-shipping
users.

---

<h2><a class="anchor" id="author--contact"></a>Author & Contact</h2>

- Ravindra Shinde 
- Data Analyst
- 📧 Email: ravindra.shinde500@gmail.com
- 🔗[linkedin](https://www.linkedin.com/in/ravindrashinde0815/)
