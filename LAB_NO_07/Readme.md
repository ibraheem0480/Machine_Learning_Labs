# 🖼️ Lab 07 – Computer Vision Dataset Preparation

> **Machine Learning Laboratory** | Preparing image datasets for deep learning-based image classification using TensorFlow/Keras.

---

## 📖 Overview

A well-structured dataset is essential for building accurate deep learning models. This laboratory focuses on organizing image datasets into a standardized directory structure suitable for Convolutional Neural Networks (CNNs).

Using Python file handling utilities, the dataset is divided into **training**, **validation**, and **testing** subsets with separate folders for each image class. The prepared dataset serves as the foundation for the CNN image classification model developed in **Lab 08**

The laboratory consists of a single Jupyter notebook that automates the dataset preparation process.

---

## 🎯 Learning Outcomes

After completing this laboratory, students will be able to:

- Understand the structure of image classification datasets
- Organize images into training, validation, and testing sets
- Create class-wise directory structures using Python
- Automate dataset preparation using file handling libraries
- Prepare datasets compatible with TensorFlow/Keras
- Understand how folder-based datasets are used for image classification
- Build an efficient workflow for computer vision projects

---

# 🛠 Software & Libraries

| Category | Tools |
|-----------|-------|
| Programming Language | Python |
| Development Environment | Jupyter Notebook |
| File Handling | OS, Shutil |
| Data Processing | NumPy |
| Deep Learning Framework | TensorFlow / Keras |
| Dataset Preparation | Folder Organization |
| Image Loading | ImageDataGenerator (Lab 08) |

---

# 📚 Laboratory Exercise

## 📌 Exercise 7 — Image Dataset Preparation

**Notebook:** `Lab_07_22JZELE0480.ipynb`

### Topics Covered

- Importing required Python libraries
- Defining the original image dataset directory
- Creating a computer vision workspace
- Creating:
  - Training folder
  - Validation folder
  - Testing folder
- Creating class-wise directories
- Copying images into their respective folders
- Organizing data for TensorFlow/Keras image generators

**Learning Focus**

Prepare an image dataset in a standardized format that enables efficient loading, preprocessing, and training of Convolutional Neural Networks.

---

# 📂 Dataset Structure

```text
Computer vision/
│
├── train/
│   ├── healthy/
│   └── Cercospora/
│
├── validation/
│   ├── healthy/
│   └── Cercospora/
│
└── test/
    ├── healthy/
    └── Cercospora/
```

Each class is stored in its own folder, allowing TensorFlow/Keras to automatically assign labels during model training.

---

# 📂 Directory Structure

```text
Lab_07/
│
├── Lab_7_22jzele0480.ipynb
├── Computer vision/
├── Corn/
│
└── README.md
```



---

### Install Required Packages

```bash
pip install numpy tensorflow keras
```

---

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Run the notebook to automatically organize the image dataset into training, validation, and testing folders.

---

# 📌 Skills Developed

- Image Dataset Preparation
- Python File Handling
- Directory Management
- Dataset Organization
- Folder-Based Image Labeling
- Computer Vision Data Preparation
- TensorFlow/Keras Dataset Formatting
- Automated Data Processing

---

# 🌍 Practical Applications

The dataset preparation techniques demonstrated in this laboratory are widely used in:

- 🌿 Plant Disease Detection
- 🏥 Medical Image Analysis
- 🚗 Object Recognition
- 🏭 Industrial Quality Inspection
- 🌾 Smart Agriculture
- 📷 Image Classification Systems
- 🤖 Computer Vision Applications
- 🔬 Deep Learning Research

---

# 📈 Dataset Preparation Workflow

```text
Raw Image Dataset
        │
        ▼
Class Identification
        │
        ▼
Create Folder Structure
        │
        ▼
Train / Validation / Test Split
        │
        ▼
Copy Images into Class Folders
        │
        ▼
CNN-Ready Dataset
```

---

# 🎓 Course Information

| Item | Details |
|------|---------|
| Course | Machine Learning Laboratory |
| Lab | Lab 07 |
| Topic | Computer Vision Dataset Preparation |
| Institution | UET Peshawar – Nowshera Campus |

---

# 👨‍💻 Author

**IBRAAHEEM KHAN**

**Registration Number:** 22JZELE0480

**Department:** Electrical Engineering

**Course:** Machine Learning Laboratory

**Supervisor:** Engr. Irshad Ullah

**Institution:** University of Engineering & Technology (UET) Peshawar – Nowshera Campus

---

# 📄 Academic Note

This laboratory was completed as part of the **Machine Learning Laboratory** course to develop practical skills in organizing image datasets for deep learning applications. The prepared dataset provides the foundation for training and evaluating Convolutional Neural Networks (CNNs) in the subsequent laboratory.

---

# 📜 License

This project is intended for **educational and research purposes**.

You are welcome to use, modify, and extend the material for academic learning while providing appropriate credit to the original author.

---

## ⭐ Support

If you found this laboratory helpful, consider giving the repository a **Star ⭐** on GitHub.
