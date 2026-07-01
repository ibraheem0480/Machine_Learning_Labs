# 🧹 Lab 03 – Data Cleaning & Preprocessing

> **Machine Learning Laboratory** | Preparing real-world time-series data through cleaning, preprocessing, outlier detection, and feature enhancement.

---

## 📖 Overview

Data preprocessing is a critical stage in every machine learning pipeline. This laboratory introduces essential techniques for cleaning and preparing real-world time-series datasets before feature engineering and model development.

Using the **AEP Hourly Electricity Demand** dataset, this lab demonstrates how to inspect data quality, identify missing timestamps, detect outliers, and integrate external holiday information to improve dataset usability for predictive modeling.

The laboratory consists of three Jupyter notebooks, each focusing on a specific preprocessing task.

---

## 🎯 Learning Outcomes

After completing this laboratory, students will be able to:

- Load and inspect large time-series datasets
- Parse and manipulate date-time information using Pandas
- Explore dataset structure and descriptive statistics
- Detect missing timestamps and missing values
- Identify outliers using the Interquartile Range (IQR) method
- Visualize abnormal observations with boxplots
- Merge external holiday calendars with time-series data
- Prepare clean datasets for machine learning workflows

---

# 🛠 Software & Libraries

| Category | Tools |
|-----------|-------|
| Programming Language | Python |
| Development Environment | Jupyter Notebook |
| Data Processing | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Dataset | AEP Hourly Electricity Demand |
| Preprocessing Techniques | Missing Value Handling, IQR Outlier Detection, Data Merging |

---

# 📚 Laboratory Exercises

## 📌 Exercise 3.1 — Dataset Exploration & Missing Timestamp Analysis

**Notebook:** `Lab_03_Part_01_22JZELE04480.ipynb`

### Topics Covered

- Importing required libraries
- Loading CSV datasets
- Parsing date-time columns
- Dataset inspection
- Data types and summary statistics
- Identifying missing timestamps
- Exploring the overall time range

**Learning Focus**

Understand the structure, completeness, and quality of a real-world time-series dataset before applying preprocessing techniques.

---

## 📌 Exercise 3.2 — Outlier Detection Using IQR

**Notebook:** `Lab_03_Part_02_22JZELE04480.ipynb`

### Topics Covered

- Loading cleaned datasets
- Boxplot visualization
- Quartile calculation (Q1 & Q3)
- Interquartile Range (IQR)
- Detecting abnormal observations
- Identifying outlier indices
- Preparing data for further processing

**Learning Focus**

Learn how statistical techniques can identify extreme values that may negatively affect machine learning model performance.

---

## 📌 Exercise 3.3 — Holiday Feature Integration

**Notebook:** `Lab_03_Part_03_22JZELE04480.ipynb`

### Topics Covered

- Loading holiday datasets
- Date normalization
- Feature merging
- Removing unnecessary columns
- Joining external calendar information
- Preparing enriched datasets

**Learning Focus**

Enhance predictive performance by incorporating calendar-based features that influence electricity demand patterns.

---

# 📂 Directory Structure

```text
Lab-03/
│
├── Lab_03_Part_01_22JZELE04480.ipynb
├── Lab_03_Part_02_22JZELE04480.ipynb
├── Lab_03_Part_03_22JZELE04480.ipynb
│
└── README.md
```

---


### Install Required Packages

```bash
pip install numpy pandas matplotlib seaborn
```

---

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Run each notebook sequentially to reproduce the preprocessing workflow.

---

# 📌 Skills Developed

- Time-Series Data Analysis
- Exploratory Data Analysis (EDA)
- Data Cleaning
- Missing Timestamp Detection
- Missing Value Analysis
- Statistical Outlier Detection
- Feature Integration
- Dataset Merging
- Data Preprocessing for Machine Learning

---

# 🌍 Practical Applications

The techniques covered in this laboratory are commonly used in:

- ⚡ Electricity Demand Forecasting
- 📈 Time-Series Prediction
- 🏙 Smart Grid Analytics
- 🤖 Machine Learning Pipelines
- 📊 Predictive Analytics
- 🧹 Data Cleaning Workflows
- 🔬 Engineering Research
- 📉 Load Forecasting Systems

---

# 📈 Data Preparation Workflow

```text
Raw AEP Dataset
        │
        ▼
Dataset Inspection
        │
        ▼
Missing Timestamp Analysis
        │
        ▼
Outlier Detection (IQR)
        │
        ▼
Holiday Feature Integration
        │
        ▼
Clean Machine Learning Dataset
```

---

# 🎓 Course Information

| Item | Details |
|------|---------|
| Course | Machine Learning Laboratory |
| Lab | Lab_03 |
| Topic | Data Cleaning & Preprocessing |
| Institution | UET Peshawar – Nowshera Campus |

---

# 👨‍💻 Author

**IBRAHEEM KHAN**

**Registration Number:** 22JZELE0480

**Department:** Electrical Engineering

**Course:** Machine Learning Laboratory

**Supervisor:** Engr. Irshad Ullah

**Institution:** University of Engineering & Technology (UET) Peshawar – Nowshera Campus

---

# 📄 Academic Note

This laboratory was completed as part of the Machine Learning Laboratory course to develop practical expertise in preparing real-world time-series datasets for predictive modeling. The preprocessing techniques introduced here establish the foundation for subsequent laboratories involving feature engineering, machine learning, and deep learning applications.

---

# 📜 License

This project is provided for **educational and research purposes**.

You are welcome to use, modify, and extend the material for academic learning while giving appropriate credit to the original author.

---

## ⭐ Support

If you found this laboratory helpful, consider giving the repository a **Star ⭐** on GitHub.
