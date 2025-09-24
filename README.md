SOC Maturity Data Analysis

This repository provides a Python workflow for analyzing SOC (Security Operations Center) maturity data.
It performs correlation analysis, regression modeling, and standardized beta estimation on synthesized SOC performance metrics.

📌 Features

Data Preprocessing

Loads data from an Excel file

Log-transforms time-based metrics (MTTD, MTTR, MTTC)

Correlation Analysis

Computes Pearson’s r correlation matrix

Provides corresponding p-values

Regression Analysis

Unstandardized OLS regression coefficients using statsmodels

Standardized Beta coefficients using scikit-learn

Outputs

Correlation matrix

Significance matrix (p-values)

Full OLS regression summary

Standardized regression betas

🛠️ Requirements

The project uses the following Python packages:

pip install pandas numpy scipy statsmodels scikit-learn openpyxl

📂 Project Structure
SOC-Maturity-Analysis/
│── SOC_analysis.py       # Main analysis script
│── Synthesised data.xlsx # Input dataset (not included in repo)
│── README.md             # Project documentation

▶️ Usage

Clone the repository:

git clone https://github.com/yourusername/SOC-Maturity-Analysis.git
cd SOC-Maturity-Analysis


Place your dataset (Synthesised data.xlsx) in the project root directory.

Run the script:

python SOC_analysis.py

📊 Example Outputs

Correlation Matrix (Pearson r):

            AAS  log_MTTD  log_MTTR  log_MTTC  FPR (%)
AAS        1.000    0.321    -0.214     0.198   -0.142
log_MTTD   0.321    1.000     0.453     0.375    0.210
...


Standardized Betas (β):

CTI          -0.317
Detection     0.502
Emulation    -0.128
Automation   -0.276
dtype: float64

📖 Notes

Replace Synthesised data.xlsx with your dataset.

Ensure column names in the Excel file match those used in the script.

The analysis framework is extensible to additional maturity or performance metrics.
