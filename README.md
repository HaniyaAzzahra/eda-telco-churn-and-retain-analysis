# eda-telco-churn-and-retain-analysis
EDA, K-Prototype clustering, and churn prediction validate trough (Logistic regression, XGBoost, Random Forest). Detailed step by step from data cleaning to actionable insight

Hi Guys 👋🏻👋🏻, this is my personal portfolio project to learn and exercise my skills in doing exploratory data analysis for a telco company’s customers, specifically for segmentation & retention.

This notebook walks through the full end-to-end process — from raw data to actionable retention strategy. Here is what is covered:

* Step 1 — Data Quality Assessment. Validated 7,043 records, fixed data types, handled missing values in TotalCharges, and confirmed the data was clean before analysis began.

* Step 2 — Exploratory Data Analysis. Broke down churn patterns across demographics, services, contracts, and payment methods. Identified which customer segments carry the highest and lowest risk before building any models.

  * Layer 1 — Rule-Based Persona. Designed 3 customer personas using business logic and domain knowledge. This established the baseline segmentation and revealed where manual rules hit their ceiling.

   * Layer 2 — Statistical Clustering (K-Prototype). Let the data define natural customer groups. Used elbow method and silhouette score to select K=5. The clusters revealed behavioral segments that manual rules could not        capture.

* Feature Validation — Mutual Information & XGBoost. Identified which features actually predict churn. Confirmed 4 key drivers that all three predictive models agree on: tenure, contract type, support/security add-ons, and service zone.

Layer 3 — Predictive Scoring. Built and compared Logistic Regression, Random Forest, and XGBoost. Selected Random Forest as the best model (AUC 0.832). Scored every active customer by churn probability, ranked them by revenue at risk, and produced a ready-to-use retention priority list.

Step 3 — Stakeholder Deliverable. Translated all findings into a presentation deck that tells the full story for business stakeholders — from customer segments and churn drivers to the retention priority list. The goal was not just to build models, but to make the insights actionable for stakeholders who need the business takeaway, not the technical details

If you are here to see how customer segmentation and churn prediction work in practice from cleaning data to delivering a prioritized action list, this notebook walks through every decision, trade-off, and business interpretation along the way.
