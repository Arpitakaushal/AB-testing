# 📊 Facebook vs AdWords Campaign Analysis

This project analyzes the performance of **Facebook Ads** vs **AdWords Ads** using Python, Pandas, Seaborn, Matplotlib, and statistical methods.  
It helps marketers and analysts **understand which advertising platform drives more conversions**, **analyze trends over time**, and **optimize advertising budget**.

---

## 📂 Files in this Repository
- `marketing_campaign.csv` → Dataset used for analysis  
  - Dataset link: [Download CSV](https://example.com/marketing_campaign.csv)  
- `facebook_ads_analysis.ipynb` → Jupyter Notebook with all code and analysis  
- `README.md` → Documentation for the project  

---

## 🛠️ Technologies & Libraries Used
- Python 3  
- Pandas, NumPy  
- Matplotlib, Seaborn (Data Visualization)  
- Scipy, Statsmodels (Statistical Analysis)  
- Scikit-learn (Regression Analysis)  

---

## 📈 Project Workflow

### 1. Data Cleaning
- Converted date column to datetime format  
- Removed unwanted symbols (`%`, `$`) from rate and cost columns  
- Converted cleaned values to numeric format  

### 2. Exploratory Data Analysis (EDA)
- Histograms of clicks & conversions for both campaigns  
- Categorized conversions into buckets (`<6`, `6-10`, `10-15`, `>15`)  
- Compared daily conversion frequency between Facebook and AdWords  

### 3. Correlation Analysis
- Strong correlation between **Facebook Ad Clicks & Conversions (0.87)**  
- Moderate correlation between **AdWords Ad Clicks & Conversions (0.45)**  

### 4. Hypothesis Testing
- **Null Hypothesis (H0):** µ_Facebook ≤ µ_AdWords  
- **Alternative Hypothesis (H1):** µ_Facebook > µ_AdWords  
- Result: p-value < 0.05 → Reject H0 → Facebook ads drive significantly more conversions  

### 5. Regression Analysis
- Built Linear Regression model to predict Facebook conversions from clicks  
- Achieved R² score of **76.35%**  
- Example prediction:  
  - 50 Clicks → ~12 Conversions  
  - 80 Clicks → ~18 Conversions  

### 6. Time-Series Analysis
- Weekly trend → Highest conversions on **Monday & Tuesday**  
- Monthly trend → General increase, dips in Feb, Apr, May, Jun, Aug, Nov  

### 7. Cost Per Conversion (CPC) Analysis
- Lowest CPC in **May & November** (cost-effective months)  
- Highest CPC in **February**  

### 8. Cointegration Test
- Found a **long-term equilibrium relationship** between Ad Spend & Conversions  

---

## 🔑 Key Insights
- Facebook Ads outperform AdWords in terms of conversion effectiveness  
- Strong correlation suggests clicks on Facebook ads strongly drive sales  
- Advertising budget should be **optimized towards Facebook campaigns**  
- Seasonal and monthly patterns must be considered for cost-effective planning  

---

## 🚀 How to Run the Project
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/Facebook_Ads_Project.git
2.Install required libraries:
  
   pip install pandas numpy matplotlib seaborn scipy scikit-learn statsmodels
3. Run Jupyter Notebook:

  jupyter notebook facebook_ads_analysis.ipynb

📌  Conclusion

Facebook Ads outperform AdWords in terms of conversions and overall campaign effectiveness.

Strong correlation between Facebook clicks and conversions indicates that increasing clicks directly drives higher sales.

Time-series analysis shows consistent weekly performance with peak conversions on Mondays and Tuesdays, and some seasonal variations across months.

Cost Per Conversion (CPC) analysis highlights the most cost-effective months for advertising.

Statistical tests (hypothesis testing & cointegration) confirm that Facebook advertising delivers significantly better results and maintains a stable relationship between spend and conversions.

Insights from this project can guide marketers to optimize ad spend, improve campaign strategies, and maximize ROI.
