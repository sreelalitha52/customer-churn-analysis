# Customer Churn Analysis

## 📊 Dataset Used
- **Dataset**: Telco Customer Churn (commonly available on [Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn) or IBM sample datasets).  
- **Rows**: Each row represents a **customer**.  
- **Columns**: Customer demographics, account info, services used, tenure, charges, and churn status.

---

## 🛠️ Steps Performed
1. **Load Data**  
   - Imported CSV file into a pandas DataFrame.  

2. **Clean Missing Values**  
   - Checked for duplicates and nulls.  
   - Fixed data types (e.g., `TotalCharges` → numeric).  

3. **Feature Engineering**  
   - Created a `tenure_group` column to bucket customers by length of tenure.  

4. **Group Data**  
   - Aggregated churn rates by **Contract type**, **Internet Service**, **Payment Method**, and **Tenure Group**.  

5. **Plot Trends**  
   - Used matplotlib/seaborn to visualize churn patterns across segments.  

6. **Summarise Insights**  
   - Identified **which groups have the highest churn risk**.  
   - Compared churners vs non-churners on average monthly charges.  
   - Listed top customer segments contributing most to churn.  

7. **Save Work**  
   - Notebook saved as `customer_churn_analysis.ipynb`.  
   - Key insights exported into `insights_summary.md` and included in this README.  

---

## 🔑 Key Insights
- **Overall churn rate**: ~26% (depends on dataset sample).  
- **Highest churn risk**:  
  - Customers on **Month-to-Month contracts**.  
  - Customers with **Fiber optic internet**.  
  - Customers in the **1–12 months tenure group**.  
- **Customer behavior**: Churners often pay **slightly higher monthly charges** compared to non-churners.  
- **Retention suggestion**: Incentivize long-term contracts, improve Fiber optic support, and target early-tenure customers with promotions.  

---

## ▶️ How to Run the Notebook
1. Clone this repository or download the project files.  
2. Install required libraries:
   ---bash
   pip install pandas matplotlib seaborn
