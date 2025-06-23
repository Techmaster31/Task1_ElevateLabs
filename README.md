# Task1_ElevateLabs
First task of the Internship.

# 🧹 Task 1: Data Cleaning and Preprocessing

## 📌 Objective
Clean and prepare a raw dataset by handling missing values, removing duplicates, and ensuring consistent formatting for analysis.

## 🛠 Tools Used
- Python 3
- Pandas
- Jupyter Notebook / VSCode / Any Python IDE

## 📂 Dataset
**Dataset Used:** `marketing_campaign.csv`  
**Source:** [Kaggle - Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)

## 🔍 Data Cleaning Steps

### 1. Handle Missing Values
- Checked for missing values using `.isnull().sum()`.
- Filled 24 missing values in the `Income` column using the **median** strategy.

### 2. Remove Duplicate Rows
- Verified using `.duplicated().sum()`.
- No duplicate records found, so no rows removed.

### 3. Convert Date Formats
- Converted `Dt_Customer` column to Python `datetime` format (`YYYY-MM-DD`) using `pd.to_datetime()`.

### 4. Standardize Text Values
- Converted `Education` and `Marital_Status` to lowercase and stripped whitespaces for consistency.

### 5. Rename Column Headers
- Transformed all column headers to lowercase and replaced spaces with underscores for clean and uniform naming.

### 6. Fix Data Types
- Ensured `year_birth` and `recency` were integers.
- Checked that `Dt_Customer` was of type `datetime64`.

## 📁 Output
- ✅ Cleaned file saved as: `cleaned_marketing_campaign.csv`
