# ⚙️ Lab 04 – Feature Engineering & Correlation Analysis

> **Machine Learning Laboratory** | Transforming raw time-series data into meaningful machine learning features and analyzing their relationships with the target variable.

---

## 📖 Overview

Feature engineering is one of the most important stages in the machine learning workflow. This laboratory focuses on extracting meaningful features from the cleaned **AEP Hourly Electricity Demand** dataset prepared in the previous lab.

By deriving temporal and seasonal attributes from the **Datetime** column, the dataset becomes more informative for predictive modeling. The laboratory also introduces correlation analysis techniques to evaluate how different features influence electricity demand.

The lab is organized into two Jupyter notebooks, covering feature creation and statistical relationship analysis.

---

## 🎯 Learning Outcomes

After completing this laboratory, students will be able to:

- Extract informative features from date and time values
- Create temporal features such as hour, month, week, and quarter
- Generate binary indicators for weekends and day/night periods
- Engineer seasonal features for annual demand patterns
- Organize and rename dataset columns for better readability
- Save processed datasets for future machine learning tasks
- Perform correlation analysis using multiple statistical methods
- Interpret feature importance based on correlation coefficients

---

# 🛠 Software & Libraries

| Category | Tools |
|-----------|-------|
| Programming Language | Python |
| Development Environment | Jupyter Notebook |
| Data Processing | Pandas, NumPy |
| Dataset | AEP Hourly Electricity Demand |
| Feature Engineering | Date-Time Extraction, Seasonal Features, Binary Indicators |
| Statistical Analysis | Pearson, Kendall, Spearman Correlation |

---

# 📚 Laboratory Exercises

## 📌 Exercise 4.1 — Time-Series Feature Engineering

**Notebook:** `Lab_04_Part_01_22jzele0480.ipynb`

### Topics Covered

- Loading the cleaned AEP dataset
- Extracting hour, month, and day-of-week
- Computing ISO week number
- Extracting day of year and quarter
- Creating weekend indicators
- Creating day/night indicators
- Generating seasonal features
  - Winter
  - Spring
  - Summer
  - Autumn
- Renaming and organizing dataset columns
- Saving the feature-engineered dataset

**Learning Focus**

Convert raw temporal information into meaningful machine learning features that capture daily, weekly, monthly, and seasonal patterns in electricity demand.

---

## 📌 Exercise 4.2 — Feature Correlation Analysis

**Notebook:** `Lab_04_Part_02_22jzele0480.ipynb`

### Topics Covered

- Loading the feature-engineered dataset
- Setting Datetime as the index
- Pearson correlation analysis
- Kendall correlation analysis
- Spearman correlation analysis
- Missing value inspection
- Feature-target relationship analysis

**Learning Focus**

Evaluate the strength and direction of relationships between engineered features and the target variable to support effective feature selection and model development.

---

# 📂 Directory Structure

```text
Lab-04/
│
├── Lab_04_Part_01_22jzele0480.ipynb
├── Lab_04_Part_02_22jzele0480.ipynb
│
└── README.md
```


---

### Install Required Packages

```bash
pip install numpy pandas
```

---

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebooks and execute the cells sequentially to reproduce the feature engineering and correlation analysis workflow.

---

# 📌 Skills Developed

- Time-Series Feature Engineering
- Date & Time Processing
- Temporal Feature Extraction
- Seasonal Feature Creation
- Binary Feature Engineering
- Feature Organization
- Correlation Analysis
- Statistical Interpretation
- Machine Learning Data Preparation

---

# 🌍 Practical Applications

The techniques introduced in this laboratory are commonly used in:

- ⚡ Energy Demand Forecasting
- 📈 Time-Series Forecasting
- 🤖 Machine Learning Pipelines
- 🏙 Smart Grid Analytics
- 📊 Predictive Modeling
- 🔍 Feature Selection
- 🧠 Deep Learning Data Preparation
- 🔬 Engineering Research

---

# 📈 Feature Engineering Workflow

```text
Cleaned Time-Series Dataset
            │
            ▼
Date-Time Feature Extraction
            │
            ▼
Weekend & Day/Night Indicators
            │
            ▼
Seasonal Feature Generation
            │
            ▼
Correlation Analysis
            │
            ▼
Machine Learning Ready Dataset
```

---

# 🎓 Course Information

| Item | Details |
|------|---------|
| Course | Machine Learning Laboratory |
| Lab | Lab 04 |
| Topic | Feature Engineering & Correlation Analysis |
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

This laboratory was completed as part of the Machine Learning Laboratory course to develop practical skills in transforming raw time-series data into meaningful predictive features. The feature engineering and correlation analysis techniques presented here establish a strong foundation for subsequent machine learning and deep learning laboratories.

---

# 📜 License

This project is intended for **educational and research purposes**.

You are welcome to use, modify, and extend the material for academic learning while providing appropriate credit to the original author.

---

## ⭐ Support

If you found this laboratory helpful, consider giving the repository a **Star ⭐** on GitHub.
