# Hertzsprung-Russell-Diagram-Visualization

# 🌌 Stellar Classification & Hertzsprung–Russell Diagram Using Machine Learning

## 📘 Project Overview

This project aims to automate the classification of stars using machine learning, while also visualizing stellar properties through a scientifically structured **Hertzsprung–Russell (H-R) diagram**. The approach blends **astrophysics** with **data science**, leveraging real-world astronomical data and the power of the **Random Forest algorithm** for accurate classification based on physical attributes like:

- Luminosity  
- Magnitude (Apparent & Absolute)  
- Spectral Class  
- Color Index

---

## 🎯 Objectives

1. Develop a classification model for stars based on physical properties.
2. Pre-process and cleanse a large-scale astronomical dataset.
3. Evaluate classification performance using standard ML metrics.
4. Construct a Hertzsprung–Russell diagram from the dataset.
5. Provide insights into the evolutionary stages of stars.

---

## 🧠 Background & Significance

In astrophysics, stars are traditionally classified based on characteristics such as **temperature**, **brightness**, and **spectral features**. The **Hertzsprung–Russell diagram** plays a pivotal role in visualizing these traits, revealing patterns in stellar evolution.

However, manual classification of stars from massive datasets is inefficient and prone to inconsistencies. This project introduces a **machine learning-based alternative** — enabling scalable, consistent, and accurate classification, backed by visual analytics.

---

## 📊 Dataset

- **Source:** [The Astronomy Nexus](https://www.astronexus.com/)
- **Size:** 100,000+ stellar entries
- **Features Used:**
  - `Apparent Magnitude`: Brightness as seen from Earth
  - `Absolute Magnitude`: Intrinsic brightness at 10 parsecs
  - `Luminosity`: Energy output per unit time
  - `Color Index (B−V)`: Numerical indicator of color and temperature
  - `Spectral Class`: Stellar classification category (e.g., O, B, A, F, G, K, M)

---

## ⚙️ Methodology

### 1. Pre-processing

- **Missing Values:** Removed rows with NaN or invalid entries.
- **Standardization:** Normalized numerical columns (e.g., magnitude, color index).
- **Categorical Cleaning:** Ensured uniformity in spectral class labels (e.g., all uppercase).

### 2. Model Training

- **Algorithm Used:** Random Forest Classifier (via scikit-learn)
- **Train/Test Split:** 80:20 ratio using stratified sampling to maintain spectral class distribution.
- **Evaluation Metrics:**
  - Accuracy
  - Precision / Recall / F1 Score
  - Confusion Matrix
  - Macro & Weighted Averages

### 3. H-R Diagram Construction

- **Plot Type:** Scatter Plot
- **Axes:**
  - X-axis: `Color Index` or `Spectral Class` (Temperature Proxy)
  - Y-axis: `Luminosity` or `Absolute Magnitude`
- **Color Coding:** Based on classification labels

---

## ✅ Results

### 🔍 Classification Performance

- **Model Accuracy:** `100%`
- **Confusion Matrix:** Demonstrated perfect classification across all classes
- **Interpretation:** The Random Forest classifier was able to fully capture the relationships between stellar attributes and their classifications.

### 🌠 H-R Diagram

- Constructed successfully with clear grouping of **Main Sequence**, **Giants**, and **White Dwarfs**.
- Demonstrated expected patterns — such as inverse relation between temperature and magnitude.

---

## 🔮 Future Improvements

- Integrate **Deep Learning** models (e.g., neural networks) for more generalized performance.
- Add more features like:
  - Stellar **age**
  - **Metallicity**
  - **Radial velocity**
- Expand to cover **multi-class celestial object classification**.
- Improve visual analytics with **interactive plots** (e.g., Plotly, Dash).

---

## 🧾 Technologies Used

| Tool/Library     | Purpose                              |
|------------------|--------------------------------------|
| Python           | Programming Language                 |
| Scikit-learn     | Machine Learning                     |
| Pandas / NumPy   | Data Processing                      |
| Matplotlib       | Data Visualization (H-R Diagram)     |
| Jupyter Notebook | Interactive Development Environment  |

---
