# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping behavior to understand purchasing patterns, customer preferences, and factors that influence sales.

The project follows a complete data analytics workflow — from loading and cleaning the data in Python to analyzing it with SQL in PostgreSQL and presenting insights through a Power BI dashboard.

## Dataset

The dataset contains **3,900 customer records** with information such as:

* Customer age and gender
* Products and categories purchased
* Purchased amount
* Location and season
* Review ratings
* Subscription status
* Shipping type
* Discounts
* Previous purchases
* Payment method
* Purchase frequency

The original dataset contains 18 columns.

## Tools Used

* **Python** – Data loading, cleaning and analysis
* **Pandas** – Data manipulation
* **Matplotlib / Seaborn** – Data visualization
* **PostgreSQL** – SQL analysis and data storage
* **Power BI** – Interactive dashboard and visualization
* **Jupyter Notebook** – Project development

## Project Steps

### 1. Data Loading

The dataset was loaded into Python using Pandas and examined to understand its structure and columns.

### 2. Exploratory Data Analysis

EDA was performed to understand customer demographics, purchasing behavior, product categories, ratings, and other important patterns.

### 3. Data Cleaning

The data was cleaned by:

* Checking missing values
* Filling missing review ratings using category-level median values
* Standardizing column names
* Renaming columns for easier analysis
* Creating age groups
* Converting purchase frequency into number of days
* Removing redundant columns

The dataset initially had 37 missing values in `Review Rating`, which were successfully handled.

### 4. PostgreSQL Analysis

The cleaned dataset was loaded into a PostgreSQL database named `customer_behavior`, with the data stored in the `customer` table.

SQL queries were then used to analyze customer behavior, sales patterns, product performance, and other business questions.

### 5. Power BI Dashboard

The PostgreSQL data was connected to Power BI to create an interactive dashboard.

The dashboard helps explore:

* Sales performance
* Customer segments
* Product categories
* Purchase behavior
* Subscription trends
* Shipping preferences
* Customer demographics

### 6. Report

The final report summarizes the analysis, key findings, and business recommendations in a simple and easy-to-understand format.

## Dashboard

The Power BI dashboard provides an interactive view of customer shopping behavior and allows users to explore the data using filters and visualizations.

## Results

The analysis provides insights into:

* Customer purchasing patterns
* Popular products and categories
* Customer demographics
* Subscription behavior
* Purchase frequency
* Shipping preferences
* Discount usage
* Customer loyalty and repeat purchases

These insights can help businesses improve marketing strategies, customer retention, product positioning, and promotional decisions.

## Business Recommendations

* Promote subscription benefits to increase customer subscriptions.
* Use loyalty programs to encourage repeat purchases.
* Review discount strategies while maintaining healthy margins.
* Promote popular and highly rated products.
* Use customer demographics and purchasing behavior for targeted marketing.

## How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd customer-shopping-analysis
```

### 2. Install Python libraries

```bash
pip install pandas matplotlib seaborn sqlalchemy psycopg2-binary
```

### 3. Run the Jupyter Notebook

Open:

```text
customer_shopping.ipynb
```

Run the cells to load, clean, and analyze the dataset.

### 4. Set up PostgreSQL

Create a PostgreSQL database named:

```text
customer_behavior
```

Update the PostgreSQL connection details in the notebook according to your local setup.

The cleaned data will be loaded into the `customer` table.

### 5. Run SQL Analysis

Open PostgreSQL/pgAdmin and run the SQL queries included in the project.

### 6. Open Power BI

Connect Power BI to:

```text
Server: localhost:5432
Database: customer_behavior
Table: customer
```

Load the data and open the Power BI dashboard.

## Project Structure

```text
customer-shopping-analysis/
│
├── customer_shopping.ipynb
├── customer_shopping_behavior.csv
├── SQL/
│   └── customer_analysis.sql
├── PowerBI/
│   └── customer_behavior_dashboard.pbix
├── Report/
│   └── customer_behavior_report.pdf
└── README.md
```

## Conclusion

This project demonstrates an end-to-end data analytics workflow using Python, SQL, PostgreSQL, and Power BI. It focuses on turning raw customer data into clear insights that can support better business decisions.
