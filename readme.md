# Predicting Occupancy Rate of Government Housing Projects in India

## 📌 Overview
This project uses Machine Learning to predict the **percentage of government-developed houses that are occupied** across Indian states.  
It is built using **real housing data from the Indian Government (data.gov.in)** and focuses on understanding how project progress and investment relate to housing utilization.

---

##  Problem Statement
Government housing projects involve significant investment, but not all completed houses are actually occupied.  
The goal of this project is to **predict the occupancy percentage of completed houses** using project level and financial indicators, helping understand utilization trends.

---

##  Dataset
- **Source:** https://www.data.gov.in/sector/Housing  
- **Type:** State-wise aggregated government housing data  
- **Features include:**
  - Number of projects considered
  - Investment amount
  - Central assistance
  - Houses involved
  - Houses grounded
  - Houses completed
  - Houses occupied

---

##  Methodology
1. **Data Cleaning**
   - Renamed columns for clarity
   - Handled missing values
   - Removed invalid rows where completed houses = 0

2. **Feature Engineering**
   - Created a synthetic feature:
     ```
     Occupancy Percentage = (Houses Occupied / Houses Completed) × 100
     ```

3. **Modeling**
   - Split data into training and testing sets (80/20)
   - Trained a **Linear Regression** model

4. **Evaluation**
   - Used **Root Mean Squared Error (RMSE)** to measure prediction accuracy
   - Visualized **Actual vs Predicted Occupancy Percentage**

---

##  Machine Learning Model
- **Algorithm:** Linear Regression  
- **Type:** Supervised Learning (Regression)

---

##  Evaluation Metric
- **RMSE (Root Mean Squared Error)**  
  Measures the average deviation between actual and predicted occupancy percentages.

---

##  Results
- The model captures the **general trend** between housing project progress and occupancy.
- Predictions are reasonably accurate given the **small, aggregated dataset**.
- Scatter plot shows most predictions clustering around the ideal diagonal line.

---

##  Key Insights
- Higher completion and grounding rates generally lead to higher occupancy.
- Investment alone does not guarantee high occupancy completion efficiency matters.
- Aggregated state-level data hides local factors influencing housing utilization.

---

##  Tools & Technologies
- Python
- pandas
- NumPy
- scikit-learn
- matplotlib

---

##  Limitations
- Small dataset (state-level aggregation)
- No time-series data
- Policy, regional, and socio-economic factors not included
- Model captures correlation, not causation

---

##  Future Improvements
- Try advanced models (Ridge Regression, Random Forest)
- Add more government datasets
- Include year-wise data for trend analysis
- Perform deeper exploratory data analysis (EDA)

---

##  Project Structure
