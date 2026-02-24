# 💸 Salary Prediction Using Machine Learning

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge\&logo=scikit-learn\&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge\&logo=pandas\&logoColor=white)

> **Predicting annual income brackets using Decision Tree Classifiers to identify key socioeconomic drivers.**

---

## 📖 Project Overview

This project implements a **Decision Tree-based classifier** to predict whether an employee's salary is above or below **$50K/year**.
By analyzing demographic and employment features like **age, education level, and working hours**, the model identifies patterns that distinguish high-income earners.

---

## 🎯 Key Objectives

* **Data Preprocessing**: Cleaning raw data and encoding categorical features like education level.
* **Model Training**: Implementing a Decision Tree Classifier to handle binary classification.
* **Performance Analysis**: Evaluating results using confusion matrices and classification metrics such as Precision, Recall, and F1-Score.

---

## 🚀 Key Features

* ✅ **Clean Pipeline** – Automated data cleaning and mapping for education categories such as BSc, MSc, and PhD.
* ✅ **Visualized Results** – Performance heatmaps and confusion matrices generated using Seaborn.
* ✅ **Interactive Logic** – Structured sample predictions based on age, education, and working hours.

---

## 📊 Dataset Insights

The model is trained on the **Adult Census Income Dataset**.
* **Source**: [Download Dataset](https://www.mediafire.com/file/z02ebrv02rqdgvq/adult_3.csv/file)
* **Features**: Age, Education, Occupation, Hours-per-week, and Marital Status.
* **Target**: Salary Category (`<=50K` or `>50K`).

---

## 📈 Methodology & Results

1. **Preprocessing**
   * Handled missing values
   * Mapped education strings into simplified numerical categories

2. **Splitting**
   * 80/20 Train-Test split for model validation

3. **Training**
   * Decision Tree model with `max_depth = 3` for interpretability

4. **Sample Predictions**

| Age | Education | Hours/Week | Prediction |
| --- | --------- | ---------- | ---------- |
| 25  | HS        | 40         | <=50K      |
| 35  | BSc       | 45         | >50K       |
| 55  | PhD       | 60         | >50K       |

---

## 🛠️ Tech Stack
* **Language**: Python 3.x
* **ML Libraries**: Scikit-learn, Pandas, NumPy
* **Visualization**: Matplotlib, Seaborn
* **Formatting**: Tabulate
* **Environment**: Google Colab / Jupyter Notebook

---

## 💻 How to Run

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/ParvathyM155/Salary_Prediction_Using_Machine_Learning.git
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Notebook
Open the notebook file:
```
Employee_Salary_Prediction.ipynb
```

Run it in your preferred environment (Jupyter, VS Code, or Google Colab).

---

## ✍️ Author

**Parvathy M**
