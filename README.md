# 🎫 Coupon Acceptance Analysis: "Will They Pull Over?"
### A Behavioral Study of In-Vehicle Coupon Recommendations

---

## 📌 Project Overview
This project analyzes data from the UCI Machine Learning Repository to predict whether a driver will accept a coupon delivered to their mobile device while driving. The data represents various scenarios including weather, time of day, passenger types, and the driver's destination.

**The Goal:** Use Exploratory Data Analysis (EDA) and Visualization to identify which demographics and environmental factors are most likely to lead to coupon acceptance.

---

## 📊 Key Findings

### 📈 General Trends
* **Overall Acceptance:** The general acceptance rate for coupons across the entire dataset was **~56%**.
* **Habitual Influence:** Drivers with an existing habit of visiting an establishment (1-3 times per month) show a significantly higher acceptance rate (**60-70%**) compared to those who "never" visit (**<20%**).

### 🔍 Category Deep-Dives

| Category | High-Acceptance Segment | Acceptance Rate |
| :--- | :--- | :--- |
| **Bar Coupons** | Frequent bar-goers (>1/mo) over age 25 | ~69% |
| **Coffee House** | Mid-morning (10 AM) + No Urgent Destination | ~64% |
| **Carry-out** | Social context (Driving with Friends/Partners) | ~76% |

### 👨‍👩‍👧‍👦 Demographic & Social Influence
* **Social Context:** Drivers traveling with Friends or Partners showed a significantly higher acceptance rate (**76%**) than those driving Alone (**73%**).
* **The "Kid" Factor:** Drivers with children in the car had the lowest acceptance rate (**70%**), suggesting that logistical complexity is weighed against the convenience of the coupon.
* **Age & Environment:** Drivers under the age of 30 were the most responsive demographic overall, particularly during Sunny weather with no urgent time constraints.

---

## 💡 Actionable Recommendations
1.  **Optimize Delivery Timing:** Target Coffee House coupons specifically between 10:00 and 14:00 for drivers in the "No Urgent Destination" category.
2.  **Target High-Frequency Users:** Focus marketing spend on users who already visit these establishments at least 1-3 times per month.
3.  **Passenger Context:** Prioritize Carry-out coupons for drivers traveling with friends or partners to capitalize on higher social conversion rates.

---

## 🛠️ How to Run the Analysis

### 1. Prerequisites
Ensure you have a Python environment installed (3.8+ recommended). Install the required libraries:
```bash
pip install pandas numpy seaborn matplotlib
```
### 2. Installation & Setup
Bash
# Clone the repository
```
git clone [https://github.com/rover141/Assignment5.1.git](https://github.com/rover141/Assignment5.1.git)
```
# Navigate to the directory
```
cd Assignment5.1
```
### 3. Execution
Launch Jupyter Notebook: jupyter notebook

Navigate to the /notebooks folder and open prompt.ipynb.

Select Cell > Run All to generate the analysis and visualizations.

---


### 📁 Repository Structure
```
Assignment5.1
├── data/
│   └── coupons.csv             # Source dataset from UCI
├── images/
│   └── *.png                   # Exported visualizations for this report
├── notebooks/
│   └── prompt.ipynb            # Main Jupyter Notebook analysis
└── README.md                   # Non-technical report and project overview
```
---



## 🏁 Next Steps and Recommendations
### Predictive Modeling (Machine Learning): 
Build a Random Forest or XGBoost Classifier to automatically determine if a coupon should be sent in real-time to minimize "coupon fatigue."

### Geospatial Proximity Integration: 
Incorporate a "Distance to Venue" variable to see if drivers require deeper discounts for longer detours.

### A/B Testing for Incentives: 
Run an A/B test specifically for the "Kid(s)" segment, testing messaging like "Drive-Thru" or "Kid-Friendly" to bridge the acceptance gap.

### Expansion of Demographic Features: 
Include features like "Vehicle Type" (e.g., EV vs. Gas) to see if charging stops influence coffee house habits.
