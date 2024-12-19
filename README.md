# Customer-Churn-Analysis
This code is a comprehensive analysis of customer churn using a dataset containing demographic and service-related information. Here's a breakdown of what it does:

1. Data Preparation:
Reading and Inspecting Data:

Loads the dataset Customer Churn.csv and displays basic information like column types and summary statistics.
Fixes the TotalCharges column by replacing spaces with 0 and converting it to a float type.
Data Cleaning:

Ensures no null values exist (df.isnull().sum().sum() confirms this).
Converts the SeniorCitizen column values (1 to "yes", 0 to "no").
2. Exploratory Data Analysis (EDA):
Customer Churn Overview:

A bar plot and pie chart show the distribution of churned vs. non-churned customers.
Churn by Demographics:

Count plot of gender shows churn distribution by gender.
SeniorCitizen column visualized with a stacked bar chart to illustrate churn percentages.
Churn by Tenure:

A histogram (sns.histplot) visualizes the tenure distribution across churned and non-churned customers.
Churn by Contract:

A count plot illustrates customer churn based on contract type (e.g., month-to-month, one year, two years).
Churn by Payment Method:

A count plot compares churned vs. non-churned customers for different payment methods.
3. Additional Service Analysis:
Analyzes the impact of services like:
PhoneService
MultipleLines
InternetService
OnlineSecurity
StreamingTV, etc.
Visualized with:
Count plots for each service category, grouped by churn status.
4. Key Visualizations and Insights:
Distribution Visualizations:

Pie charts and histograms provide a holistic view of data distribution.
Stacked bar charts for churn percentages are labeled with precise values.
Multiplot Grid:

Services-related attributes are visualized in a grid of count plots for compact, comparative analysis.
5. Usability:
The code is modular, uses subplots for compact visualization, and integrates Seaborn for aesthetics and Matplotlib for customization.
