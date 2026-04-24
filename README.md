# 🧠 Signify Data Pipeline

This repository contains my contribution to the **Signify Project**, where I built a complete data preprocessing and feature engineering pipeline for sign language recognition.

---

## 📌 Project Overview

The goal of this pipeline is to transform raw sign language video data into a structured dataset suitable for machine learning models.

---

## ⚙️ Work Done

- Filtered WLASL dataset to extract relevant sign classes  
- Extracted video URLs from dataset metadata  
- Downloaded and cleaned video data (handled missing and unsupported formats)  
- Converted videos into frames using OpenCV  
- Extracted hand landmarks using MediaPipe  
- Converted frames into numerical feature vectors (1890 features per sample)  
- Generated labeled dataset for supervised learning  
- Validated dataset using Logistic Regression  

---

## 🧠 Feature Engineering

- Each frame → 21 landmarks × (x, y, z) = 63 features  
- Each video → 30 frames  
- Final feature vector → **1890 features per video**

---

## 📊 Output

- `dataset.npy` → Feature matrix (X)  
- `labels.npy` → Labels (y)  
- Dataset size → 25 samples, 9 classes  

---

## 🤖 Model Validation

A basic Logistic Regression model was used to validate the dataset.

**Accuracy:** ~20%  
(Low due to small dataset size, focus was on pipeline building)

---

## 🛠️ Tech Stack

- Python  
- NumPy  
- OpenCV  
- MediaPipe  
- Scikit-learn  

---

## 📁 Project Structure

Signify-Data-Pipeline/
│
├── scripts/
│ ├── filter_dataset.py
│ ├── extract_urls.py
│ ├── clean_videos.py
│ ├── extract_frames.py
│ ├── extract_landmarks.py
│ ├── train_model.py
│
├── README.md
├── requirements.txt



---

## 🚀 Key Learning

- Real-world data is messy and requires extensive cleaning  
- Feature engineering is crucial for ML performance  
- Small datasets significantly impact model accuracy  
- Building a complete pipeline is more important than just training a model  

---

## 💼 Contribution

This repository specifically highlights my work in:
**Data Collection, Data Cleaning, Feature Extraction, and Dataset Preparation**

---

## 🔗 Note

This is part of a larger team project (Signify). This repository focuses only on the data pipeline component.
