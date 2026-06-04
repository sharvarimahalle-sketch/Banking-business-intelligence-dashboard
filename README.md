# Banking business intelligence dashboard
> End-to-end data analytics project combining Python EDA with an interactive Power BI dashboard to analyse the financial behaviour of 2,913 banking customers across loans, deposits and account types.

---

## 📌 Overview

This project explores a banking customer dataset to uncover patterns in loan uptake, deposit behaviour, income segmentation and demographic distribution. The analysis was carried out in two stages — exploratory data analysis in Python, followed by an interactive multi-page dashboard built in Power BI.

---

## Dataset

| Property | Detail |
|----------|--------|
| **Source** | Banking customer records (excel) |
| **Rows** | ~2,913 customers |
| **Key Columns** | Estimated Income, Bank Loans, Bank Deposits, Saving Accounts, Checking Accounts, Business Lending, Nationality, Occupation, Gender, Loyalty Classification, Risk Weighting |

---

## Tools Used

| Tool | Purpose |
|------|---------|
| **Python** (Pandas, Seaborn, Matplotlib) | Data loading, EDA, feature engineering |
| **Jupyter Notebook** | Analysis environment |
| **Power BI** | Interactive dashboard |
| **DAX** | Custom measures and calculated columns |
| **Canva** | Custom dashboard background design |

---

##  Steps

### 1. Data Loading & Inspection
- Loaded CSV using Pandas
- Checked shape, data types, null values, and summary statistics

### 2. Feature Engineering
- Created `Income Band` column (Low / Medium / High) from `Estimated Income` 

### 3. Exploratory Data Analysis
- **Univariate Analysis** — distribution of all categorical and numerical columns
- **Bivariate Analysis** — categorical variables broken down by Nationality
- **Numerical Analysis** — histograms with KDE for 9 financial variables
- **Correlation Heatmap** — identified strong correlations between deposit, savings, and checking accounts

### 4. Power BI Dashboard
- Imported dataset into Power BI
- Designed custom background in **Canva**
- Added **DAX measures** (Total Loan, Total Deposit, etc.) and **calculated columns** (Income Band grouping)
- Inserted **navigation buttons** for seamless page switching
- Applied **slicers/filters** for Year, Gender, Banking Relationship, and Investment Advisor

---

## 📊 Dashboard Pages

| Page | Description |
|------|-------------|
| **Home** | KPI cards — Total Clients, Total Loan, Total Deposit, Checking Accounts, Saving Accounts, Business Lending |
| **Loan Analysis** | Loan breakdown by Banking Relationship, Income Band, Nationality, and Occupation |
| **Deposit Analysis** | Deposit breakdown by BR, Income Band, Nationality, and Occupation |
| **Summary** | Loan vs Deposit comparison across all dimensions + written Key Insights panel |

---

## Key Results

- **₹4.38bn** total loans | **₹3.77bn** total deposits across 2,913 clients
- **Medium income** customers drive **50%+** of both loan and deposit volume
- **Private Bank** segment holds the highest loan and deposit values
- **European** customers dominate all segments; Australian customers represent a clear growth opportunity
- **Checking accounts (₹963M)** significantly outpace savings accounts (₹699M) — customers use the bank for transactions, not saving
- **Web Developers** top the occupation-wise loan chart — signals opportunity for tech-professional products

---

## How to Run

### Python Notebook
```
# 1. Clone the repository
git clone https://github.com/your-username/Banking business intelligence dashboard.git

# 2. Install dependencies
pip install pandas matplotlib seaborn numpy

# 3. Open the notebook
jupyter notebook Banking.ipynb
```

### Power BI Dashboard
1. Open `Banking business intelligence dashboard.pbix` in **Power BI Desktop**
2. Ensure the source CSV path is correctly mapped under **Transform Data → Source**
3. Refresh the data and explore using the navigation buttons and filters

---

## Project Structure

```
Banking business intelligence dashboard/
│
├── EDA_Banking business intelligence dashboard.ipynb                   # Python EDA notebook
├── data_Banking.xlsx                                                   # Raw dataset
├── Banking business intelligence dashboard.pbix                        # Power BI dashboard file
├── Home.png, Loan Analysis.png, Deposit Analysis.png, Summary.png      # Screenshots of all 4 dashboard pages
└── README.md                                                           # Project documentation
```

---

## 👤 Author

**Sharvari Mahalle**  
[LinkedIn](www.linkedin.com/in/sharvarimahalle) 
