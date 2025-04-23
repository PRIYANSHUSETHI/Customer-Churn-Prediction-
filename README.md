# 📉 Customer Churn Prediction

This project aims to build a machine learning model that predicts whether a telecom customer will churn (i.e., stop using the service) based on their demographic and service usage data. Understanding churn behavior helps businesses proactively engage customers and reduce attrition rates.

---

## 🔍 Problem Statement

Customer retention is a major challenge for telecom companies. By identifying potential churners early, businesses can take proactive steps to improve customer satisfaction. This project uses real-world data to create a churn prediction model using classification algorithms.

---

## 📁 Dataset

The dataset used in this project is the **Telco Customer Churn** dataset available on Kaggle. It includes information such as:

- Customer demographics (gender, senior citizen status, etc.)
- Account information (tenure, contract type, etc.)
- Service details (internet service, online security, streaming services, etc.)
- Monthly and total charges
- Churn label (Yes/No)

---

## 🔧 Project Workflow

1. **Data Preprocessing**
   - Removed irrelevant columns like `customerID`
   - Converted `TotalCharges` to numeric
   - Handled missing and inconsistent data

2. **Exploratory Data Analysis**
   - Visualized distributions, outliers, and correlations
   - Analyzed churn patterns across various customer segments

3. **Feature Engineering**
   - Created new features like `TenureGroup`, `EngagementScore`, `AvgChargePerMonth`
   - Engineered interaction features for better model insight

4. **Data Encoding & Balancing**
   - Applied `LabelEncoder` to categorical features
   - Used SMOTE to balance the imbalanced target variable

5. **Model Building**
   - Trained and evaluated:
     - Decision Tree
     - Random Forest
     - XGBoost
   - Selected Random Forest based on accuracy

6. **Model Evaluation**
   - Accuracy, confusion matrix, classification report on test data
   - Feature importances and performance metrics

7. **Model Deployment**
   - Saved the trained model and encoders using `pickle`
   - Built a test pipeline to make predictions from new customer data

---

## 🧠 Technologies Used

- Python
- pandas, numpy
- scikit-learn
- imbalanced-learn (SMOTE)
- seaborn, matplotlib, plotly
- XGBoost
- pickle (for model persistence)

---

## 🚀 How to Run

1. Clone the repository
2. Install required libraries using `pip install -r requirements.txt`
3. Run the notebook or script file
4. Load `customer_churn_model.pkl` and `encoders.pkl` for making predictions

---

## 📊 Visualizations

The project includes insightful plots such as:
- Churn rate by tenure group
- Engagement score distribution
- Box plots of average charges by churn status
- Churn rate by service combinations (e.g., security + support)

---

## 📌 Results

- Best model: **Random Forest**
- Achieved high accuracy and robust classification performance
- Model can be integrated into dashboards or CRM tools for real-time churn prediction

---

## 📬 Contact

For questions or collaboration, feel free to reach out via [LinkedIn](https://www.linkedin.com/) or open an issue on this repo.

---

## 📄 License

This project is licensed under the MIT License.