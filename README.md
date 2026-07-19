# 🧹 Week 1 – Applicant Dataset Cleaning & Exploration

## 📌 Project Overview

This project focuses on cleaning and exploring a real-world style applicant dataset using **Python** and **Pandas**. The objective is to identify common data quality issues, clean the dataset systematically, and prepare it for further analysis or machine learning.

The notebook follows a complete data cleaning workflow, documenting every decision and verifying each transformation before exporting the final cleaned dataset.

---

## 🎯 Objectives

- Explore the dataset before making any modifications.
- Identify and handle missing values.
- Detect and remove duplicate records.
- Standardize inconsistent text fields.
- Convert incorrect data types.
- Produce a clean, analysis-ready dataset.
- Document every cleaning decision for reproducibility.

---

## 🗂 Dataset

The dataset contains applicant information with the following fields:

- Applicant Name
- Email
- Phone
- Domain Applied
- University
- Application Date
- Status

To simulate real-world data quality issues, the dataset intentionally contains:

- Missing values
- Duplicate records
- Inconsistent capitalization
- Different spellings of the same domain
- Extra spaces
- Inconsistent phone number formatting
- Mixed date formats

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Faker (for generating synthetic applicant data)
- Jupyter Notebook

---

## 📋 Project Workflow

### 1. Dataset Exploration

Performed an initial inspection using:

- Dataset shape
- Data types
- Missing values
- Duplicate records
- Unique values
- Basic statistics

---

### 2. Missing Value Handling

Handled missing values on a column-by-column basis using appropriate strategies.

Examples include:

- Dropping rows with missing critical identifiers.
- Filling non-critical fields with meaningful default values.
- Justifying every cleaning decision.

---

### 3. Duplicate Removal

Removed:

- Exact duplicate rows
- Near-duplicate applicant records using Email as a unique identifier

---

### 4. Text Standardization

Standardized multiple text columns, including:

- Applicant Name
- Domain Applied
- University
- Status

Cleaning included:

- Removing leading/trailing spaces
- Standardizing capitalization
- Mapping inconsistent spellings to a single standard format

Example:

```
web dev
WEB DEV
Web Development
```

↓

```
Web Development
```

---

### 5. Phone Number Cleaning

Standardized phone numbers by:

- Removing spaces
- Removing hyphens
- Keeping a single consistent numeric format

Example:

```
0301-1234567
0301 1234567
```

↓

```
03011234567
```

---

### 6. Date Conversion

Converted the **Application Date** column into proper datetime format using Pandas.

---

### 7. Verification

After every cleaning step, verification was performed by checking:

- Missing values
- Unique categories
- Frequency counts
- Data types
- Duplicate records

This ensured every transformation produced the expected result.

---

### 8. Export

The cleaned dataset was exported as:

```
applicants_cleaned.csv
```

---

## 📂 Repository Structure

```
├── Week1_Data_Cleaning_Eimon.ipynb
├── applicants.csv
├── applicants_cleaned.csv
└── README.md
```

---

## 📈 Skills Demonstrated

- Data Cleaning
- Data Wrangling
- Exploratory Data Analysis (EDA)
- Data Quality Assessment
- Pandas
- Python Programming
- Data Validation
- Feature Standardization
- Documentation

---

## 📚 Key Learning Outcomes

Through this project I learned how to:

- Inspect data before cleaning.
- Make justified data cleaning decisions.
- Handle missing values appropriately.
- Remove duplicate records.
- Standardize categorical variables.
- Validate every cleaning operation.
- Produce a reproducible data cleaning pipeline.

---

## 🚀 Future Improvements

- Automate validation checks.
- Build reusable data cleaning functions.
- Generate a complete data quality report.
- Integrate the cleaning pipeline into an ETL workflow.

---

## 👩‍💻 Author

**Eimon Arooj Mazhar**

Computer Science Graduate | Data Science Intern

---

> **Note:** This project was completed as part of a Data Science internship assignment to practice real-world data cleaning, preprocessing, and documentation using Python and Pandas.
