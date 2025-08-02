# sql-covid-data-analysis-portfolio
This project contains a series of SQL queries used to analyze COVID-19 data from two main datasets: **CovidDeaths** and **CovidVaccination**. It aims to uncover insights related to infection trends, death rates, vaccination progress, and population-level comparisons using SQL Server.

## 🧰 Technologies Used

- **SQL Server (T-SQL)**
- **SQL Server Management Studio (SSMS)** or compatible SQL tool
- Datasets: `PortfolioProject..CovidDeaths`, `PortfolioProject..CovidVaccination`

---

## 📊 Analysis Covered

### ✅ Death Rate Analysis
- Likelihood of dying from COVID-19 in a given country.
- Calculation of death percentage over time:
  ```sql
  (CAST(total_deaths AS INT) / total_cases) * 100

✅ Infection Rate Analysis
-Percentage of population infected over time:
  (total_cases / population) * 100
-Countries with the highest infection rates.

✅ Country-Level Metrics
-Highest death counts and infection counts by location.
-Infection and mortality trends in specific countries (e.g. India).

✅ Vaccination Progress (commented out but structured for extension)
-Percentage of population vaccinated.
-Comparing vaccination vs. infection rates.

📌 Key SQL Techniques Used
-Filtering using WHERE, LIKE, and IS NOT NULL
-Aggregation with MAX, SUM, and GROUP BY
-Type casting using CAST(...) AS INT
-Mathematical operations for percentage calculations
-Date-based sorting and ordering

🧠 Learning Outcomes
-Real-world SQL querying on global health datasets
-Use of aggregate functions for comparative analysis
-Handling nulls, joins (optional), and subqueries
-Building reusable and modular SQL code for reporting

🚀 How to Use
-Load the CovidDeaths and CovidVaccination datasets into SQL Server under the PortfolioProject database.
-Open ProjectPortfolio.sql in SSMS or your preferred SQL IDE.
-Run each section to generate insights or modify queries for deeper exploration.

🙌 Acknowledgements
-Data is assumed to be from publicly available COVID-19 sources like Our World in Data.
-Inspired by common analytical use cases in data science and business intelligence.
