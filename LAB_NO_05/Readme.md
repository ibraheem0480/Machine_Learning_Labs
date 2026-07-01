# 🔄 Lab 05 – Data Transformation & Preprocessing

> **Machine Learning Laboratory** | Preparing feature-engineered time-series data for machine learning through data splitting, scaling, encoding, and preprocessing.

---

## 📖 Overview

Data transformation is a crucial step in the machine learning pipeline. Before a predictive model can be trained, the dataset must be divided into appropriate subsets, normalized, encoded, and transformed into a format suitable for learning algorithms.

This laboratory builds upon the feature-engineered **AEP Hourly Electricity Demand** dataset created in **Lab 04**. It demonstrates essential preprocessing techniques, including dataset splitting, feature scaling, categorical encoding, cyclical feature transformation, and saving preprocessing objects for future model deployment.

The laboratory consists of a single Jupyter notebook that performs the complete preprocessing workflow.

---

## 🎯 Learning Outcomes

After completing this laboratory, students will be able to:

- Load a feature-engineered dataset for machine learning
- Split data into training, validation, and testing subsets
- Understand the importance of proper dataset partitioning
- Apply **Min-Max Normalization**
- Apply **Standardization** using StandardScaler
- Encode categorical variables using One-Hot Encoding
- Transform cyclical time-based features using sine and cosine functions
- Save preprocessing objects for future inference
- Prepare datasets for machine learning and deep learning models

---

# 🛠 Software & Libraries

| Category | Tools |
|-----------|-------|
| Programming Language | Python |
| Development Environment | Jupyter Notebook |
| Data Processing | Pandas, NumPy |
| Machine Learning | Scikit-learn |
| Scaling Methods | MinMaxScaler, StandardScaler |
| Encoding Techniques | OneHotEncoder, Cyclical (Sine/Cosine) Encoding |
| Serialization | Pickle |
| Dataset | AEP Hourly Electricity Demand |

---

# 📚 Laboratory Exercise

## 📌 Exercise 5 — Data Splitting, Scaling & Encoding

**Notebook:** `Lab_5_22jzele0480.ipynb`

### Topics Covered

- Importing required libraries
- Loading the feature-engineered dataset
- Dataset inspection
- Splitting into:
  - Training Set
  - Validation Set
  - Testing Set
- Feature normalization using MinMaxScaler
- Feature standardization using StandardScaler
- One-Hot Encoding of categorical variables
- Cyclical encoding of temporal features
- Saving preprocessing objects using Pickle
- Preparing transformed datasets for machine learning

**Learning Focus**

Prepare high-quality input data that improves model convergence, generalization, and predictive performance.

---

# 🔍 Core Preprocessing Techniques

## 📌 Train, Validation & Test Split

The dataset is divided into three independent subsets:

- **Training Set** – Used to train machine learning models.
- **Validation Set** – Used to tune hyperparameters and monitor model performance.
- **Testing Set** – Used to evaluate the final trained model on unseen data.

---

## 📌 Min-Max Scaling

Min-Max Scaling transforms numerical features into a fixed range, typically between **0 and 1**.

```python
from sklearn.preprocessing import MinMaxScaler
```

This technique is particularly useful for neural networks and gradient-based optimization algorithms.

---

## 📌 Standardization

Standardization transforms data to have:

- Mean ≈ 0
- Standard Deviation ≈ 1

```python
from sklearn.preprocessing import StandardScaler
```

This improves learning performance when features have different scales.

---

## 📌 One-Hot Encoding

Categorical variables are converted into binary numerical columns using:

```python
from sklearn.preprocessing import OneHotEncoder
```

This enables machine learning algorithms to process categorical information effectively.

---

## 📌 Cyclical Feature Encoding

Time-based variables such as hours, months, and weeks follow a repeating cycle.

Instead of using raw numerical values, sine and cosine transformations preserve their circular relationships.

Examples include:

- Hour of Day
- Day of Week
- Week of Year
- Month of Year

---

# 📂 Directory Structure

```text
Lab-05/
│
├── Lab_5_22jzele0467.ipynb
├── AEPscaler.pkl
│
└── README.md
```



---

### Install Required Packages

```bash
pip install numpy pandas scikit-learn
```

---

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Run the notebook sequentially to reproduce the complete preprocessing pipeline.

---

# 📌 Skills Developed

- Dataset Preparation
- Train-Validation-Test Splitting
- Data Normalization
- Data Standardization
- One-Hot Encoding
- Cyclical Feature Encoding
- Feature Transformation
- Data Serialization using Pickle
- Machine Learning Preprocessing

---

# 🌍 Practical Applications

The preprocessing techniques demonstrated in this laboratory are widely used in:

- ⚡ Energy Demand Forecasting
- 📈 Time-Series Prediction
- 🤖 Machine Learning Pipelines
- 🧠 Deep Learning Workflows
- 🏙 Smart Grid Analytics
- 📊 Predictive Analytics
- 🔄 Data Transformation Pipelines
- 🔬 AI Research Projects

---

# 📈 Data Transformation Workflow

```text
Feature-Engineered Dataset
            │
            ▼
Train / Validation / Test Split
            │
            ▼
Feature Scaling
(Min-Max & Standardization)
            │
            ▼
Categorical Encoding
            │
            ▼
Cyclical Feature Encoding
            │
            ▼
Save Preprocessing Objects
            │
            ▼
Model-Ready Dataset
```

---

# 🎓 Course Information

| Item | Details |
|------|---------|
| Course | Machine Learning Laboratory |
| Lab | Lab 05 |
| Topic | Data Transformation & Preprocessing |
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

This laboratory was completed as part of the Machine Learning Laboratory course to develop practical skills in transforming and preparing datasets for predictive modeling. The preprocessing techniques implemented in this lab provide a solid foundation for subsequent machine learning and deep learning laboratories involving regression, neural networks, and time-series forecasting.

---

# 📜 License

This project is intended for **educational and research purposes**.

You are welcome to use, modify, and extend the material for academic learning while providing appropriate credit to the original author.

---

## ⭐ Support

If you found this laboratory helpful, consider giving the repository a **Star ⭐** on GitHub.
