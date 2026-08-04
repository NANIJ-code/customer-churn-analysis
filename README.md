# Telco Customer Churn Analysis

## Project Overview

Customer churn is one of the main challenges for telecommunication companies because losing existing customers is usually more expensive than keeping them. This project analyzes the Telco Customer Churn dataset to identify the main factors that influence customer attrition and to provide business recommendations that can help reduce churn.

The analysis focuses on understanding customer behavior by comparing customers who stayed with those who left the company. Instead of building a machine learning model, this project uses Exploratory Data Analysis (EDA) to discover patterns, trends, and possible reasons behind customer churn.

---

## Dataset

The dataset contains information about customers of a telecommunications company, including:

- Customer contract type
- Customer tenure
- Monthly charges
- Total charges
- Churn status

The target variable is **Churn**, which indicates whether a customer left the company.

---

## Project Workflow

The project follows a simple data analysis process.

### Data Loading

The dataset is imported using **Pandas**. This library is used because it provides easy tools for reading, organizing, filtering, and manipulating tabular data.

---

### Data Exploration

Before starting the analysis, the dataset is explored to understand its structure.

This step includes:

- Displaying the first rows of the dataset
- Checking missing values
- Generating descriptive statistics

The objective is to understand the available information and identify potential data quality issues before performing any analysis.

---

### Data Cleaning

The dataset contains incorrect values in the **TotalCharges** column because some values are stored as text.

During this step:

- The column is converted into numeric values.
- Invalid values are replaced with missing values.
- Missing values are filled using the median.

The median is chosen because it is less affected by extreme values than the mean, making it a more reliable replacement for missing numerical data.

---

### Churn Distribution Analysis

The first analysis measures the proportion of customers who stayed and those who left.

A **count plot** is used because it is the simplest way to compare the number of observations in each category.

The chart is created with **Seaborn**, which provides clear statistical visualizations with very little code and integrates well with Pandas. **Matplotlib** is used to customize the figure, titles, and axis labels.

This first visualization provides a general view of the churn rate before investigating the factors that may explain it.

---

### Contract Type Analysis

The relationship between contract type and customer churn is then examined.

A grouped **count plot** compares the number of customers who stayed and those who left for each contract category.

This visualization makes it easy to identify whether some contract types are associated with higher customer attrition.

---

### Customer Tenure Analysis

The duration of each customer's relationship with the company is analyzed using a **histogram**.

A histogram is appropriate because tenure is a continuous numerical variable. It shows how customers are distributed across different time periods.

The chart compares churn and non-churn customers in the same figure, making it possible to identify the periods where customers are most likely to leave.

---

### Monthly Charges Analysis

Monthly charges are compared between churning and non-churning customers using a **box plot**.

A box plot is selected because it summarizes the distribution of numerical values by displaying:

- Median
- Quartiles
- Minimum and maximum values
- Outliers

This allows an easy comparison of customer payment behavior between the two groups.

---

## Libraries Used

The project uses three main Python libraries.

**Pandas** is used for data loading, cleaning, and data manipulation.

**Seaborn** is used to create statistical visualizations because it offers simple functions for producing clear and informative charts.

**Matplotlib** is used together with Seaborn to customize figure size, titles, labels, and overall presentation of the graphs.

---

## Main Findings

The exploratory analysis reveals several important patterns.

- Approximately one quarter of customers leave the company.
- Customers with month-to-month contracts are much more likely to churn than customers with one-year or two-year contracts.
- The highest churn risk occurs during the first months after joining the company.
- Customers who leave generally pay higher monthly charges than those who remain.

These observations suggest that contract flexibility, customer retention during the first months, and pricing all play an important role in customer churn.

---

## Recommendations

The results of this analysis can support business decisions aimed at improving customer retention.

The company should encourage customers to move from month-to-month contracts to longer-term contracts by offering attractive discounts or additional services.

Special attention should be given to new customers during their first months through onboarding programs, personalized support, and loyalty campaigns, since this period shows the highest risk of churn.

Finally, pricing strategies should be reviewed for customers with high monthly charges. Promotional offers, personalized discounts, or service bundles could reduce dissatisfaction and lower the probability of customer attrition.

---

## Conclusion

This project demonstrates how Exploratory Data Analysis can identify the main factors associated with customer churn without using predictive models. By cleaning the data and analyzing customer characteristics through appropriate visualizations, it becomes possible to understand customer behavior and identify business opportunities.

The insights obtained from this analysis can help decision-makers develop more effective retention strategies, improve customer satisfaction, and reduce future customer losses.
```
