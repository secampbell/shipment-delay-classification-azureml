# Predicting Shipment Delays with Azure ML

This project uses Microsoft Azure Machine Learning Studio to classify whether a shipment was significantly delayed based on various features.

## 📁 Dataset
- **Source:** Fabricated (using Tonic Fabricate)
- **File:** `shipments_significant_delay_2025.csv`
- **Target column:** `is_significantly_delayed` (1 = delayed 7+ days)

## 🔍 Goal
Train a model to predict if a shipment will be significantly delayed using features like:
- Carrier
- Shipping Method
- Estimated vs. Actual Delivery Dates
- Delay in Days

## ⚙️ Model Summary
- **Tool:** Azure AutoML
- **Model:** LightGBM with MaxAbsScaler
- **AUC (Weighted):** 1.0000 (note: synthetic dataset)
- **Runtime:** 19 minutes

## 🧠 Notes
The high performance is likely due to consistent patterns in the synthetic data. Real-world behavior may produce more nuanced results.

## 📸 Screenshots
- Dataset config
- AutoML setup
- Final model results

## 🛠️ Next Steps
- Add real-world noise to simulate imperfect data
- Use regression to predict exact delay duration
- Try SHAP to explain feature importance
