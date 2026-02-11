# Assignment5.1
Project: Will a Customer Accept the Driving Coupon?
Project Overview
This project analyzes data from the UCI Machine Learning Repository to predict whether a driver will accept a coupon delivered to their mobile device while driving. The data represents various scenarios including weather, time of day, passenger types, and the driver's destination.

The primary goal is to use Exploratory Data Analysis (EDA) and Visualization to identify which demographics and environmental factors are most likely to lead to a coupon acceptance.

Key Findings
Overall Acceptance: The general acceptance rate for coupons across the entire dataset was ~56%.

Bar Coupons: Drivers who frequent bars more than once a month and are over the age of 25 showed an acceptance rate of ~69%, compared to ~33% for the general population.

Coffee House Trends: Acceptance peaked during the mid-morning hours (10 AM), reaching approximately 64%. Drivers with No Urgent Destination were significantly more likely to accept the coupon (around 58%) compared to those commuting to Work (around 44%). This suggests that coffee coupons are more effective when the driver has the flexibility to make an unscheduled stop.
Demographic Influence: Drivers traveling with Friends or Partners showed an acceptance rate of 76% for Carry-out and Coffee coupons, which is significantly higher than those driving Alone 73%. Conversely, drivers with Kid(s) in the car had the lowest acceptance rate in this category at 70%, suggesting that convenience is weighed against the complexity of the trip. Furthermore, drivers under the age of 30 were the most responsive demographic overall, particularly when the weather was Sunny and they had no urgent time constraints.

Actionable Recommendations
Optimize Delivery Timing: Target Coffee House coupons specifically between [Time] and [Time] for drivers in the "No Urgent Destination" category.

Target High-Frequency Users: Focus Bar and Restaurant coupons on users who already report visiting these establishments at least 1-3 times per month.

Passenger Context: Carry-out coupons should be prioritized for drivers traveling with friends or partners, as they show a higher conversion rate than solo drivers.

Data Description
The dataset includes variables such as:

Destination: No Urgent Destination, Home, Work.

Weather: Sunny, Rainy, Snowy.

Temperature: 30°F, 55°F, 80°F.

Coupon Types: Bar, Carry out & Take away, Coffee House, Restaurant (<$20), Restaurant ($20-$50).

Repository Contents
data/: Contains the original coupons.csv dataset.

notebooks/: The main Jupyter Notebook featuring data cleaning, visualizations, and statistical analysis.

images/: Exported plots used for the final report.

How to Run the Analysis
Clone this repository.

Ensure you have pandas, seaborn, and matplotlib installed.

Open notebooks/prompt.ipynb in Jupyter Notebook or VS Code.
