## 📊 Call Centre Analysis Dashboard
## 📊 Project Call Centre

### 🔍 Overview

This Power BI dashboard comprehensively analyses a call centre across key metrics like call volume, acceptance rate, and agent/team leader performance. The dashboard offers insights into operational efficiency and highlights performance distribution under different team leaders. It's designed to assist management in monitoring, analysing, and optimising contact centre operations.

---
### 📁 Dataset Structure

The dashboard is built using the following data tables:

* **CALL\_CENTER\_DATA**: Contains all transactional-level call records with metrics like call status, duration, and offer application.
* **AGENT**: Agent-specific information used for mapping calls received, accepted, and offers applied.
* **TEAM\_LEADERS**: Contains team leader names and associated agents.
* **All Measures**: This table contains DAX-calculated KPIs used across the dashboard (note: error currently exists likely due to naming with special characters).

### 📈 Key Metrics & Visuals

#### ✅ **Top Summary KPIs** *(in “Top 10” Tab)*

* **Total Calls**: `16,491`
* **Total Calls with Accept**: `11,571`
* **Total Calls with Offer Applied**: `8,108`
* **Offer Percentage**: `92.49%` – Derived as offers applied vs. total eligible calls
* **Acceptance Percentage**: `75.86%`
* **Breakage**: `29.93%` – Percentage of calls that didn't result in offer application post-acceptance

These KPIs offer a snapshot of funnel efficiency — from call received to acceptance and offer application.

#### 📋 **Agent Performance - Top 10 Listings**

* **Top 10 Calls Received**: Displays agents like *Harrison Harold* and *Gee Garry* with call volume close to 800.
* **Top 10 Calls Accepted**: Highlights agents like *Centerville Cece* and *Filipsano Fiona* with high conversion from received to accepted calls.
* **Top 10 Offers Applied**: Features agents who performed best in guiding customers to final offer application, with *Gee Garry* and *Filipsano Fiona* topping the list.

These lists are accompanied by totals at the bottom, showcasing group contribution and distribution.

#### 👥 **Team Leader Breakdown - (Home Tab)**

* A **donut chart comparison** shows call distributions across three team leaders:

  * **Jimson Bill**: 31.70%
  * **Oferten Quinton**: 32.87%
  * **Winnerson Aceona**: 35.42%

* This visualisation reflects how calls are distributed under leadership for performance comparison.

#### 📞 **Call Volume Metrics (Home Tab)**

* **Total Calls Received**: `17,573`
* **Total Calls with Acceptance**: `12,244`
* **Total Handled Time**: `1,32,98,106` (appears to be cumulative seconds or milliseconds — needs clarification)

These numbers help monitor productivity and overall call engagement.

### 🧠 Insights

* **Balanced Team Performance**: Team leaders show nearly equal call load, indicating fair resource distribution.
* **High Breakage Rate (29.93%)**: Needs attention — implies that nearly 1 in 3 accepted calls do not result in an offer application.
* **Agent-specific opportunities**: Some agents receive significantly more calls than others — performance reward or workload review may be warranted.

### ⚙️ Technical Considerations

* **Calculated Measure Error**: The table “All Measures” is showing a warning/error, likely due to improper use of special characters in measure/table names. This should be corrected using bracket notation.
* **Visual Design**: Use of consistent icons, corporate-style layout, dark theme, and strategic colour-coding improves user readability and visual storytelling.
* **Navigation**: Tab-like buttons (Home, Top 10, Metrics, Insights) suggest interactive navigation — great for layered exploration.

### 📌 Recommendations for Enhancement

1. **Data Validation**: Review the unit used for “Total Handled Time” and apply formatting (hh\:mm\:ss) for better clarity.
2. **Breakage Drilldown**: Add a slicer or decomposition tree to understand root causes of offer breakage.
3. **Time Trends**: Introduce time series to monitor metrics over weeks/months (e.g., via line chart or area chart).
4. **Dynamic Filtering**: Enable drill-through or slicers to view agent/team performance per time (June, July, August buttons are a great start).

### 🛠 Tools Used

* **Microsoft Power BI Desktop**
* DAX for measure calculation
* Custom visuals (donut, KPI cards, tables)
* Power BI bookmarks & buttons for navigation

  ### Screenshot
  https://github.com/SriUtkarsh2709/Project-Call-Centre/blob/main/Call%20centre%20analysis.png  

Let me know if you'd like this adapted as a `README.md` file for your GitHub repo.
# Project-Call-Centre
