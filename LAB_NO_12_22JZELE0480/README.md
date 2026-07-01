# 🔄 Lab 12 – Long Short-Term Memory (LSTM) for Time-Series Forecasting

> **Machine Learning Laboratory** | Forecasting electricity demand using Long Short-Term Memory (LSTM) neural networks.

---

## 📖 Overview

Long Short-Term Memory (LSTM) networks are a specialized type of Recurrent Neural Network (RNN) designed to learn long-term dependencies in sequential data. They are widely used for time-series forecasting because they can retain important historical information while overcoming the limitations of traditional recurrent networks.

In this laboratory, an **LSTM model** is developed using the preprocessed **AEP Hourly Electricity Demand** dataset to forecast future electricity demand. The complete deep learning workflow includes data loading, model construction, training, checkpointing, prediction, and performance evaluation.

The laboratory consists of a single Jupyter notebook implementing the complete LSTM forecasting pipeline.

---

## 🎯 Learning Outcomes

After completing this laboratory, students will be able to:

- Understand the architecture of Long Short-Term Memory (LSTM) networks
- Prepare sequential data for LSTM models
- Build an LSTM forecasting model using TensorFlow/Keras
- Configure optimizers, loss functions, and evaluation metrics
- Apply dropout regularization to improve generalization
- Use callbacks for model checkpointing and training monitoring
- Train and validate deep learning models
- Generate forecasts from sequential input data
- Evaluate forecasting performance using regression metrics

---

# 🛠 Software & Libraries

| Category | Tools |
|-----------|-------|
| Programming Language | Python |
| Development Environment | Jupyter Notebook |
| Data Processing | NumPy, Pandas |
| Deep Learning Framework | TensorFlow, Keras |
| Model Type | Long Short-Term Memory (LSTM) |
| Layers | Input, LSTM, Dropout, Dense |
| Optimization | Adam, SGD |
| Callbacks | ModelCheckpoint |
| Evaluation Metrics | MAE, MSE, RMSE, R² Score, Explained Variance |
| File Handling | Pickle, CSV |

---

# 📚 Laboratory Exercise

## 📌 Exercise 12 — LSTM for Time-Series Forecasting

**Notebook:** `Lab_12_22JZELE0480.ipynb`

### Topics Covered

- Importing TensorFlow/Keras libraries
- Loading training, validation, and testing datasets
- Defining time steps and feature dimensions
- Building an LSTM architecture
- Displaying model summary
- Visualizing the model architecture
- Configuring optimizer and loss function
- Setting up ModelCheckpoint callbacks
- Training the LSTM model
- Monitoring training and validation performance
- Predicting future electricity demand
- Evaluating forecasting performance

**Learning Focus**

Develop an LSTM-based forecasting model capable of learning temporal dependencies from historical electricity demand data and accurately predicting future demand.

---

# 🔍 Core Deep Learning Concepts

## 📌 Long Short-Term Memory (LSTM)

LSTM is a specialized recurrent neural network architecture that learns both short-term and long-term dependencies in sequential data using memory cells and gating mechanisms.

Unlike traditional neural networks, LSTMs are designed to retain important historical information over extended time periods, making them highly effective for forecasting applications.

---

## 📌 Sequential Data Modeling

Sequential data contains observations arranged in chronological order.

The LSTM model processes historical sequences to learn temporal patterns and predict future values.

---

## 📌 Model Checkpointing

Model checkpointing automatically saves the best-performing model during training based on validation performance.

This ensures that the most accurate model is preserved for future predictions.

---

## 📌 Forecast Evaluation

The forecasting model is evaluated using standard regression metrics, including:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Coefficient of Determination (R² Score)
- Explained Variance Score

---

# 📂 Directory Structure

```text
Lab-12/
│
├── Lab_12_22JZELE0480.ipynb
├── AEP_train.csv
├── AEP_validation.csv
├── AEP_test.csv
├── AEP_scaler.pkl
│
└── README.md
```


---

### Install Required Packages

```bash
pip install numpy pandas scikit-learn tensorflow keras h5py
```

---

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Run the notebook sequentially to train and evaluate the LSTM forecasting model.

---

# 📌 Skills Developed

- Time-Series Forecasting
- Long Short-Term Memory (LSTM)
- Sequential Data Modeling
- TensorFlow & Keras
- Deep Learning Model Design
- Model Training
- Dropout Regularization
- Model Checkpointing
- Forecast Performance Evaluation
- Energy Demand Prediction

---

# 🌍 Practical Applications

The techniques demonstrated in this laboratory are widely used in:

- ⚡ Electricity Demand Forecasting
- 🏙 Smart Grid Analytics
- 📈 Energy Consumption Prediction
- 🏭 Industrial Monitoring
- 🌦 Weather Forecasting
- 📊 Financial Time-Series Analysis
- 🔧 Predictive Maintenance
- 🤖 AI-Based Forecasting Systems

---

# 📈 Forecasting Workflow

```text
Historical Time-Series Data
            │
            ▼
Sequence Preparation
            │
            ▼
LSTM Network
            │
            ▼
Learning Temporal Dependencies
            │
            ▼
Model Training
            │
            ▼
Prediction
            │
            ▼
Performance Evaluation
(MAE • MSE • RMSE • R²)
```

---

# 🎓 Course Information

| Item | Details |
|------|---------|
| Course | Machine Learning Laboratory |
| Lab | Lab 12 |
| Topic | Long Short-Term Memory (LSTM) for Time-Series Forecasting |
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

This laboratory was completed as part of the **Machine Learning Laboratory** course to develop practical skills in applying Long Short-Term Memory (LSTM) networks for time-series forecasting. The implementation demonstrates how recurrent neural networks can effectively capture long-term temporal dependencies, providing a strong foundation for advanced forecasting and sequential data analysis.

---

# 📜 License

This project is intended for **educational and research purposes**.

You are welcome to use, modify, and extend the material for academic learning while providing appropriate credit to the original author.

---

## ⭐ Support

If you found this laboratory helpful, consider giving the repository a **Star ⭐** on GitHub.
