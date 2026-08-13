# NorthStar Retail — Purchase Data Analysis (Practice Project)

> ⚠️ **Disclaimer:** This is a personal practice/learning project, **not** a real business case study or a production-grade analysis. "NorthStar Retail" is a fictional company, and all data used (`customer_purchases.csv`) is **synthetic/dummy data**, generated specifically for this exercise. It does not represent any real company, customers, or transactions.

## Why this project exists

I built this to review and reinforce core Python/pandas and statistics skills:

- Data cleaning (mixed date formats, dirty currency strings, missing values, duplicates, inconsistent text formatting)
- `datetime` handling in pandas
- Confidence intervals
- One-sample t-test
- Two-sample t-test
- A/B testing
- Hypothesis testing fundamentals (H0/H1, p-values, decision rules)

This is meant as a **hands-on refresher**, not a portfolio-polished analysis. The notebook reflects an actual learning process, including mistakes I made and fixed along the way.

## The data

`customer_purchases.csv` — 3,665 synthetic transaction rows, spanning 2020–2026, across 480 fictional customers.

The dataset was generated intentionally "dirty" to practice real-world cleaning:
- Multiple mixed date formats + blank/garbage dates
- `purchase_value` as a mix of numbers, `$1,234.50` strings, `N/A`/`-` placeholders, negatives, and extreme outliers
- Inconsistent casing/whitespace in `channel`, `region`, `customer_id`
- Exact duplicate rows
- Missing values across several columns

## What's in the notebook

1. **Cleaning** — parsing dates, converting currency strings to numeric, standardizing text fields, dropping duplicates/invalid rows
2. **Time-based analysis** — monthly revenue trend, weekday averages, customer recency, churn-risk list, cohort analysis
3. **Confidence intervals** — for mean purchase value (overall, by year, for an A/B group difference)
4. **One-sample t-tests** — testing purchase value against claimed benchmarks
5. **Two-sample t-tests** — channel comparison, year-over-year comparison, payment method comparison, weekday vs. weekend
6. **A/B testing** — simulated email campaign test (Group A vs Group B)

## Tools

Python, pandas, numpy, scipy.stats, matplotlib, seaborn

## Files

- `Python_Code.ipynb` — full notebook with cleaning + analysis
- `customer_purchases.csv` — synthetic dataset
- `analysis_brief.md` — original scenario/question brief used to guide the practice

---
*Feedback and suggestions are welcome — this project is meant to keep improving as I keep learning.*
