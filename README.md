# Customer_Shopping_Behaviour
This is my overall data analytics project from scratch

# 🛒 Customer Shopping Behavior Analysis
### End-to-End Data Analytics Project | Python • PostgreSQL • SQL • Power BI

# 📖 Project Overview

Customer behavior analysis is one of the most important applications of data analytics in the retail industry. Businesses use customer purchasing data to understand buying patterns, identify valuable customers, optimize marketing campaigns, and improve overall sales performance.

This project demonstrates a **complete end-to-end Data Analytics workflow** starting from raw Excel data, performing data cleaning and exploratory analysis in Python, storing the cleaned data in PostgreSQL, analyzing business problems using SQL, creating an interactive Power BI dashboard, and documenting the project for GitHub portfolio presentation.

The project simulates a real-world business case that a Data Analyst might solve in a retail company.

---

# 🎯 Business Problem Statement

A retail company wants to understand customer shopping behavior to improve customer engagement, increase revenue, and optimize marketing strategies.

The company wants answers to questions such as:

- Which customers generate the highest revenue?
- Which product categories perform the best?
- Which age group contributes the most sales?
- Do subscribers spend more than non-subscribers?
- Does discounting increase sales?
- Which shipping methods are preferred?
- Which customers are likely to become loyal customers?

The objective is to transform raw customer data into meaningful business insights that support strategic decision-making.

---

# 📊 Dataset Overview

The dataset contains customer shopping records including:

- Customer ID
- Age
- Gender
- Item Purchased
- Category
- Purchase Amount (USD)
- Location
- Size
- Color
- Season
- Review Rating
- Subscription Status
- Shipping Type
- Discount Applied
- Promo Code Used
- Previous Purchases
- Payment Method
- Purchase Frequency

**Dataset Type:** Retail Customer Shopping Data

---

# 🛠 Technology Stack

| Tool | Purpose |
|------|----------|
| Python | Data Cleaning & Analysis |
| Pandas | Data Manipulation |
| PostgreSQL | Database Management |
| SQLAlchemy | Database Connection |
| Psycopg2 | PostgreSQL Driver |
| SQL | Business Analysis |
| Power BI | Dashboard Development |
| Git | Version Control |
| GitHub | Project Portfolio |

---

# 📂 Project Structure

```
Customer-Shopping-Behavior/
│
├── Dataset/
│   └── customer_shopping_behavior.csv.xlsx
│
├── Python/
│   └── customer_shopping_behaviour.ipynb
│
├── SQL/
│   └── business_queries.sql
│
├── Dashboard/
│   ├── Customer_Behavior.pbix
│   └── dashboard.png
│
├── Report/
│   └── Project_Report.pdf
│
├── Presentation/
│   └── Customer_Behavior_Presentation.pptx
│
├── Images/
│   ├── workflow.png
│   └── dataset.png
│
└── README.md
```

---

# 🚀 End-to-End Project Workflow

```
Business Problem
        │
        ▼
Dataset Understanding
        │
        ▼
Python Data Cleaning & EDA
        │
        ▼
Feature Engineering
        │
        ▼
PostgreSQL Database
        │
        ▼
SQL Business Analysis
        │
        ▼
Power BI Dashboard
        │
        ▼
Project Report
        │
        ▼
Presentation Deck
        │
        ▼
GitHub Repository
```

---

# 📋 Project Stages

| Stage | Description | Status |
|--------|-------------|:------:|
| Business Problem Statement | Define business objectives | ✅ |
| Dataset Overview | Understand available data | ✅ |
| Python (EDA & Cleaning) | Data preprocessing | ✅ |
| PostgreSQL Integration | Store cleaned dataset | ✅ |
| SQL Business Analysis | Solve business questions | ⏳ |
| Power BI Dashboard | Interactive dashboard | ⏳ |
| Project Report | Documentation | ⏳ |
| Presentation Deck | Business presentation | ⏳ |
| GitHub Repository | Portfolio Project | ✅ |
| LinkedIn Showcase | Professional Networking | ⏳ |

---

# 🐍 Python Data Cleaning & Exploratory Data Analysis

The dataset was analyzed and cleaned using **Python** and **Pandas**.

### Tasks Performed

- Imported dataset
- Checked dataset structure
- Examined data types
- Generated summary statistics
- Detected missing values
- Filled missing Review Ratings using Category-wise Median
- Standardized column names
- Renamed columns
- Removed redundant columns
- Created new features
- Prepared dataset for SQL analysis

---

# 🧹 Data Cleaning

### Missing Value Handling

Missing values in the **Review Rating** column were replaced using the **median rating within each product category**, ensuring a more realistic imputation than using the overall median.

---

### Column Standardization

Column names were converted into **snake_case** for better compatibility with Python and SQL.

Example

```
Purchase Amount (USD)
```

↓

```
purchase_amount
```

---

### Removed Redundant Data

The following redundant column was removed

```
promo_code_used
```

because it contained duplicate information already represented by

```
discount_applied
```

---

# ⚡ Feature Engineering

Two additional features were created.

### Age Group

Customers were grouped into

- Young Adult
- Adult
- Middle-aged
- Senior

using **pd.qcut()**.

---

### Purchase Frequency (Days)

Purchase frequencies were converted into numerical values.

| Frequency | Days |
|-----------|-----:|
| Weekly | 7 |
| Fortnightly | 14 |
| Monthly | 30 |
| Quarterly | 90 |
| Annually | 365 |

---

# 🗄 PostgreSQL Integration

The cleaned dataset was successfully loaded into PostgreSQL using SQLAlchemy.

**Database**

```
customer_behavior
```

**Table**

```
customer
```

This enables efficient querying and business analysis using SQL.

---

# 📈 SQL Business Analysis

The following business questions are answered using SQL:

- Revenue generated by Gender
- Average Purchase Amount
- Top Rated Products
- Revenue by Category
- Revenue by Age Group
- Subscription Analysis
- Discount Analysis
- Customer Segmentation
- Shipping Method Analysis
- Repeat Customer Analysis
- Purchase Frequency Analysis

---

# 📊 Power BI Dashboard

The dashboard provides interactive business insights through:

### KPI Cards

- Total Customers
- Total Revenue
- Average Purchase Amount
- Average Review Rating

### Charts

- Revenue by Category
- Sales by Category
- Revenue by Age Group
- Subscription Analysis
- Customer Distribution

### Interactive Filters

- Gender
- Category
- Shipping Type
- Subscription Status

---

# 📝 Project Report

A professional project report documents:

- Business Problem
- Dataset Description
- Data Cleaning Process
- Feature Engineering
- SQL Analysis
- Dashboard Insights
- Business Recommendations

---

# 📽 Presentation Deck

A concise presentation summarizes:

- Project Overview
- Business Problem
- Methodology
- Dashboard Screenshots
- Key Insights
- Business Recommendations
- Future Scope

---

# 💻 GitHub Repository

The project is maintained on GitHub with:

- Complete Source Code
- Dataset
- SQL Scripts
- Dashboard
- Documentation
- Project Report
- Presentation

---


# 📦 Required Libraries

Install dependencies

```bash
pip install pandas
pip install sqlalchemy
pip install psycopg2-binary
```

---

# ▶️ How to Run

Clone the repository

```bash
git clone https://github.com/your-username/customer-shopping-behavior-analysis.git
```

Move into the project folder

```bash
cd customer-shopping-behavior-analysis
```

Install required libraries

```bash
pip install pandas sqlalchemy psycopg2-binary
```

Open Jupyter Notebook

```bash
jupyter notebook
```

Run

```
customer_shopping_behaviour.ipynb
```

Configure PostgreSQL credentials before loading the data.

---

# 📈 Project Outcomes

This project demonstrates:

- ✅ Data Cleaning
- ✅ Exploratory Data Analysis
- ✅ Feature Engineering
- ✅ Database Integration
- ✅ SQL Analysis
- ✅ Business Intelligence
- ✅ Dashboard Development
- ✅ GitHub Portfolio Development

---

# 🚀 Future Improvements

- Customer Segmentation using Machine Learning
- Sales Forecasting
- Customer Lifetime Value Prediction
- Recommendation System
- Cloud Database Deployment
- Automated ETL Pipeline

---

# 👨‍💻 Author

**Anshuman Parmar**

B.Tech Chemical Engineering

Birla Institute of Technology, Mesra



---

# ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub.

It motivates me to build more real-world Data Analytics projects.
