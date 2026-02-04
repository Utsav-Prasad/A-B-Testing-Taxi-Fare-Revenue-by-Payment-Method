🚕 Maximizing Revenue for Taxi Drivers through Payment Type Analysis
📌 Project Overview

In the fast-paced taxi booking industry, maximizing driver revenue is critical for sustainability and driver satisfaction.
This project uses data-driven analysis and hypothesis testing to examine whether payment method (Card vs Cash) impacts fare amount, and whether nudging customers toward certain payment types can increase driver revenue without harming customer experience.

🎯 Objective

Analyze the relationship between payment type and fare amount

Perform A/B testing using statistical hypothesis testing

Identify whether credit card payments generate higher fares than cash

Provide actionable business insights for taxi drivers and platforms

❓ Research Question

Is there a relationship between total fare amount and payment type, and can customers be nudged toward payment methods that generate higher revenue for drivers without negatively impacting customer experience?

📊 Dataset

Source: NYC Yellow Taxi Trip Records (January 2020)

Initial Size: ~6.4 million records

Final Cleaned Data: ~2.7 million records

Key Features Used:

passenger_count

trip_distance

payment_type

fare_amount

trip_duration

🧹 Data Cleaning & Preparation

Removed missing values (~1%)

Removed duplicate records

Filtered:

Valid passenger counts (1–5)

Payment types (Card & Cash only)

Positive fare, distance, and duration

Removed outliers using IQR method

📈 Exploratory Data Analysis (EDA)

Fare and trip distance distributions by payment type

Payment type preference visualization

Passenger count vs payment method analysis

Descriptive statistics comparison

Key Observation:

Credit card payments show higher average fare and trip distance than cash payments.

🧪 Hypothesis Testing
Test Used

Independent Two-Sample T-Test (Welch’s T-Test)

Chosen due to:

Large sample size

Non-normal fare distribution

Unknown population variance

Hypotheses

Null (H₀): No difference in average fare between card and cash payments

Alternative (H₁): A significant difference exists

Results

T-Statistic: 165.59

P-Value: < 0.05

✅ Null hypothesis rejected

💡 Key Business Insight

Customers who pay using credit cards generate significantly higher average fares than those who pay with cash.

📌 Recommendation

Taxi platforms and drivers can strategically encourage credit card payments (e.g., rewards, convenience nudges) to increase revenue, while maintaining a positive customer experience.

🛠️ Tools & Technologies

Python

Pandas & NumPy

Matplotlib & Seaborn

SciPy & Statsmodels

Jupyter Notebook# A-B-Testing-Taxi-Fare-Revenue-by-Payment-Method
This project examines the impact of payment methods on taxi fare revenue using NYC Yellow Taxi data. Through EDA and A/B hypothesis testing, it finds that credit card payments generate significantly higher fares, offering data-driven insights to improve driver revenue.
