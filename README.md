# AtliQ-Hospitality-Analytics

## Executive Summary

This project delivers a comprehensive Power BI analytics solution for AtliQ Grands, a luxury hotel chain experiencing market share decline due to competitive pressures and data-driven decision-making gaps. The dashboard provides real-time insights into key revenue metrics, occupancy patterns, and booking trends across 25 properties in 4 cities. Analysis reveals an overall occupancy rate of 57.9% with revenue of ₹1.71bn, alongside critical opportunities to optimize weekend performance (73.6% occupancy) and improve ADR metrics (currently at 12.7K with a -0.2% decline).

**You can explore the interactive Power BI dashboard here :** 👉 [**Live Dashboard**](https://app.powerbi.com/view?r=eyJrIjoiY2MwNDk2NmQtYWJjYy00ZmYwLTg4NzQtZmU4ZmNkYzcyOGRjIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## Business Problem

AtliQ Grands, a prominent player in India's luxury hospitality sector for 20 years, is losing market share and revenue to competitors who have adopted data-driven strategies. Without an in-house analytics team, the organization lacks visibility into:

- Revenue performance trends and booking patterns across properties
- Occupancy optimization opportunities by day type and platform
- Property-level performance benchmarking and rating impacts
- Strategic pricing decisions to improve Average Daily Rate (ADR) and RevPAR

The revenue management team requires actionable insights from historical data to reverse declining market position and regain competitive advantage.

## Project Background

AtliQ Grands operates five-star properties across Mumbai, Bangalore, Hyderabad, and Delhi in two segments: Business and Luxury. The company engaged external analytics expertise to transform raw booking data into strategic intelligence. This project encompasses data from multiple properties across Q2-Q3, analyzing booking patterns, revenue metrics, cancellations, and customer ratings to identify performance drivers and improvement opportunities.

## Methodology

### Analytical Framing

The analysis follows a multi-dimensional approach examining performance across:
- **Temporal Analysis**: Week-over-week trends, weekend vs. weekday patterns
- **Property Segmentation**: City-wise, property-wise, and room class comparisons
- **Revenue Metrics**: ADR, RevPAR, Occupancy %, Realization %, and DSRN tracking
- **Channel Performance**: Booking platform effectiveness and direct vs. online dynamics
- **Operational Efficiency**: Cancellation rates, no-show patterns, and capacity utilization

Key metrics were defined per stakeholder requirements, including custom KPIs like DBRN (Daily Booked Room Nights), DSRN (Daily Sellable Room Nights), DURN (Daily Utilized Room Nights), and Realization % to provide granular operational visibility.

## Tools & Analytical Skills Applied

**Technologies Used**
- **Power BI Desktop** - Primary platform for data modeling, visualization, and dashboard development
- **DAX (Data Analysis Expressions)** - Advanced calculations for dynamic metrics, WoW%, MoM changes, and custom KPIs
- **Power Query** - Data transformation, cleansing, and ETL operations
- **Excel** - Initial data processing and validation

**Analytical Techniques**
- Star schema data modeling with fact and dimension table relationships
- Comparative analysis (weekend vs. weekday, platform performance, property benchmarking)
- Trend analysis with percentage change calculations
- Segmentation analysis by city, property, room class, and booking channel
- Performance variance identification and outlier detection
- Interactive visualizations with drill-through capabilities and cross-filtering
- Custom tooltips and parameter-based week selection functionality


## Results & Business Recommendations

### Key Findings

1. **Revenue Concentration**: Mumbai leads with ₹668.6M (39% of total), while Delhi underperforms at ₹294.5M despite having comparable properties
2. **Platform Dependency**: 41% of bookings come from "others" platform, with direct offline at 20% and makeyourtrip at 7%—revealing over-reliance on third-party channels
3. **Weekend Premium Opportunity**: Weekend occupancy (73.6%) significantly exceeds weekday (51.3%), but ADR shows minimal premium (₹12,724 vs ₹12,680)
4. **Cancellation Impact**: 24.8% cancellation rate represents substantial revenue leakage across 33.4K cancelled bookings
5. **Property Performance Variance**: Atliq Exotica Mumbai leads with ₹106M revenue, while some properties show high ratings (4.3) but suboptimal revenue conversion

### Strategic Recommendations

1. **Dynamic Pricing Strategy**: Implement weekend pricing premiums to capitalize on 73.6% occupancy—potential for 10-15% ADR increase on weekends could yield ₹50M+ additional annual revenue

2. **Direct Booking Incentives**: Reduce third-party platform dependency (currently 41%) through loyalty programs and direct booking discounts—target 30% reduction in platform fees within 12 months

3. **Underperforming Property Intervention**: Deploy Mumbai's best practices to Delhi properties; focus on Atliq Blu properties showing 65.8% occupancy with improvement potential to benchmark levels

4. **Cancellation Mitigation**: Implement stricter cancellation policies for peak periods and introduce tiered deposit structures—target 5% reduction in cancellation rate for ₹35M revenue protection

5. **Luxury Segment Expansion**: With Business segment showing 61.6% revenue share, strategically increase Luxury positioning in high-performing cities where ratings support premium pricing

6. **Revenue Management System**: Invest in automated dynamic pricing based on real-time occupancy, competitor rates, and demand forecasting to optimize ADR and RevPAR metrics continuously

### Projected Impact

Full implementation of these recommendations could potentially increase revenue by 15-20% (₹255-340M) and improve market positioning within 12-18 months, recovering lost market share in the luxury hospitality segment.

## Dashboard Preview

![Dashboard Overview]([screenshots/dashboard_overview.png](https://github.com/swarajkawale019/AtliQ-Hospitality-Analysis/blob/0c42188bf31109923cadf6cfadf359f506db11d4/visuals/Screenshot%20(131).png))
![Property Analysis]([screenshots/property_analysis.png](https://github.com/swarajkawale019/AtliQ-Hospitality-Analysis/blob/0c42188bf31109923cadf6cfadf359f506db11d4/visuals/Screenshot%20(132).png))


## Key Metrics Defined

- **Revenue**: Total revenue realized from successful bookings
- **RevPAR** (Revenue Per Available Room): Revenue / Total room capacity
- **ADR** (Average Daily Rate): Revenue / Total bookings
- **DSRN** (Daily Sellable Room Nights): Total room inventory available daily
- **DBRN** (Daily Booked Room Nights): Total rooms booked daily
- **DURN** (Daily Utilized Room Nights): Total rooms utilized (check-out completed)
- **Occupancy %**: DBRN / DSRN
- **Realization %**: DURN / DBRN (successful checkouts vs bookings)
- **Cancellation %**: Cancelled bookings / Total bookings
- **No Show Rate %**: No-show bookings / Total bookings


**You can explore the interactive Power BI dashboard here :** 👉 [**Live Dashboard**](https://app.powerbi.com/view?r=eyJrIjoiY2MwNDk2NmQtYWJjYy00ZmYwLTg4NzQtZmU4ZmNkYzcyOGRjIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)
