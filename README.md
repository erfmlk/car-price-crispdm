# Car Price Prediction Using CRISP-DM
# car-price-crispdm
**Project for Assignment 11.1: What Drives the Price of a Car?**

_Second Practical Application Assignment_ 

Course: **Professional Certificate in Machine Learning and Artificial Intelligence by Berkeley**  

**By: Erfan Maleki**

---

## Overview
This project analyzes used car listings to predict vehicle prices based on technical specifications and categorical features. The work follows the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) framework to guide the project lifecycle from business understanding to deployment.

---

## Objective
To develop a robust machine learning pipeline that:
- Accurately predicts used car prices
- Identifies the most influential factors driving price
- Provides actionable recommendations for stakeholders (e.g., dealers, platforms)

---

## Dataset Details
**Source:** Craigslist Vehicle Listings – [UCI Repository]  
**File Used:** `vehicles.csv` (located inside the ZIP file `practical_application_II_starter.zip`)

### Main Fields:
- `year`: Model year of the vehicle  
- `odometer`: Vehicle mileage  
- `cylinders`: Engine cylinder count  
- `manufacturer`, `model`, `fuel`, `transmission`, `drive`, `type`, etc.  
- `price`: Target variable (cleaned for outliers and invalid entries)

---

## Tools & Libraries
- **Python**  
- **pandas**, **numpy** – Data manipulation  
- **matplotlib**, **seaborn** – Visualizations  
- **scikit-learn** – Modeling pipeline  
- **joblib** – Exporting trained models  
- **Jupyter Notebook** – Interactive development

---

## Key Insights from Analysis
- **Newer vehicles** and **lower mileage** strongly correlate with higher prices.
- **Automatic transmissions** and **electric/diesel vehicles** are priced higher.
- Brands like **BMW**, **Lexus**, and **Mercedes-Benz** retain value better.
- Vehicle types like **SUVs** and **sedans** offer more predictable resale values.

---

## Final Model
- **Model Used:** Random Forest Regressor  
- **Evaluation Metric:** RMSE ~ **$2,200** on test set  
- **Deployment:** Model exported via `joblib` for reuse in pricing tools.

---

## Repository Structure

| File / Folder                      | Description                                         |
|-----------------------------------|-----------------------------------------------------|
| `Car_Price_Analysis.ipynb`        | Jupyter Notebook with full CRISP-DM workflow        |
| `Car_Price_Analysis.docx`         | Written project report summarizing findings         |
| `practical_application_II_starter.zip` | Contains dataset, starter files, and images    |
| `readings_starter.zip`            | PDF references for CRISP-DM methodology             |
| `LICENSE`                         | Project license                                     |
| `README.md`                       | This project summary and usage guide                |

---

## How to Run

1. **Clone the repository**:
```bash
git clone https://github.com/erfmlk/car-price-crispdm.git
cd car-price-crispdm
