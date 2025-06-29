# 📊 Layoffs SQL Data Analysis Project

This project focuses on analyzing large-scale layoffs in the tech industry using structured SQL queries. It includes **data cleaning**, **standardization**, and **exploratory data analysis (EDA)** to uncover insights from company layoffs.

# 📁 Dataset

**File:** `layoffs.csv`  
**Source:** Publicly available dataset of tech layoffs (2020–2023) 

---

## 📁 Files

- **Data Cleaning-Layoffs.sql**: Prepares the raw data by removing duplicates, cleaning nulls, fixing formats, and standardizing values.
- **EDA-Layoffs.sql**: Performs insights extraction from cleaned data using SQL queries.

---

## 🔧 Data Cleaning Highlights
1. ✅ Removed duplicate rows using `ROW_NUMBER()`.
2. ✅ Handled blank/NULL values in `industry`, `percentage_laid_off`, and `total_laid_off`.
3. ✅ Trimmed extra spaces and periods from `company` and `country`.
4. ✅ Standardized date format and converted `date` column to `DATE` type.
5. ✅ Standardized industries (e.g., “Crypto”, “Fintech”).
6. ✅ Dropped unnecessary columns (like `row_num`) post-cleaning.

---

## 📊 EDA Highlights & Insights

### 🔹 Total Layoffs
- Peak layoffs happened in the years **2022 and 2023**.
- Companies with highest layoffs include **Meta, Amazon, Google**.

### 🔹 100% Layoffs
- Several startups shut down completely even after raising millions.

### 🔹 Country-wise Layoffs
- 🇺🇸 **United States** leads by a huge margin, followed by 🇮🇳 India and 🇬🇧 UK.

### 🔹 Funding Stage Analysis
- Startups in **Late Stage (Series C or beyond)** had the most layoffs.

### 🔹 Time-based Trend
- Layoffs peaked in **mid-2022**, followed by a decline in 2024.
- Used a **rolling total** to observe cumulative layoffs over time.

### 🔹 Company & Year-wise Ranking
- Each year's **top 5 companies** with the most layoffs were ranked using `DENSE_RANK()`.

---

## 📁 Table Used

- `layoffs_staging2`: Cleaned table with all standardized values.

---

## 🛠 Tools Used

- MySQL / SQL
- GitHub (for version control)

---

## 🚀 How to Use
1. Clone this repository
2. Run `Data Cleaning-Layoffs.sql` first
3. Then run `EDA-Layoffs.sql` to extract insights

---

GitHub Repository: [Your GitHub Repo URL](https://github.com/yourusername/layoffs-sql-analysis)

