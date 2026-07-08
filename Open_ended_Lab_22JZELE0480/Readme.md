
CityLearn Demand Forecasting - Open Ended ML Lab
🚀 Machine Learning Lab 13 | CityLearn Demand Forecasting Project
This project develops a comprehensive machine learning and deep learning forecasting pipeline for the CityLearn challenge dataset. The primary objective is to design an LSTM-based model capable of forecasting district-level electricity demand by leveraging building energy data, weather information, electricity pricing, carbon intensity data, and sophisticated time-series feature engineering.

📖 Project Overview
CityLearn is an open-source environment developed for demand response research, building energy management, and reinforcement learning applications in smart grid systems. In this lab, the CityLearn dataset is repurposed for a supervised time-series forecasting task where the model predicts district net electricity consumption.

The project follows a complete machine learning workflow including:

Data Acquisition: Dataset loading from CityLearn framework

Feature Extraction: Building-level energy data collection and aggregation

Target Creation: District-level net electricity demand generation

Data Integration: Merging with weather, pricing, and carbon intensity data

Data Preprocessing: Cleaning and handling missing values

Feature Engineering: Creating time-based features for pattern recognition

Feature Scaling: Using saved scaler (AEP_scaler.pkl) for normalization

Sequence Preparation: Time-series sequence creation with lookback window

Model Development: LSTM neural network architecture design

Model Training: Training with checkpointing and validation monitoring

Performance Evaluation: Comprehensive forecast evaluation and visualization

🎯 Objectives
The main objectives of this open-ended lab include:

Understanding Dataset Structure: Gain familiarity with CityLearn dataset organization and schema

Data Processing: Extract and combine building-level electricity consumption data

Target Aggregation: Create district-level net electricity demand from individual buildings

Feature Integration: Merge demand data with weather, pricing, and carbon intensity features

Time-Series Preparation: Prepare sequential data suitable for deep learning models

Model Development: Build and train an LSTM forecasting model with optimal architecture

Performance Assessment: Evaluate model performance using comprehensive regression metrics

Model Optimization: Improve validation performance through better preprocessing and training strategies

🛠️ Technology Stack
Category	Tools / Libraries
Programming Language	Python 3.x
Development Environment	Jupyter Notebook
Data Handling	Pandas, NumPy
Data Visualization	Matplotlib
Machine Learning	Scikit-learn
Deep Learning	TensorFlow, Keras
Dataset Source	CityLearn Framework
Model Architecture	LSTM Neural Network
Scaling File	AEP_scaler.pkl
Model Persistence	Keras .h5 checkpoints
📁 Project Structure
text
CityLearn Assignment/
│
├── Open_Ended_Lab_22JZELE0480.ipynb        # Main Jupyter Notebook
├── AEP_scaler.pkl                       # Pre-trained scaler file
├── history.json                         # Training history data
├── history.png                          # Training history visualization
├── Lab 13 Open Ended ML.docx            # Lab report documentation
│
├── Model Checkpoints/
│   ├── E1-cp-0001-loss0.12.h5
│   ├── E1-cp-0002-loss0.11.h5
│   ├── E1-cp-0005-loss0.10.h5
│   ├── ...
│   └── E1-cp-0030-loss0.07.h5
│
└── README.md                            # Project documentation
📚 Detailed Workflow
🔹 1. Library Import and Setup
The notebook begins by importing essential Python libraries:

python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from sklearn.preprocessing import MinMaxScaler
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import LSTM, Dense, Dropout
from citylearn.data import DataSet
import pickle
🔹 2. CityLearn Dataset Loading
The CityLearn dataset is accessed through the framework's built-in data loading mechanism:

python
from citylearn.data import DataSet
# Available datasets are checked and the appropriate CityLearn challenge dataset is selected
🔹 3. Building Data Collection
Individual building electricity data is extracted from the CityLearn schema and compiled into a unified dataframe for district-level analysis.

🔹 4. District Demand Creation
Building-level energy consumption values are aggregated by time_step to create:

python
district_net_electricity_consumption = sum(building_data for building in buildings)
This aggregated value serves as the primary forecasting target.

🔹 5. Feature Integration
The demand dataset is augmented with additional features including:

Weather Data: Temperature, humidity, solar radiation, wind speed

Electricity Pricing: Dynamic pricing information

Carbon Intensity: Carbon emission factors for electricity

🔹 6. Data Cleaning and Preprocessing
Missing values are handled using appropriate imputation techniques:

python
data = data.ffill()  # Forward fill
data = data.bfill()  # Backward fill
# Columns with all missing values are removed
🔹 7. Feature Engineering
Time-based features are created to capture periodic patterns:

Hour of Day: Sine/cosine encoding for cyclical nature

Day of Week: Day encoding for weekly patterns

Month: Seasonal patterns

Day of Year: Annual seasonality

python
data['hour_sin'] = np.sin(2 * np.pi * data['hour'] / 24)
data['hour_cos'] = np.cos(2 * np.pi * data['hour'] / 24)
🔹 8. Feature Scaling
The pre-trained scaler file AEP_scaler.pkl is loaded and applied:

python
scaler_path = r'Z:\University\8th Semester\ML Lab\CityLearn Assignment\AEP_scaler.pkl'
with open(scaler_path, 'rb') as f:
    scaler = pickle.load(f)
A compatibility check ensures the scaler matches the current dataset features. If incompatible, a new scaler is fitted to maintain workflow continuity.

🔹 9. Sequence Creation
Time-series data is converted to supervised learning sequences using a sliding window:

python
time_steps = 24  # Using 24 hours of history to predict next value
X, y = create_sequences(scaled_data, time_steps)
🔹 10. LSTM Model Architecture
The LSTM model is constructed using TensorFlow/Keras with:

python
model = Sequential([
    LSTM(64, return_sequences=True, input_shape=(time_steps, n_features)),
    Dropout(0.2),
    LSTM(32, return_sequences=False),
    Dropout(0.2),
    Dense(1)
])
🔹 11. Model Training
Training includes:

Model checkpoints saving the best performing models

Validation monitoring to prevent overfitting

Early stopping for optimal training duration

python
checkpoint = ModelCheckpoint('E1-cp-{epoch:04d}-loss{val_loss:.2f}.h5', 
                             monitor='val_loss', save_best_only=True)
🔹 12. Forecast Evaluation
The model's predictions are inverse-transformed to original scale and evaluated using:

Metric	Description
MAE	Mean Absolute Error
MedAE	Median Absolute Error
MSE	Mean Squared Error
RMSE	Root Mean Squared Error
R² Score	Coefficient of Determination
Explained Variance	Variance Explained
Visual comparisons of actual vs predicted demand values are generated for intuitive assessment.

⚙️ Installation and Setup
Prerequisites
Python 3.7 or higher

Jupyter Notebook

Required Python packages

Installation Commands
bash
# Install required packages
pip install numpy pandas matplotlib scikit-learn tensorflow keras citylearn h5py

# Launch Jupyter Notebook
jupyter notebook

# Open the notebook
Open_Ended_Lab_22JZELE0480.ipynb

# Execute cells sequentially
🚀 Key Skills Demonstrated
CityLearn Framework: Working with energy management datasets

Data Preprocessing: Cleaning, imputation, and transformation

Feature Engineering: Creating predictive features from raw data

Time-Series Analysis: Sequence creation and window-based prediction

Deep Learning: LSTM architecture design and optimization

Model Training: Checkpointing, validation, and performance monitoring

Model Evaluation: Comprehensive regression metrics implementation

Energy Forecasting: Real-world demand prediction application

🌟 Applications and Use Cases
This project has practical applications in:

Smart Building Management: Optimizing energy consumption patterns

Demand Response Systems: Predicting peak demand for load shifting

Power Distribution Planning: Infrastructure capacity planning

Smart Grid Optimization: Balancing supply and demand

Energy Management Systems: Operational optimization

Load Forecasting Research: Academic and industrial research

AI for Power Systems: Advanced analytics in energy sector

📊 Results and Performance
The trained LSTM model successfully captures:

Daily Patterns: Diurnal variations in electricity demand

Weekly Patterns: Weekend vs weekday consumption differences

Seasonal Trends: Long-term demand fluctuations

Weather Impacts: Environmental effects on consumption

The model checkpoints demonstrate progressive improvement with validation loss decreasing from 0.12 to 0.07 over training epochs.

👨‍💻 Author Information
IBRAHEEM KHAN
Registration Number: 22JZELE0480

Course: Machine Learning Lab (Open Ended Project)
Supervisor: Engr. Irshad Ullah
Department: Electrical Engineering
Institution: UET Peshawar - Nowshera Campus

Research Interests: Machine Learning, Energy Forecasting, Smart Grid Systems, Deep Learning Applications
