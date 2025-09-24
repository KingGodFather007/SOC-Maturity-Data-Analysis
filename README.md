# SOC-Maturity-Analysis  

This repository contains a comprehensive Python pipeline for **SOC (Security Operations Center) Maturity Analysis**.  
The project demonstrates data preprocessing, correlation analysis, regression modeling, and standardized beta estimation to evaluate the relationships between SOC capabilities and operational performance metrics.  

---

## 🚀 Features  

* **Data Preprocessing**:  
  * Loads data from Excel spreadsheets  
  * Applies log-transformations on time-based metrics (MTTD, MTTR, MTTC)  

* **Correlation Analysis**:  
  * Computes Pearson correlation coefficients (*r*)  
  * Generates *p*-value significance matrix  

* **Regression Modeling**:  
  * OLS regression (unstandardized coefficients) with `statsmodels`  
  * Standardized beta coefficients using `scikit-learn`  

* **Comprehensive Outputs**:  
  * Correlation matrix with significance testing  
  * Detailed OLS regression summary  
  * Standardized beta weights (β)  

* **Extensible Framework**:  
  * Can be adapted to additional maturity dimensions and performance indicators  

---

## 📂 Project Structure  


```
SOC-Maturity-Analysis/
│── SOC_analysis.py # Main analysis script
│── Synthesised data.xlsx # Input dataset (not included in repo)
│── README.md # Project documentation
```

---

## 🛠️ Requirements  

Install dependencies with:  

```
pip install pandas numpy scipy statsmodels scikit-learn openpyxl
```

## ▶️ Usage
* Clone the repository:
```
git clone https://github.com/yourusername/SOC-Maturity-Analysis.git
cd SOC-Maturity-Analysis

```

* Place your dataset (Synthesised data.xlsx) in the project root directory.
* Run the analysis:
```
python SOC_analysis.py
```
