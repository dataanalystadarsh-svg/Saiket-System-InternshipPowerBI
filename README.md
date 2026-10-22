Projects Title- Customer Churn Analysis And Prediction

Task 1- DATA CONNECTION

-This include Data Importing and Connection in Power BI.

Task 2- DATA TRANSFORMATION

-This include Data Cleaning and Transformation Technique.

-Proficiency in DATA

Task 3- DASHBOARD COMPONENTS

a_)- Churn Rate (%) Overview
-Rating Summary Visualization

<img width="1350" height="737" alt="Screenshot 2026-10-22 152601" src="https://github.com/user-attachments/assets/c47a07a6-e969-44a3-af56-176d4a3c87ef" />


b_)- Customer Demographics
-Based on Gender, Partner Status, Dependents Status.
- Used Bar Charts / Pie Charts

  <img width="1414" height="739" alt="Screenshot 2026-10-22 152620" src="https://github.com/user-attachments/assets/7ecc3aea-ba8b-4c39-9af4-bcbeb559260c" />


c_)- Customer Tenure Analysis in Months
-Total Months
-Used Histograms.

<img width="1345" height="748" alt="Screenshot 2026-10-22 152634" src="https://github.com/user-attachments/assets/caf67840-9c85-4a77-9c62-181ab75fd48c" />


d_)- Churn Analysis based on Contract Types , Payment Method, Internet Services.
- used bar charts or Stacked bar chart.

  <img width="1388" height="733" alt="Screenshot 2026-10-22 152650" src="https://github.com/user-attachments/assets/197c49c5-4f4e-414b-88a1-c726362b67c0" />

Creating Required Column or Measures for Projects :-
1- Add and Transform Data
Add Column- Customer column to make senior citizen readable
syntax: if[SeniorCitizen] = 1 then "Senior" else "Non-Senior"

2- To Avoid a Numeric Churn Flag-
syntax: if[Churn] = "Yes" then 1 else 0

3- Create Tenure Group- A histograms works better with buckests.
syntax: if[tenure] <= 12 then "0-12 months"
else if[tenure] <= 24 then "13-24 months"
else if[tenure] <= 48 then "25-48 months"
else "49-72 months"

DAX MEASURES-

1- Total Customers = COUNTROWS(Telco)

2- Churned Customers = CALCULATE(COUNTROWS(Telco), Telco[Churn] = "Yes")

3- Churn Rate % = DIVIDE([Churned Customers], [Total Customers])

4- Avg Tenure = AVERAGE(Telco[Tenure])

Prepared by Adarsh Verma. I used the assistant help of CLAUDE AI for understanding of logic and components of data as i also studied the prompt engineering of Ai assistant.
that will help to complete our work effectively and efficiently.

Thank you.
