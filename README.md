# Smart Banking Fraud Detection System

## 1. Project Overview

The **Smart Banking Fraud Detection System** is a machine learning-based application designed to identify potentially fraudulent financial transactions.

The application analyzes transaction details and uses machine learning models to estimate fraud risk. It provides a simple interactive dashboard where users can enter transaction information and view the risk assessment.

## 2. Problem Statement

Financial fraud is a major challenge in digital banking. Suspicious transactions need to be identified quickly to reduce potential financial losses.

This project aims to support fraud detection by analyzing transaction patterns and identifying potentially risky activities using machine learning techniques.

## 3. Objectives

- Analyze financial transaction details.
- Identify potentially suspicious transactions.
- Generate a transaction risk score.
- Display fraud detection results through an interactive dashboard.
- Provide understandable reasons for flagged transactions where available.

## 4. Technologies Used

| Technology | Purpose |
|---|---|
| Python | Application development |
| Streamlit | Interactive web dashboard |
| Scikit-learn | Machine learning and preprocessing |
| XGBoost | Fraud classification |
| Random Forest | Fraud classification |
| Isolation Forest | Anomaly detection |
| NumPy | Numerical operations |
| Pandas | Data handling |

## 5. Key Features

- Interactive transaction input dashboard.
- Machine learning-based fraud risk assessment.
- Combination of multiple model outputs.
- Transaction risk score generation.
- Risk category display.
- Explanation of suspicious transaction indicators.

## 6. Machine Learning Models

The project uses the following trained model files:

- `rf_model.pkl` – Random Forest model.
- `xgb_model.pkl` – XGBoost model.
- `iso_model.pkl` – Isolation Forest model.
- `scaler.pkl` – Feature scaling.
- `type_encoder.pkl` – Transaction type encoding.

The application combines model outputs and additional rule-based checks to calculate a transaction risk score.

## 7. Project Structure

```text
Smart-Banking-Fraud-Detection/
│
├── AI-Powered-Fraud-Detection-System/
│   ├── app.py
│   ├── requirements.txt
│   ├── README.md
│   ├── Report.docx
│   ├── rf_model.pkl
│   ├── xgb_model.pkl
│   ├── iso_model.pkl
│   ├── scaler.pkl
│   └── type_encoder.pkl
│
└── .gitignore
```

## 8. Installation and Setup

### Step 1: Clone the repository

```bash
git clone https://github.com/kotamadhavi40-glitch/Smart-banking-fraud-detection.git
```

### Step 2: Open the project folder

```bash
cd Smart-banking-fraud-detection
cd AI-Powered-Fraud-Detection-System
```

### Step 3: Create a virtual environment

```bash
python -m venv .venv
```

### Step 4: Activate the virtual environment

Windows:

```bash
.venv\Scripts\activate
```

### Step 5: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 6: Run the application

```bash
python -m streamlit run app.py
```

The application will open in your browser at:

`http://localhost:8501`

## 9. Results

The application provides:

- Transaction risk assessment.
- Fraud risk score.
- Risk category.
- Indicators explaining why a transaction may be flagged.

Actual model performance metrics should be added after running a separate evaluation on the test dataset.

## 10. Current Limitations

- The current application uses a Streamlit-based interface.
- Real-time Kafka transaction streaming is not implemented.
- Fraud-ring detection using graph neural networks is not implemented.
- Model lifecycle tracking and deployment monitoring are future improvements.
- The current version is an initial machine learning-based prototype.

## 11. Future Enhancements

- Integrate Apache Kafka for real-time transaction streaming.
- Develop fraud-ring detection using PyTorch Geometric.
- Implement FastAPI for model serving.
- Integrate Feast for feature management.
- Use MLflow for experiment tracking.
- Add Evidently AI for model monitoring.
- Deploy the application using Kubernetes.

## 12. Conclusion

The Smart Banking Fraud Detection System demonstrates how machine learning techniques can support the identification of potentially fraudulent financial transactions.

This project provided practical experience in Python, machine learning models, data preprocessing, and Streamlit application development. It also provides a foundation for learning and implementing advanced fraud detection technologies.

---

**Project Name:** Smart Banking Fraud Detection System
