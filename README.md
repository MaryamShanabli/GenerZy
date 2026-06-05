# ⚡ GenerZy · MotionSense AI Project

<div align="center">

[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/spaces/maryamshanabli/GenerZy)
[![Streamlit App](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://huggingface.co/spaces/maryamshanabli/GenerZy)
[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)]()

> **Every video game has an energy bar — why shouldn't your life have one**

> 🏆 **1st Place Winner at the MotionSense AI Competition**

[🕹️ Launch Live Telemetry Demo on Hugging Face Spaces](https://huggingface.co/spaces/maryamshanabli/GenerZy)

</div>

---

## 🚀 Project Overview

GenerZy is an intelligent telemetry dashboard that transforms continuous smartphone and wearable sensor data into a live player energy matrix. By deploying optimized machine learning architectures, the system categorizes human movement patterns in real-time to gamify healthy habit loops and prevent prolonged physical stagnation.

### 🛰️ Core Architecture

- **Signal Feature Extraction:** Processes high-dimensional coordinate vectors from wearable biometric hardware
- **Gradient Boosting Tree Matrix:** Executes instantaneous classification routines across trained multi-class boundaries
- **Immersive Interface:** Built natively with Streamlit using custom cyber-grid stylistic configurations

---

## 📂 Repository Structure

```
MotionSense_Project/
│
├── data/
│   ├── train_data_ready.csv
│   ├── test_data_ready.csv
│   ├── X_train_sel.npy
│   ├── X_val_sel.npy
│   ├── X_test_sel.npy
│   ├── y_train_app.npy
│   ├── y_val_app.npy
│   ├── y_test_app.npy
│   └── final_features.csv
│
├── model/
│   ├── best_gradient_boosting_model.joblib
│   └── robust_scaler_final.joblib
│
├── notebooks/
│   └── MotionSense_Project.ipynb
│
├── app/
│   └── app.py
│
├── requirements.txt
└── README.md
```

---

## 🛠️ Setup

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/<repository-name>.git
cd <repository-name>
```

### 2. Create a Virtual Environment

```bash
# Linux / macOS
python -m venv venv
source venv/bin/activate

# Windows
python -m venv venv
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🎮 Running the Project

### Jupyter Notebook

```bash
jupyter notebook notebooks/MotionSense_Project.ipynb
```

### Streamlit App (Local)

```bash
streamlit run app/app.py
```

---

## 🔬 Model Specifications

The classifier is an optimized **Gradient Boosting Classifier** reaching near-perfect validation accuracy.

| Metric | Value |
| --- | --- |
| **Validation Accuracy** | `0.9946` |
| **Test Accuracy** | `0.9647` |

```json
{
    "n_estimators": 500,
    "learning_rate": 0.2,
    "max_depth": 4,
    "subsample": 0.8,
    "min_samples_split": 5
}
```

---

## 📊 Top 10 Features by Importance

```
1   tBodyGyroJerk-std()-Y
2   tGravityAcc-arCoeff()-Y,3
3   fBodyAccJerk-entropy()-X
4   fBodyAcc-bandsEnergy()-1,24.1
5   tGravityAcc-mean()-Z
6   tBodyGyroJerk-min()-X
7   fBodyAcc-bandsEnergy()-1,24
8   tBodyAccJerk-std()-X
9   tBodyGyroJerk-mad()-Z
10  angle(X,gravityMean)
```

---

## 🌐 Deployment

- Live demo hosted on [Hugging Face Spaces](https://huggingface.co/spaces/maryamshanabli/GenerZy)
- Input features are automatically normalized via a Robust Scaler before classification
