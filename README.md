# Loan Portfolio Risk Analysis

A reproducible, story-driven analysis of a loan portfolio: default rate measurement, risk segmentation, and key driver exploration.

# What it shows
- Clear EDA and business framing
- Clean notebook in `notebooks/`

## Project Structure
```
loan-portfolio-analysis/
├─ data/                      # Place your public dataset(s) here
├─ images/                    # Optional figures for README
├─ notebooks/
│  └─ loan_portfolio_analysis.ipynb  # Narrative analysis
│  └─ executive_summary.ipynb  # Finding from the analysis
├─ src/
│  ├─ load_data.py
│  └─ segmentation.py
├─ requirements.txt
└─ README.md
```

## ▶️ How to run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/loan_portfolio_analysis.ipynb
```

> The notebook assumes a DataFrame with a binary **`bad`** column (1 = default, 0 = good).  
> Use `src/segmentation.py::segment_table(df, col)` to build segment tables with counts and default rates.

## 📊 Example questions answered
- What is the overall default rate?
- Which borrower/loan attributes correlate with higher default?
- Which segments underperform vs the portfolio average?
- What is the overall quality of the data?

## Final conclusion:
- Provided in executive_summary.ipynb

## 📄 Data
This repo is set up for **public or synthetic data**. Put your excel(s) in `data/` and reference them in the notebook.
