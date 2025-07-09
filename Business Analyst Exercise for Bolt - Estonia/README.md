# 📘 Customer Support Ticket Forecasting & Market Health Analysis

**Role:** Senior Business Analyst  
**Company:** BOLT 
**Industry:** Customer Support / Tech Platform Operations 
**Scope:** Forecasting agent staffing needs and market health analysis using ticket and order data for a specific market over a 31-day horizon  
**Key Deliverables:** Formal KPI definitions, Data Analysis & Exploration, Time Series Forecasting, Market Health Insights, Reporting for Technical and Non-Technical Stakeholders 

---

## 🧭 Project Overview
This project addresses forecasting the daily number of customer support agents required to cover the expected volume of support tickets in a specific market over at least 31 days. Additionally, it includes a detailed analysis of the market's health through the key metric Tickets Per Ride (TPR).

Understanding ticket volume is critical for operational planning as it directly impacts staffing needs. The TPR ratio provides insights into the efficiency and “health” of the market, indicating whether the support workload aligns with business activity.

---

## Formal Definition: Tickets Per Ride (TPR)
TPR is defined as:

TPR = Number of Support Tickets / Number of Orders (Rides)
 
Where:
- Support Tickets refers to the total customer support requests generated in a given period.
- Orders (Rides) refers to the total number of completed transactions or rides in the same period.

TPR serves as a normalized indicator of how many tickets arise per order, helping to measure service quality and operational workload.

---

## Data Sources
Two CSV files were provided:
- Tickets dataset: Containing ticket-level data, including timestamps and ticket counts.
- Orders dataset: Containing order-level data (rides), timestamps, and counts for the same market and time frame.

---

## Methodology
### 🔹 Data Preparation & Exploration
- Loaded and cleaned datasets, ensuring consistent time formats and matching periods.
- Aggregated data at the daily level to align tickets and orders.
- Calculated daily TPR values to observe trends and anomalies.

### 🔹 Market Health Analysis
- Analyzed TPR trends over time to assess market stability.
- Identified periods of abnormal TPR spikes or drops.
- Compared TPR against historical averages to flag potential service issues.

### 🔹 Forecasting Agent Demand
- Modeled the daily ticket volume using time series forecasting techniques (e.g., ARIMA, Exponential Smoothing).
- Derived agent requirements based on historical agent productivity rates (tickets handled per agent per day).
- Produced a 31-day forecast with confidence intervals to support capacity planning.

---

## Key Assumptions & Considerations
- Average ticket handling time and agent productivity were estimated due to lack of direct data.
- The relationship between ticket volume and required agents was assumed linear.
- External factors such as promotions, outages, or seasonality were not explicitly modeled due to missing data.
- Edge cases such as zero-ride days or ticket spikes were carefully reviewed for anomalies.

---

## Limitations & Missing Information
- No data on average ticket resolution times, which impacts agent load.
- No segmentation by ticket priority or complexity.
- Lack of contextual factors (marketing campaigns, operational changes) that influence ticket volume.
- More granular agent performance data would improve forecasting precision.

---

## Conclusions & Recommendations
- TPR is a valuable KPI to monitor ongoing market health and support workload.
- The forecast indicates expected ticket volumes and corresponding staffing needs, enabling proactive resource allocation.
- Recommendations include collecting additional data on ticket resolution and agent efficiency, and integrating external business factors to enhance forecast robustness.
- Establishing continuous monitoring of TPR trends can help detect emerging issues early and adjust staffing dynamically.

---

## How to Use This Analysis
- Business stakeholders can leverage the forecast to optimize hiring and scheduling.
- Support managers can track TPR as an early warning system for operational risks.
- Data analysts can build upon this foundation by incorporating more detailed data and refining forecasting models.
