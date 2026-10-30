# Reliance Industries Stock Market EDA (2021–2024)

An Exploratory Data Analysis (EDA) project analyzing daily trading metrics for Reliance Industries stock data collected over a three-year period (741 trading sessions). This repository contains Phase 1 deliverables focused on data understanding, schema validation, quality remediation, and trend evaluation.

---

## 📊 Project Overview

The objective of this project is to perform end-to-end exploratory data analysis on historical stock market trends for Reliance Industries. 

* **Dataset Scope:** 2021 – 2024
* **Total Trading Days:** 741 records
* **Initial Features:** Date, Open, High, Low, Close, Volume
* **Target Analysis:** Price distribution, volume spikes, and day-over-day market directional trends.

---

## 🧹 Key Findings & Data Quality Enhancements (Phase 1)

1. **Schema & Null Value Remediation:**
   * Detected and resolved **1 missing record** in the `Date` feature using `df.dropna(subset=['Date'])`.
   * Standardized all continuous stock metrics (`Close`, `High`, `Low`, `Open`) from object strings to `float64` using `pd.to_numeric(..., errors='coerce')`.

2. **Summary Statistics:**
   * **Mean Closing Price:** ₹1,096.54
   * **52-Week/Period Price Range:** ₹831.35 (Min) to ₹1,291.32 (Max)
   * **Daily Volume Average:** ~15.1 million shares traded daily (Peak volume: 91.46M shares).

3. **Categorical Trend Breakdown:**
   * Engineeered a custom categorical `Trend` feature comparing daily `Close` vs. `Open`.
   * **Down Days (Bearish):** 374 days (50.5%)
   * **Up Days (Bullish):** 367 days (49.5%)

---

## 📁 Repository Structure

```text
Reliance-Stock-EDA/
├── .gitignore              # Ignores Jupyter checkpoints and virtual environments
├── README.md               # Project documentation and summary report
├── stock-market_EDA.ipynb  # Primary Jupyter notebook with code and findings
└── stock_data.csv          # Cleaned historical stock dataset
🚀 How to Run Locally
Clone the repository:

Bash
git clone [https://github.com/yaqoobkhangtr-ux/Reliance-Stock-EDA.git](https://github.com/yaqoobkhangtr-ux/Reliance-Stock-EDA.git)
cd Reliance-Stock-EDA
Install dependencies:

Bash
pip install pandas numpy jupyter
Launch Jupyter Notebook:

Bash
jupyter notebook stock-market_EDA.ipynb
👤 Author
Developer: Yaqoob Khan

GitHub: @yaqoobkhangtr-ux

Program: Data Science & Analytics (Innomatics Research Labs)


---

### Step-by-Step Commands to Push `README.md`

Open your **PowerShell** window and run these three commands:

1. **Stage the new README file:**
   ```powershell
   git add README.md
Save the commit:

PowerShell
git commit -m "Add professional README documentation for Phase 1"
Push to GitHub:

PowerShell
git push origin main
Refresh your repository page at [https://github.com/yaqoobkhangtr-ux/Reliance-Stock-EDA](https://github.com/yaqoobkhangtr-ux/Reliance-Stock-EDA)
