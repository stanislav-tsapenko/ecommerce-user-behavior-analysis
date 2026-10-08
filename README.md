# E-commerce Sales and User Behavior Analysis

## Project Overview

This repository contains an analytical project focused on e-commerce data to identify sales trends, user behavior patterns, and key factors influencing revenue.
The goal of this project is to provide actionable insights that can assist in making informed business decisions.

## Data Source

The data for this analysis was obtained from 'data-analytics-mate' via an SQL query.
It includes key metrics such as: `order_date`, `session_date`, `price`, `account_id`, `is_verified`, `is_unsubscribed`, `device`, `traffic_source`, `product_category`, `country`, `continent`, `operating_system`, etc.
The dataset covers 349,545 sessions and 27,946 accounts from 2020-11-01 to 2021-01-31. The source database (`data-analytics-mate`) is not public, so the results are saved in the notebook outputs.

## Tools and Technologies

* **Google Colab / Python:** Used for data preparation, cleaning, transformation, and statistical analysis.
    * Key libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`.
* **Tableau Public:** Utilized for interactive data visualization and dashboard creation.

## Repository Structure

* `Comprehensive_E_commerce_Sales_and_User_Behavior_Analysis.ipynb`: Google Colab notebook with data preparation, cleaning, statistical analysis and initial visualizations.
* Tableau dashboard: see the link in the section below (the workbook is published on Tableau Public).
  
## Analysis and Insights

This project explores:
* **Key Sales and User Metrics:** Analysis of fundamental sales figures and user characteristics.
* **Sales Dynamics:** Examination of how sales metrics evolve over time.
* **Pivot Tables and Aggregated Metrics:** Utilization of summarized data to highlight important trends and totals.
* **Statistical Analysis of Relationships:** Investigation into the correlations and connections between different variables.
* **Statistical Analysis of Differences Between Groups:** Comparison of metrics across various user segments or categories to identify significant variations.

Key insights:
* **Revenue:** $31.97M from 33,538 orders (average order value $953). The United States alone brings $13.94M (about 44% of total revenue), followed by India ($2.81M) and Canada ($2.44M).
* **Products:** the top 3 categories (Sofas & Armchairs $8.39M, Chairs $6.15M, Beds $4.92M) generate about 61% of revenue.
* **Devices and channels:** desktop accounts for 59% of revenue; Organic Search is the largest marketing channel (35.8% of revenue).
* **Relationships:** daily revenue correlates strongly with session count (Spearman ρ = 0.90). Revenue across continents, channels, devices and categories also moves together (all pairs significantly positively correlated), which is expected because all segments follow the same overall demand and seasonality.
* **Group differences:** daily revenue of verified users is higher than that of unsubscribed users (Mann–Whitney U, p < 0.0001); traffic channels differ significantly in daily sessions (Kruskal–Wallis, p < 0.00001); revenue per order does not differ by day of the week (p = 0.12). These results show association, not causation.

## Business Recommendations

Based on the results above (hypotheses to be tested, not proven effects):
* **Focus on the US market:** it brings about 44% of revenue, so marketing budget and delivery/payment experience there have the biggest impact.
* **Prioritise the leading categories:** Sofas & Armchairs, Chairs and Beds generate about 61% of revenue; they are the first candidates for promotion and stock planning.
* **Do not neglect desktop:** it accounts for 59% of revenue, so checkout improvements on desktop should be tested first.
* **Review channel mix:** Organic Search is the largest channel (35.8% of revenue); it is worth checking how dependent the business is on it and how Paid Search and Direct compare in return.
## Limitations

* The data covers only three months (November 2020 – January 2021), which includes holiday-season demand, so seasonal conclusions should be treated with caution.
* Daily revenue correlations between segments are partly driven by common overall demand and do not show cause and effect.
* Groups of users (verified/unsubscribed, registered/unregistered) are compared by total daily revenue; because the groups differ in size, a per-user comparison would be more precise.
* The source database (`data-analytics-mate`) is not public, so the analysis can be reproduced only from the saved notebook outputs.
## How to View the Tableau Dashboard

You can view the interactive Tableau dashboard via the following link:
[**↗ Comprehensive E-commerce Sales and User Behavior Analysis**](https://public.tableau.com/views/E_commerce_17498228881310/ComprehensiveE-commerceSalesandUserBehaviorAnalysis)

## How to Run the Colab Notebook

You can open and run the Google Colab notebook directly in your browser:
[**↗ Run in Google Colab**](https://colab.research.google.com/github/stanislav-tsapenko/ecommerce-user-behavior-analysis/blob/main/Comprehensive_E_commerce_Sales_and_User_Behavior_Analysis.ipynb)

## Future Steps

* Develop a predictive model for forecasting future sales and product demand.
* Conduct deeper customer segmentation to develop more targeted marketing campaigns.

## Contact

* **Stanislav Tsapenko**
* [**↗ LinkedIn**](https://www.linkedin.com/in/stanislav-tsapenko-bb097a319)
* [**↗ Email**](mailto:stanislav.tsapenko.da@gmail.com)
