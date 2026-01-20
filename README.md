# AtliQ-Hospitality-Analytics

## Project Background

AtliQ Grands is a prominent luxury/business hotel chain operating across India for the past 20 years. The company owns multiple five-star properties in key metropolitan cities including Mumbai, Bangalore, Hyderabad, and Delhi, serving both business and leisure travelers. However, due to strategic moves from competitors and ineffective decision-making in management, AtliQ Grands has been experiencing a decline in market share and revenue in the luxury/business hotels category.

This project aims to incorporate "Business and Data Intelligence" to help the organization regain its competitive position. The company operates under two property categories (Luxury and Business) with key business metrics focused on revenue optimization, occupancy rates, and pricing strategies.

Insights and recommendations are provided on the following key areas:

- **Revenue Performance Analysis:** City-wise and property-wise revenue distribution and trends
- **Occupancy & Pricing Optimization:** Weekend vs. weekday patterns, ADR, and RevPAR analysis
- **Booking Channel Performance:** Platform-wise contribution and direct vs. third-party bookings
- **Operational Efficiency:** Cancellation rates, realization percentages, and customer ratings impact

The Power BI dashboard with interactive visualizations can be found here 👉 [**Live Dashboard**](https://app.powerbi.com/view?r=eyJrIjoiY2MwNDk2NmQtYWJjYy00ZmYwLTg4NzQtZmU4ZmNkYzcyOGRjIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9).

## Methodology

Analyzed historical booking data (May–July 2022) from five interconnected tables using Power BI. Cleaned and transformed data with Power Query, designed an optimized star schema data model, and developed 25+ DAX measures covering revenue, occupancy, pricing, utilization, and realization metrics aligned with hospitality industry standards. Implemented time intelligence for week-on-week trend analysis and built an interactive dashboard following stakeholder mock-ups, enabling performance monitoring across cities, properties, room categories, and booking platforms to support data-driven revenue optimization.

## Data Structure & Initial Checks

AtliQ Grands' database structure consists of five tables with a star schema design, containing booking and property data from May 2022 to July 2022. The total dataset comprises 134,590 booking records across 25 properties. A description of each table is as follows:

- **dim_date:** Contains date-related information including day type (weekend/weekday), week number, and month-year identifiers
- **dim_hotels:** Property master data including property ID, property name, category (Luxury/Business), and city location
- **dim_rooms:** Room classification data with room ID and room class types (Standard, Elite, Premium, Presidential)
- **fact_bookings:** Granular booking-level data including booking ID, property ID, booking dates, guest count, room category, booking platform, ratings, booking status, revenue realized, and check-in/check-out dates
- **fact_aggregated_bookings:** Pre-aggregated data showing successful bookings and capacity by property, room category, and check-in date for performance tracking

![Image](https://github.com/swarajkawale019/AtliQ-Hospitality-Analysis/blob/75ca1352c84b6c0df164c335ed1a211d390a328b/data_model.png)

## Executive Summary

### Overview of Findings

AtliQ Grands generated ₹1.71 billion in revenue across 134.6K bookings with an overall occupancy rate of 57.9% during the analysis period. Mumbai emerges as the strongest market contributing 39% of total revenue, while significant opportunities exist in weekend pricing optimization (73.6% occupancy with minimal premium), reducing platform dependency (41% from third-party channels), and addressing the 24.8% cancellation rate. The analysis reveals a performance gap between cities and properties that can be bridged through data-driven revenue management strategies.

![Dashboard Overview](https://github.com/swarajkawale019/AtliQ-Hospitality-Analysis/blob/main/visuals/Screenshot%20(131).png?raw=true)



![Dashboard](https://github.com/swarajkawale019/AtliQ-Hospitality-Analysis/blob/main/visuals/Screenshot%20(132).png?raw=true)

## Insights Deep Dive

### Revenue Performance Analysis
- **Mumbai is the primary revenue driver (₹668.6M, 39%)**, clearly outperforming other cities and justifying continued investment focus.
- **Delhi underperforms at ₹294.5M despite similar scale**, indicating pricing and demand-side inefficiencies rather than capacity issues.
- **Business hotels contribute 61.6% of total revenue**, confirming strong business travel positioning but highlighting missed luxury upside.

### Occupancy & Pricing Optimization
- **Weekend occupancy (73.6%) far exceeds weekdays (51.3%)**, yet ADR remains nearly flat, resulting in avoidable revenue loss from weak dynamic pricing.
- **Overall occupancy of 57.9% is below industry benchmarks (65–75%)**, reflecting inefficient capacity utilization.
- **Premium and Presidential rooms show high pricing power but low occupancy**, signaling targeting and packaging gaps rather than pricing issues.

### Booking Channel Performance
- **Over-reliance on “Others” channels (41%)** increases commission costs and limits customer ownership.
- **Direct bookings contribute only 20%**, representing a significant missed margin opportunity.
- **Fragmented OTA presence** reduces negotiation leverage and visibility on high-impact platforms.

### Operational Efficiency
- **High cancellation rate (24.8%) translates to ~₹425M in potential revenue loss**, driven by lenient booking and cancellation policies.
- **Only 70.1% of bookings convert to stays**, confirming major leakage from cancellations and no-shows.
- **Average customer rating of 3.6 is below luxury benchmarks**, negatively impacting demand, rankings, and repeat business.

## Recommendations

- **Action:** Implement demand-based weekend pricing with 10–15% premiums during Friday–Sunday peak periods.  
  **Expected Impact:** Higher RevPAR with potential ₹50M+ incremental annual revenue without increasing capacity.

- **Action:** Shift bookings from third-party platforms to direct channels through “Book Direct & Save” offers, SEO/SEM investment, and loyalty programs.  
  **Expected Impact:** Reduction in commission costs with ₹40–50M annual savings (directional estimate).

- **Action:** Apply Mumbai’s revenue management practices to Delhi properties, supported by competitor pricing analysis and targeted corporate sales initiatives.  
  **Expected Impact:** 15–20% revenue uplift in Delhi over the short to medium term.

- **Action:** Introduce tiered cancellation policies, advance-purchase rates, and partial non-refundable deposits during high-demand periods.  
  **Expected Impact:** A 5% reduction in cancellations could protect approximately ₹35M in annual revenue.

- **Action:** Increase focus on the Luxury segment through premium packages, targeted leisure marketing, and enhanced amenity positioning in high-performing cities.  
  **Expected Impact:** Shift luxury revenue mix from 38% to ~45%, improving overall margins.

- **Action:** Deploy an automated Revenue Management System (RMS) for real-time dynamic pricing based on demand forecasts and booking pace.  
  **Expected Impact:** Typical RMS adoption delivers 5–10% revenue improvement (₹85–170M annually, directional).


### Projected Impact

Full implementation of these recommendations could potentially increase revenue by 15-20% (₹255-340M) and improve market positioning within 12-18 months, recovering lost market share in the luxury hospitality segment.


## Tools & Technologies Used

**Technologies**
- **Power BI Desktop** - Primary platform for data modeling, visualization, and dashboard development
- **DAX (Data Analysis Expressions)** - Advanced calculations for dynamic metrics, WoW%, MoM changes, and custom KPIs
- **Power Query** - Data transformation, cleansing, and ETL operations
- **Excel** - Initial data processing and validation

**Analytical Techniques**
- Star schema data modeling with fact and dimension table relationships
- Time-series analysis for trend identification and WoW/MoM comparisons
- Comparative segmentation analysis (city, property, room class, booking channel)
- Performance benchmarking and variance analysis
- Interactive drill-through visualizations with dynamic filtering

## Key Metrics Defined

- **Revenue**: Total revenue realized from successful bookings (revenue_realized)
- **RevPAR** (Revenue Per Available Room): Revenue generated per available room = Total Revenue / Total Available Room Nights
- **ADR** (Average Daily Rate): Average revenue per sold room = Total Revenue / Total Bookings
- **DSRN** (Daily Sellable Room Nights): Total room inventory available for sale on a given day
- **DBRN** (Daily Booked Room Nights): Total rooms booked on a given day
- **DURN** (Daily Utilized Room Nights): Total rooms where guests completed check-out (successful stays)
- **Occupancy %**: Percentage of available rooms that were booked = (DBRN / DSRN) × 100
- **Realization %**: Percentage of bookings that converted to successful stays = (DURN / DBRN) × 100
- **Cancellation %**: Percentage of total bookings that were cancelled = (Cancelled Bookings / Total Bookings) × 100
- **No Show Rate %**: Percentage of bookings where guests didn't arrive = (No-Show Bookings / Total Bookings) × 100

**You can explore the interactive Power BI dashboard here :** 👉 [**Live Dashboard**](https://app.powerbi.com/view?r=eyJrIjoiY2MwNDk2NmQtYWJjYy00ZmYwLTg4NzQtZmU4ZmNkYzcyOGRjIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)
