# Car Price Prediction Using CRISP-DM
# car-price-crispdm
**Project for Assignment 11.1: What Drives the Price of a Car?**

_Second Practical Application Assignment_ 

Course: **Professional Certificate in Machine Learning and Artificial Intelligence by Berkeley**  

**By: Erfan Maleki**

---

## Overview

This project analyzes used car listings to predict vehicle prices based on technical specifications and categorical features. The project follows the CRISP-DM framework to structure the workflow from business understanding to deployment.

---

## Objective

The goal is to develop a robust machine learning pipeline that accurately predicts used car prices and identifies key value-driving factors.

---

## Dataset Details

Dataset Source: [Craigslist Vehicle Listings Dataset – UCI]  
Main fields used:
- `year`: Model year of the vehicle
- `odometer`: Mileage
- `cylinders`: Engine cylinders
- `manufacturer`, `model`, `fuel`, `transmission`, `drive`, `type`, etc.
- `price`: Target variable (filtered for outliers and cleaned)

---

## Tools & Libraries

- **Python**
- `pandas` & `numpy` – Data handling  
- `scikit-learn` – Machine learning pipeline  
- `matplotlib` & `seaborn` – Visualizations  
- `joblib` – Model export  
- `Jupyter Notebook` – Interactive analysis

---

## Key Insights

- Car **year**, **odometer**, **manufacturer**, and **drive type** are among the most influential features.
- Some luxury brands like Lexus, BMW, and Mercedes retain higher resale values.
- Vehicles with automatic transmission and newer model years tend to have higher prices.

---

## Final Model

- Model: **Random Forest Regressor**
- Evaluation: RMSE on test set: ~$2,200  
- Deployment-ready pipeline saved using `joblib`.

---

## Repository Structure

| File / Folder | Description |
|---------------|-------------|
| `notebooks/car_price_crispdm.ipynb` | Full CRISP-DM workflow in notebook |
| `data/vehicles.csv` | Cleaned dataset |
| `models/champion_pipeline.joblib` | Trained ML pipeline |
| `figures/top_features.png` | Feature importance bar chart |
| `requirements.txt` | Python dependencies |
| `README.md` | Project description |

---

## ▶ How to Run

1. Clone this repository:
```bash
git clone https://github.com/erfmlk/car-price-crispdm.git
cd car-price-crispdm
