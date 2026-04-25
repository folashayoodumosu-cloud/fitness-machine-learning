# 🏋️ Fitness Tracker Machine Learning Project

## 📌 Overview

This project builds a machine learning system that **classifies barbell exercises and counts their repetitions** using wearable sensor data. It follows a complete data science pipeline, from raw data processing to model deployment.

The project is inspired by the **quantified self**concept, in which individuals track personal data to gain insights into their performance and behaviour.

---

## 🎯 Objectives

* Process accelerometer and gyroscope data
* Perform data cleaning and transformation
* Visualise time-series sensor data
* Engineer meaningful features
* Train and evaluate machine learning models
* Classify exercises and count repetitions

---

## 📊 Dataset

The dataset was collected during gym workouts from multiple participants performing various barbell exercises.

### Sensor Data

* **Accelerometer (x, y, z)** → measures linear motion (G-forces)
* **Gyroscope (x, y, z)** → measures rotational motion (degrees/second)

This data is similar to what is captured by modern **fitness trackers and smartwatches**.

---

## ⚙️ Project Pipeline

### 1. Data Processing

* Load and merge multiple CSV files
* Extract metadata (exercise, participant, intensity)
* Convert timestamps and resample data
* Structure data for supervised learning

---

### 2. Data Visualisation

* Plot time-series sensor data
* Compare exercises and participants
* Identify patterns in movement

---

### 3. Outlier Detection

* Interquartile Range (IQR)
* Chauvenet’s Criterion
* Local Outlier Factor (LOF)

Removes extreme or incorrect values to improve model quality.

---

### 4. Feature Engineering

* Low-pass filtering (noise reduction)
* Principal Component Analysis (PCA)
* Temporal features (rolling averages)
* Frequency features (Fourier Transform)
* Clustering

Transforms raw sensor data into meaningful inputs for models.

---

### 5. Machine Learning Models

Tested multiple models:

* Naive Bayes
* Support Vector Machine (SVM)
* Random Forest
* Neural Network

Includes:

* Feature selection
* Hyperparameter tuning (Grid Search)
* Model evaluation

---

### 6. Repetition Counting

* Applied signal smoothing
* Detected peaks in motion data
* Counted repetitions using a custom algorithm

---

## 🧠 Key Concepts

* Supervised Learning
* Time-Series Analysis
* Signal Processing
* Feature Engineering
* Model Optimisation

---

## 🚀 Results

* Successfully classified barbell exercises
* Built a working repetition counting system
* Demonstrated how wearable sensor data can be used for fitness tracking

---

## 📁 Project Structure

```
data/
  raw/
  processed/
src/
  data/
  features/
  models/
notebooks/
```

---

## 🛠️ Tools & Technologies

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

---

## 📚 Inspiration

Based on work from the *Machine Learning for the Quantified Self* course.

"The quantified self is any individual engaged in the self-tracking of any kind of biological, physical, behavioural, or environmental information. The self-tracking is driven by a certain goal of the individual, with a desire to act upon the collected information." — Hoogendoorn, M., & Funk, B. (2018)

---

## 📌 Conclusion

This project shows how raw motion sensor data can be transformed into a practical machine learning application for fitness tracking, similar to modern wearable devices.

---

