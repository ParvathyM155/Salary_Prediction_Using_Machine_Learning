<div align="center">

# 💰 Salary Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3+-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=for-the-badge&logo=pandas&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

> A machine learning pipeline that predicts whether a person's income exceeds $50K/year using the UCI Adult Census dataset, featuring multi-model benchmarking, hyperparameter tuning, and comprehensive evaluation.

[Overview](#-overview) • [Features](#-features) • [Results](#-results) • [Installation](#-installation) • [Usage](#-usage) • [Project Structure](#-project-structure)

</div>

---

## 📌 Overview

This project builds an end-to-end ML pipeline to classify individuals into `<=50K` or `>50K` salary brackets based on demographic features from the **UCI Adult Census Income** dataset. The pipeline handles preprocessing, model comparison, hyperparameter optimization, and evaluation — all within a single reproducible workflow.

## ✨ Features

- **Leak-Free Pipeline** — `ColumnTransformer` inside `Pipeline` ensures no data leakage between train/test splits
- **Multi-Model Benchmarking** — Compares Decision Tree, Random Forest, Gradient Boosting & Logistic Regression
- **Hyperparameter Tuning** — `GridSearchCV` with cross-validation for optimal model selection
- **Comprehensive Evaluation** — Accuracy, Precision, Recall, F1-Score, ROC-AUC, Confusion Matrix
- **Feature Importance Analysis** — Identifies key predictors driving salary classification
- **Model Serialization** — Saves trained model with `joblib` for deployment readiness

## 📊 Results

| Model | Accuracy | F1-Score | ROC-AUC |
|-------|----------|----------|---------|
| Decision Tree | ~83% | ~0.83 | ~0.82 |
| Random Forest | ~86% | ~0.85 | ~0.90 |
| **Gradient Boosting** | **~87%** | **~0.86** | **~0.92** |
| Logistic Regression | ~85% | ~0.84 | ~0.90 |

> *Replace with your actual results after running the notebook.*

### Evaluation Plots

<p align="center">
  <img src="assets/confusion_matrix.png" width="45%" alt="Confusion Matrix"/>
  <img src="assets/roc_curve.png" width="45%" alt="ROC Curve"/>
</p>
<p align="center">
  <img src="assets/feature_importance.png" width="60%" alt="Feature Importance"/>
</p>

> *Add your saved plots to the `/assets` folder.*

## 🛠 Installation

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/salary-prediction-ml.git
cd salary-prediction-ml

# Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## 🚀 Usage

```bash
# Run the notebook
jupyter notebook salary_prediction.ipynb
```

Or run as a script:
```bash
python salary_prediction.py
```

## 📁 Project Structure

```
salary-prediction-ml/
├── salary_prediction.ipynb   # Main notebook with full pipeline
├── requirements.txt          # Python dependencies
├── salary_model.pkl          # Saved trained model (generated after run)
├── assets/                   # Evaluation plots & visuals
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── feature_importance.png
├── LICENSE                   # MIT License
└── README.md                 # Project documentation
```

## 📋 Requirements

```
pandas>=2.0
numpy>=1.24
scikit-learn>=1.3
matplotlib>=3.7
seaborn>=0.12
joblib>=1.3
```

## 🔮 Future Enhancements

- [ ] Add SMOTE for handling class imbalance
- [ ] Deploy model as REST API using Flask/FastAPI
- [ ] Build interactive prediction UI with Streamlit
- [ ] Add XGBoost and LightGBM to model comparison
- [ ] Implement SHAP values for model explainability

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -m 'feat: add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/adult) — Adult Census Income Dataset
- [scikit-learn](https://scikit-learn.org/) — Machine Learning Library

---

<div align="center">
  <b>⭐ Star this repo if you found it useful!</b>
</div>
