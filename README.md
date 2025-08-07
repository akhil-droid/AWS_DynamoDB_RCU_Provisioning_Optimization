# DynamoDB RCU Provisioning Optimization

This project builds a machine learning pipeline to predict and classify the provisioning status of AWS DynamoDB Read Capacity Units (RCUs) based on historical usage data and engineered features. The model helps identify over-provisioned, under-provisioned, and balanced states to **optimize cloud infrastructure cost and performance**.

---

## 🚀 Features

- Reads and processes time-series DynamoDB usage data
- Extracts time-based and statistical features (hour, day of week, growth rate, etc.)
- Classifies provisioning status using a Random Forest Classifier
- Visualizes RCU usage trends and provisioning accuracy
- Detects over- and under-provisioning cases

---

## 🧰 Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📊 Dataset

The dataset includes hourly records of:
- `Timestamp`
- `ConsumedRCU`
- `ProvisionedRCU`
- `TargetUtilization(TG)`
- `ActualUtilization`
- `ProvisioningStatus`

---

## 🧠 Model Training

The model is trained to predict `ProvisioningStatus` (encoded as:
- 0: Over-Provisioned
- 1: Balanced
- 2: Under-Provisioned

A Random Forest Classifier is used, evaluated with a classification report and confusion matrix.

---

## 📈 Sample Outputs

- Feature importance rankings
- Confusion matrix heatmap
- Provisioning accuracy across time

---

## 📂 How to Run

1. Clone the repo  
2. Ensure `dynamodb_rcu_raw_dataset.csv` is present  
3. Open `dynamodb_rcu_full_pipeline_final.ipynb`  
4. Run the notebook step-by-step  

---

## ✅ Future Improvements

- Incorporate real-time data streaming
- Use XGBoost or time-series models
- Deploy as a monitoring dashboard

---

## 📬 Contact

For any questions or collaborations, feel free to reach out!
