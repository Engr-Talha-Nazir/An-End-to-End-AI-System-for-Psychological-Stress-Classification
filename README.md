
# 🧠 Stress Prediction Using Machine Learning
**An End-to-End AI System for Psychological Stress Classification**

---

## 📌 Project Overview

This project presents a complete machine learning pipeline for predicting human stress levels based on biometric indicators. By leveraging the **[SWELL-KW dataset](https://cs.ru.nl/~skoldijk/SWELL-KW/Dataset.html)**, we classify stress into multiple intensity levels using various supervised learning algorithms and provide a user-friendly GUI interface for practical application.

The system is designed to assist researchers, mental health professionals, and work-environment analysts in identifying psychological stress based on physiological data such as heart rate variability and derived behavioral features.

---

## 🧬 Dataset: SWELL Knowledge Work (SWELL-KW)

The [SWELL-KW dataset](https://cs.ru.nl/~skoldijk/SWELL-KW/Dataset.html) was created to support research on stress, context awareness, and user modeling. It contains multimodal recordings from **25 participants** performing typical office tasks under three different stress conditions:

- Neutral
- Email interruptions
- Time pressure

### 🧪 Data Includes:
- Heart rate (BPM, variability)
- Stress balance and response indicators
- Mouse and keyboard logs
- Facial expression metrics (AU, emotion scores)
- Kinect body posture data
- Skin conductance
- Subjective stress, mental effort, and emotion scores (via validated questionnaires)

> 📚 Citation:
> Koldijk, S. et al., *The SWELL Knowledge Work Dataset for Stress and User Modeling Research*, ACM ICMI 2014

---

## 🧠 Models Used & Evaluation

Seven different classification algorithms were applied and compared:

| 🔢 Algorithm                     | ✅ Accuracy |
|----------------------------------|-------------|
| Logistic Regression              | 57.8%       |
| Random Forest                    | **100.0%**  |
| Decision Tree                    | 99.8%       |
| K-Nearest Neighbors (KNN)        | 97.2%       |
| Naive Bayes                      | 55.3%       |
| Linear Discriminant Analysis     | 60.6%       |
| Gradient Boosting Classifier     | 84.2%       |

Evaluated on:
- Precision, Recall, F1-score
- Confusion Matrix
- Weighted and macro averages

---

## 🧩 Features Used for Prediction
- Average Heart Rate (BPM)
- Typical Heart Rate (BPM)
- Stress Balance Ratio
- Heart Rate Stability Score
- Adaptive Stress Indicator
- Stress Response Level
- Stress Response Percentage

---

## 🖥️ GUI Interface

A Tkinter-based user interface allows users to input health metrics and receive real-time stress predictions.

**Screenshot Example**  
![GUI Screenshot](screenshots/interface.png)

---

## 📂 Folder Structure

```
stress-prediction-ml/
├── data/                     # Cleaned dataset and raw input
├── models/                   # Trained model files
├── gui/                      # Tkinter GUI code
├── notebooks/                # Jupyter notebooks
├── outputs/                  # Charts and reports
├── stress_prediction.ipynb   # Main notebook
├── requirements.txt          # Project dependencies
└── README.md                 # Project documentation
```

---

## ⚙️ How to Run

### 📦 Install Dependencies
```bash
pip install -r requirements.txt
```

### 📊 Run Notebook
```bash
jupyter notebook stress_prediction.ipynb
```

### 🖥️ Launch GUI
```bash
python gui/stress_gui.py
```

---

## 📈 Results Summary

The **Random Forest** model achieved 100% accuracy, confirming its strong performance. Ensemble methods like **Gradient Boosting** also provided high accuracy and robust generalization.

---

## 📚 References

- [SWELL-KW Dataset Description](https://cs.ru.nl/~skoldijk/SWELL-KW/Dataset.html)
- Koldijk, S., et al. *The SWELL Knowledge Work Dataset for Stress and User Modeling Research*, ACM ICMI 2014.

---

## 👨‍💻 Author

**Engr. Talha Nazir**  
Machine Learning Engineer | AI Researcher  


