# Advertising Revenue Dashboard — User Guide

## Overview
This dashboard analyzes advertising revenue trends and enables strategic planning for H2 2026. It combines executive summaries, predictive forecasting, customer segmentation, and scenario modeling.

**[📊 View Live Dashboard](https://public.tableau.com/app/profile/donovan.schell/viz/AdvertisingSalesRevenue_17797490324870/AdvertisingRevenueSummary)**

## Dashboard Tabs

### 1. Advertising Revenue Summary
**Purpose:** Executive overview of current performance and dimensional breakdowns

**Key Features:**
- **KPI Cards:** Total revenue, active advertisers, campaign count (current vs. prior period with % change)
- **Dimensional Breakdowns:** Revenue by Ad Type, Segment, Industry Vertical, and Advertiser Location
- **Monthly Trend:** Revenue progression across the selected period
- **Top Advertisers Table:** Top 5-20 advertisers with revenue, segment, vertical, campaign count, and YoY metrics

**How to Use:**
1. Adjust Year, Month Start, Month End parameters to select your analysis period
2. Click any bar in the dimensional charts to filter all views to that dimension
3. Use the Top N slider to adjust how many advertisers to display
4. Filters apply across all summary visualizations

**Key Insight:** Segment 4 and Retail vertical drive growth; B2C and Technology show pullback in Search spend.

---

### 2. Growth Forecast
**Purpose:** Predict H2 2026 outcomes based on 2024-2025 trends

**Key Features:**
- **Revenue Forecast:** Projected H2 2026 revenue based on YoY growth rate
- **Advertiser Count Forecast:** Projected active advertiser growth
- **Growth Paradox Visualization:** Dual-axis chart showing advertiser growth (steep) vs. revenue growth (flat)
- **Confidence Intervals:** Shaded bands show forecast uncertainty ranges
- **Dimensional Forecasts:** Toggle between Total, Ad Type, Segment, Vertical, and Geography breakdowns

**How to Use:**
1. Review the summary KPI projections at the top
2. Examine the dual-axis forecast chart showing diverging trends
3. Use the "Forecast Breakdown" parameter to explore segment-specific projections
4. Note: Forecast assumes H2 2024-2025 trends continue without major market shifts

**Key Insight:** While advertiser count grows 22% YoY, revenue grows only 6% — new customers are smaller than existing ones.

---

### 3. Advertiser Health (RFM Segmentation)
**Purpose:** Segment customers by Recency, Frequency, and Monetary value to identify risks and opportunities

**Key Features:**
- **Segment Distribution:** Breakdown of advertiser count and revenue by segment
- **Segment Definitions:**
  - **Champions:** 1,692 advertisers, 93% of revenue — highly active, recent, high-spend
  - **Loyal:** 434 advertisers — consistent activity (5-6 months), high spend
  - **At Risk:** 118 advertisers — high spend but inactive since Sept+
  - **New:** 123 advertisers — recently acquired (Nov-Dec), low spend
  - **Churned:** 101 advertisers — dormant since Aug or earlier

**How to Use:**
1. Review segment distribution to understand customer composition
2. Focus retention efforts on "At Risk" segment (high revenue, at risk of churn)
3. Develop upsell strategy for "New" segment (cheap to acquire, low spend)
4. Monitor "Champions" for concentration risk (93% of revenue in 45% of accounts)

**Key Insight:** High concentration in Champions creates revenue risk. New customer acquisition is working but bringing small accounts.

---

### 4. Scenario Planning
**Purpose:** Test strategic decisions and model their impact on H2 2026 revenue

**Key Features:**
- **Three Adjustable Levers:**
  - **Retention Rate:** % of current advertisers retained (default 70% based on actual)
  - **New Advertiser Acquisition:** Count of new customers acquired (default 3,100 based on actual)
  - **Revenue per Advertiser Growth:** Multiplier on baseline spend (default 1.0 = no change)
- **Impact Cards:** Real-time display of projected changes in revenue, advertiser count, and revenue per advertiser
- **Comparison Charts:** Visual before/after showing H2 2025 Actual vs. H2 2026 Scenario

**How to Use:**
1. Read parameter explanations on the left to understand each lever
2. Adjust sliders to model different strategies:
   - Increase Retention to model a churn-reduction initiative
   - Increase New Acquisition to model aggressive growth
   - Increase Revenue per Advertiser to model upsell success
3. Watch KPI cards update with projected impact
4. Review comparison charts to visualize the change

**Example Scenarios:**
- **Conservative:** Retention 65%, New Acquisition 2,500, Revenue/Advertiser 1.0
- **Aggressive:** Retention 80%, New Acquisition 4,000, Revenue/Advertiser 1.1
- **Balanced:** Retention 75%, New Acquisition 3,500, Revenue/Advertiser 1.05

**Key Insight:** All three levers matter. Balancing retention + acquisition + upsell is the path to $500M+ H2 2026 revenue.

---

### 5. Cohort Retention Analysis
**Purpose:** Track how advertiser cohorts (groups by first appearance month) retain over time

**Key Features:**
- **Cohort Heatmap:** Month-by-month retention rates for H2 2024 vs H2 2025 cohorts
- **Month 1 Retention KPI Cards:** 83.5% (H2 2024) vs 41.8% (H2 2025) with -41.7% churn gap
- **Dimensional Drill-Down:** Apply filters (Segment, Vertical, Location, Ad Type) to see cohort retention within specific dimensions
- **Context Filters:** Filters operate at the context level to show retention patterns for subsets of your advertiser base

**How to Use:**
1. Review the KPI cards at the top showing month-1 retention rates and the churn gap
2. Examine the heatmap to see retention decay over months
3. Apply dimensional filters to identify where churn is concentrated (which segments, verticals, geographies)
4. Darker blue = higher retention; lighter colors = higher churn
5. Note: H2 2024 cohort has 6 months of data; H2 2025 cohort has up to 3 months (data through Dec 2025)

**Understanding the Data:**
- **H2 2024 Cohort:** Advertisers who first appeared July-Dec 2024; tracked through Dec 2025 (12+ months follow-up)
- **H2 2025 Cohort:** Advertisers who first appeared July-Dec 2025; tracked through Dec 2025 (max 3-6 months follow-up)
- Rows show each cohort; Columns show months since first appearance

**Key Insight:** New advertiser cohorts (H2 2025) have severe month-1 churn (58% drop vs 16% for H2 2024). This is the core constraint driving the growth paradox. Early-stage advertiser experience and onboarding are critical leverage points for improving overall retention and revenue per advertiser.

**Actionable Takeaway:** Focus resources on month 1-2 retention for newly acquired accounts. Segment and geographic filters reveal where churn concentration is highest — start retention initiatives there first.

---

## Filter & Parameter Guide

### Filters (Top of each tab)
- **Year:** 2024 or 2025
- **Month Start / Month End:** July-December range
- **Ad Type, Segment, Industry Vertical, Advertiser Location:** Click charts to filter
- **Top N Advertisers:** 5-20 slider on Summary tab

### Parameters
- All tabs use the same Year and Month parameters for consistency
- Scenario Planning has three additional parameters for what-if modeling
- Changes to parameters update all visualizations in real-time

---

## Data Notes

- **Source:** H2 2024 and H2 2025 (July-December each year)
- **Grain:** Monthly revenue by advertiser, location, vertical, segment, and ad type
- **Calculations:** All YoY comparisons, forecasts, and projections are automated and recalculate with filter/parameter changes
- **RFM Methodology:** Based on last activity month, number of active months, and total revenue in the period

---

## Key Takeaways

1. **Growth Paradox:** Advertiser count growing 22% YoY while revenue grows only 6%
2. **Concentration Risk:** Champions segment generates 93% of revenue (1,692 advertisers)
3. **New Customer Quality:** New advertiser acquisition is working but bringing smaller accounts ($650 avg vs. $88K for Champions)
4. **Opportunity:** Retention improvements and revenue per advertiser growth can close the gap to 71% H2 2026 revenue growth

---

## Questions?

For detailed methodology, SQL queries, and calculated field definitions, see the GitHub repository.
