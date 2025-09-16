# AI Marketing Attribution Project

## Project Overview
This project explores **AI-driven marketing attribution** to measure the contribution of various marketing channels to conversions. Using a multi-touch dataset, I implemented both **rule-based attribution models** (first-touch, last-touch, linear) and a **machine learning-based approach** (logistic regression) to evaluate channel effectiveness.

The goal is to provide insights that help marketers **allocate budgets efficiently** and optimize campaigns based on channel performance.

---

## Dataset
- **Source:** Kaggle – [Multi-Touch Attribution Dataset](https://www.kaggle.com/datasets/vivekparasharr/multi-touch-attribution)
- **Rows:** 10,000+ user interactions  
- **Columns:**
  - `User ID` – unique identifier for each user  
  - `Timestamp` – interaction timestamp  
  - `Channel` – marketing channel  
  - `Campaign` – campaign name  
  - `Conversion` – target variable (Yes/No)  

---
## Dataset
- **Source:** Kaggle – [Multi-Touch Attribution Dataset](https://www.kaggle.com/datasets/vivekparasharr/multi-touch-attribution)
- **Rows:** 10,000+ user interactions  
- **Columns:**
  - `User ID` – unique identifier for each user  
  - `Timestamp` – interaction timestamp  
  - `Channel` – marketing channel  
  - `Campaign` – campaign name  
  - `Conversion` – target variable (Yes/No)  

---
## Methods

### 1. Data Preparation
- Converted `Conversion` to numeric (1 = Yes, 0 = No)  
- Aggregated channel sequences per user in chronological order  
- Extracted **first-touch** and **last-touch** channels  

### 2. Attribution Models
**Rule-Based:**
- **First-Touch:** Full credit to first channel in user journey  
- **Last-Touch:** Full credit to last channel  
- **Linear:** Equal credit to all channels in the sequence  

**Machine Learning-Based:**
- Logistic Regression with **one-hot encoded channels**  
- Coefficients normalized to show relative contribution  

---

## Key Findings

### Conversion Rates by Touch
- First-touch channels with highest conversion: `Email`, `Social Media`  
- Last-touch channels driving conversions: `Direct Traffic`, `Search Ads`  

### Attribution Comparison
- Linear attribution spreads credit across all channels  
- ML-based model highlights **most influential channels** based on actual conversion data  

*Visualizations are saved in the `/visuals` folder.*

---

## Visualizations

