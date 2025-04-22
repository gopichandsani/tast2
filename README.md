# Gender Distribution Across Age Groups – Power BI Report

This Power BI project presents an interactive dashboard that visualizes the count of male and female customers within various age groups. It provides insights into demographic breakdowns using clear visualizations, such as pie charts and bar graphs.

## 📊 Features

- Gender-wise distribution of customers
- Age group categorization (e.g., 18–25, 26–35, 36–45,....)
- Pie charts with in-slice data labels for clarity
- Bar charts showing gender counts per age group
- Custom text annotations and dynamic labeling

## 🔧 Tools Used

- Power BI Desktop
- DAX (for calculated columns and measures)
- Power Query (for age grouping)

## 🧮 Data Columns

- `age`: Numeric age of the customer
- `gender`: Gender of the customer (e.g., Male, Female)
- `customerid`: Unique identifier for each customer

## 📝 Data Transformations

- **Age Grouping**:
  ```powerquery
  Age Group = 
  if [age] <= 25 then "18-25" 
  else if [age] <= 35 then "26-35" 
  else if [age] <= 45 then "36-45"
  else if [age] <= 55 then "46-55" 
  else "above 56"
