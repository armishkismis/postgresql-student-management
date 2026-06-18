# PostgreSQL Student Management System
# Health Insurance Analysis using PostgreSQL

## Project Overview

This project analyzes a health insurance dataset using PostgreSQL.

The objective is to understand customer demographics, premium patterns, customer interest in insurance products, and risk-related factors.

## Dataset

Source: Kaggle - Health Insurance Cross Sell Prediction

Main fields:

- Age
- Gender
- Annual Premium
- Vehicle Age
- Vehicle Damage
- Previously Insured
- Response

## Tools Used

- pgAdmin
- Kaggle Dataset

## Business Questions

### 1. How many customers are present in the dataset?

```sql
SELECT COUNT(*)
FROM health_insurance;
```

### 2. What is the average annual premium?

```sql
SELECT AVG(annual_premium)
FROM health_insurance;
```

### 3. Which age groups pay higher premiums?

```sql
SELECT age,
AVG(annual_premium)
FROM health_insurance
GROUP BY age;
```

### 4. How many customers are interested in purchasing insurance?

```sql
SELECT COUNT(*)
FROM health_insurance
WHERE response = 1;
```

## Key Findings

- Premium generally increases with age.
- Customers with vehicle damage tend to have higher insurance interest.
- Previously insured customers show different purchasing behavior.
- Risk factors influence premium patterns.

## Skills Demonstrated

- SQL Queries
- Data Analysis
- Aggregations
- Filtering
- Business Insights
- PostgreSQL
