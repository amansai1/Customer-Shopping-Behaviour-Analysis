# Customer-Shopping-Behaviour-Analysis
End-to-End Data Analytics &amp; Business Intelligence Project
Project Overview

This project is an end-to-end data analytics and business intelligence solution that analyzes customer shopping behavior using Python, PostgreSQL (Docker), SQL, and Power BI.

The goal of the project is to extract actionable business insights related to customer demographics, purchasing patterns, subscription behavior, discounts, and product performance, and present them through an interactive Power BI dashboard.

This project was designed and implemented as a portfolio project to demonstrate real-world data engineering, SQL analytics, and BI visualization skills.

Author Details

Author: Sai Aman Teppala
Degree: MSc Data Analytics
Project Type: Portfolio Project
Year: 2025

Email: amansaileo@gmail.com

LinkedIn: https://www.linkedin.com/in/saiamanteppala/

# Technology Stack
Layer	Tools Used
Programming	Python_OPCODE (Pandas, NumPy)
Database	PostgreSQL 15 (Docker Container)
SQL IDE	VS Code (SQLTools Extension)
Visualization	Power BI Desktop
Environment	macOS (Host) + Windows 11 ARM (VMware Fusion)
Notebook	Jupyter Notebook
Version Control	Git & GitHub

# End-to-End Data Pipeline
Raw CSV Dataset
      ↓
Python Data Cleaning & Feature Engineering (Jupyter Notebook)
      ↓
PostgreSQL Database (Docker Container)
      ↓
SQL Analysis (VS Code + SQLTools)
      ↓
Power BI Dashboard (Windows VM)

# Dataset Description

The dataset represents customer shopping behavior with attributes such as:

Customer demographics (age, gender, location)

Product information (category, item purchased)

Transaction details (purchase amount, discounts, shipping type)

Behavioral indicators (previous purchases, subscription status)

Feedback metrics (review ratings)

 Note: This is a simulated retail dataset commonly used for analytics and BI practice.

 Data Cleaning & Feature Engineering (Python)

Performed using Jupyter Notebook:

Handled missing values

Standardized categorical values (Yes/No, gender, shipping types)

Converted numeric columns to appropriate data types

Created derived features:

age_group (Young Adult, Adult, Middle-aged, Senior)

Ensured schema consistency for database ingestion

# Database Setup (PostgreSQL + Docker)

PostgreSQL was deployed using Docker:

docker run -d \
  --name postgres \
  -e POSTGRES_USER=admin \
  -e POSTGRES_PASSWORD=admin123 \
  -e POSTGRES_DB=customer_behavior \
  -p 5432:5432 \
  postgres:15


The cleaned dataset was loaded into PostgreSQL using SQLAlchemy + psycopg2.

# SQL Analysis (VS Code)

SQL queries were executed using VS Code + SQLTools extension.

Key Business Questions Answered

Total revenue by gender

High-spending customers who used discounts

Top 5 products by average review rating

Purchase comparison between Standard and Express shipping

Spending behavior of subscribed vs non-subscribed customers

Products with highest discount usage

Customer segmentation (New, Returning, Loyal)

Top products within each category

Subscription likelihood of repeat buyers

Revenue contribution by age group

SQL Techniques Used

GROUP BY, HAVING

Subqueries

CASE statements

Common Table Expressions (CTEs)

Window functions (ROW_NUMBER)

Aggregations and ranking logic

# Power BI Dashboard

Power BI Desktop was installed on Windows 11 ARM via VMware Fusion (macOS host).

Dashboard Features

KPI Cards:

Number of Customers

Average Purchase Amount

Average Review Rating

Visualizations:

Donut chart (Subscription Status)

Bar charts (Revenue & Sales by Category)

Horizontal bar charts (Revenue & Sales by Age Group)

Interactive slicers:

Subscription Status

Gender

Category

Shipping Type

PostgreSQL Connectivity

Connected via PostgreSQL ODBC Driver

Encryption fallback handled during connection

Verified data using Navigator (public.customer table)

Key Business Insights

Subscribed customers generate higher total revenue

Clothing category dominates both revenue and sales volume

Young adults and middle-aged customers contribute the most revenue

Customers using discounts still make high-value purchases

Express and Standard shipping show different spending patterns

Future Enhancements

Automate ETL using Apache Airflow

Deploy PostgreSQL on AWS / Azure

Add predictive analytics (customer churn & LTV)
# Project Structure
```
Customer-Shopping-Behavior-Analysis/
│
├── dataset/
│   └── customer_shopping_data.csv
│
├── notebooks/
│   └── Customer_Shopping_Behavior_Analysis.ipynb
│
├── sql/
│   └── customer_analysis_queries.sql
│
├── powerbi/
│   └── customer_behavior_dashboard.pbix
│
├── report/
│   └── Customer_Shopping_Behavior_Analysis.pdf
│   └── Customer_Shopping_Behavior_Analysis.pptx
│
└── README.md``` 

Implement real-time dashboards

Integrate machine learning models
