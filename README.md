# Walmart Demand Forecasting using OCI

## Project Overview
This project demonstrates an end-to-end demand forecasting workflow using historical Walmart store sales data. The objective is to build, evaluate, and improve machine learning models that can support inventory planning and retail supply chain decision-making.

This project aligns with my OCI certifications:
- Oracle Cloud Infrastructure (OCI) AI Foundations
- OCI Generative AI Professional
- OCI Multicloud Architect Professional

## Business Problem
Retail organizations must accurately forecast product demand in order to:
- Reduce stockouts
- Minimize overstock and excess inventory
- Improve supply chain efficiency
- Increase revenue and customer satisfaction

This project explores how machine learning models can predict weekly sales at the store level using historical and contextual features.

## Dataset
**Source:** Public Walmart Store Sales dataset

**Key features include:**
- Store identifier
- Weekly sales
- Holiday indicator
- Economic and environmental variables (CPI, unemployment, fuel price, temperature)
- Date (time-series context)

## Methodology
1. Data loading and exploratory analysis  
2. Time-aware data preparation to prevent leakage  
3. Baseline model development (Linear Regression)  
4. Advanced modeling using Random Forest  
5. Feature engineering to improve predictive performance  
6. Model evaluation using MAE and RMSE  

## Results
| Model | MAE | RMSE |
|------|-----|------|
| Linear Regression | ~75,856 | ~107,829 |
| Random Forest | ~92,574 | ~133,009 |
| Random Forest + Feature Engineering | ~78,934 | ~112,503 |

**Key takeaway:**  
Feature engineering significantly improved model performance and reduced forecast error, demonstrating how domain-aware data preparation can meaningfully impact retail demand prediction.

## Tools & Technologies I Used
- Python  
- pandas, numpy  
- scikit-learn  
- matplotlib  
- Oracle Cloud Infrastructure (OCI)

## Project Structure
- `Walmart_demand_forecasting_baseline.ipynb` – End-to-end ML workflow
- `AI_Driven_Supply_Chain_Demand_Forecasting_OCI.ipynb` - OCI architecture and setup  
- `Walmart_store_sales.csv` – Dataset  
- `requirements.txt` – Python dependencies  
- `.gitignore` – Version control exclusions  

## How to Run (Optional)
```bash
git clone https://github.com/Mariam-Said1/oci-walmart-demand-forecasting.git
cd oci-walmart-demand-forecasting
pip install -r requirements.txt
jupyter notebook Walmart_demand_forecasting_baseline.ipynb
