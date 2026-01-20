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

## Insights Deep Dive

### Revenue Performance Analysis:

* **Mumbai dominates revenue contribution with ₹668.6M (39% of total revenue).** The city shows strong performance across both Luxury and Business segments, with Atliq Exotica Mumbai leading individual property performance at ₹106M. This concentration indicates Mumbai as the flagship market requiring continued investment and expansion.

* **Delhi significantly underperforms at ₹294.5M despite having comparable property count.** Delhi properties show lower occupancy (60.5%) and ADR compared to Mumbai (57.9% occupancy), suggesting market-specific challenges or suboptimal pricing strategies that need immediate attention.

* **Business category contributes 61.6% of total revenue (₹1.09B) compared to Luxury at 38.4%.** This revenue mix indicates AtliQ Grands' strong positioning in the business travel segment, but also reveals untapped potential in the higher-margin luxury segment where competition may be less intense.

* **Week-over-week revenue shows -81.7% decline, while RevPAR increased 27.8%.** This apparent contradiction suggests a significant reduction in available inventory or operational days in recent weeks, while pricing efficiency improved substantially, requiring investigation into capacity utilization strategies.


### Occupancy & Pricing Optimization:

* **Weekend occupancy (73.6%) significantly exceeds weekday occupancy (51.3%) by 22.3 percentage points.** This 43% higher weekend demand presents a clear opportunity for premium pricing strategies, yet current ADR shows minimal differentiation (₹12,724 weekend vs ₹12,680 weekday), leaving substantial revenue on the table.

* **Overall occupancy of 57.9% suggests moderate capacity utilization with room for improvement.** Industry benchmarks for luxury hotels typically range 65-75%, indicating AtliQ Grands is underperforming by 7-17 percentage points, representing potential revenue loss of ₹120-290M annually at current ADR levels.

* **ADR declined by -0.2% to ₹12.7K, while realization percentage stands at 70.1%.** The declining ADR trend coupled with 30% revenue leakage (unrealized bookings) indicates pricing pressure and operational inefficiencies in converting bookings to successful check-ins, directly impacting bottom-line performance.

* **Premium and Presidential room classes show highest pricing power but lower occupancy.** These high-value segments require targeted marketing to business executives and luxury travelers, with potential bundle offerings combining room upgrades with amenity packages to drive occupancy without diluting ADR.


### Booking Channel Performance:

* **"Others" platform dominates with 41% booking share, creating excessive platform dependency.** This over-reliance on unspecified third-party channels exposes AtliQ Grands to high commission costs (typically 15-25%) and limited customer data access, reducing profitability and customer relationship building opportunities.

* **Direct offline bookings contribute only 20% despite typically offering highest margins.** The underutilization of direct channels represents missed opportunities for commission savings (₹51-85M annually) and direct customer engagement, suggesting inadequate investment in sales teams or corporate account management.

* **MakeYourTrip accounts for just 7% while other major OTAs show minimal contribution.** The fragmented channel mix across multiple small platforms increases operational complexity and negotiation leverage challenges, while potentially missing strategic partnerships with dominant OTAs offering better visibility.

* **Platform-wise performance varies significantly with "journey" showing 70.5% realization vs others at 70.3%.** These minor realization differences suggest relatively consistent quality across channels, but deeper analysis of customer lifetime value and repeat booking rates by channel could reveal more strategic insights.


### Operational Efficiency:

* **24.8% cancellation rate represents 33.4K cancelled bookings and substantial revenue leakage.** At current ADR levels, this translates to approximately ₹425M in lost potential revenue annually, with peak periods likely experiencing even higher cancellation rates requiring immediate policy intervention.

* **Realization percentage of 70.1% indicates that only 70% of bookings convert to successful check-ins.** The 30% gap between bookings and realizations (combining cancellations and no-shows) suggests inadequate booking policies, lack of advance deposits, or overly lenient cancellation terms compared to industry standards.

* **Average rating of 3.6 across properties indicates moderate customer satisfaction with improvement potential.** While not critically low, this rating sits below luxury hotel benchmarks (typically 4.2-4.5), potentially impacting repeat bookings and OTA search rankings, requiring focused quality enhancement initiatives.

* **Properties with highest ratings (4.3) don't necessarily generate highest revenue.** This disconnect between customer satisfaction and revenue performance suggests pricing strategies aren't optimized for quality perception, or high-rated properties are in lower-demand markets requiring rebalanced marketing investment allocation.


## Recommendations:

Based on the insights and findings above, I would recommend the Revenue Management Team to consider the following:

* Weekend occupancy reaches 73.6% while weekday occupancy sits at 51.3%, yet pricing shows minimal differentiation. **Implement dynamic weekend pricing with 10-15% premiums during high-demand periods (Friday-Sunday), projected to generate additional ₹50M+ annually while maintaining occupancy levels above 70%.**

* 41% of bookings come through "others" platform, incurring substantial commission costs while limiting direct customer relationships. **Launch a "Book Direct & Save" campaign offering 10% discounts for direct bookings, invest in SEO/SEM for brand.com visibility, and develop a loyalty program targeting business travelers - aim to shift 30% of third-party bookings to direct channels within 12 months, saving ₹40-50M in commissions.**

* Delhi properties underperform Mumbai despite similar market potential, showing opportunity gaps in pricing and operations. **Deploy Mumbai's revenue management best practices to Delhi properties, conduct competitor pricing analysis, and implement targeted corporate sales programs for Delhi's strong business travel market - target 15-20% revenue growth in Delhi within 6 months.**

* 24.8% cancellation rate and 70.1% realization percentage indicate significant revenue leakage from booking to check-in conversion. **Introduce tiered cancellation policies with 20% non-refundable deposits for peak periods, implement 72-hour advance cancellation requirements, and offer "flexible rate" vs "advance purchase" pricing tiers - projected 5% reduction in cancellations could protect ₹35M in annual revenue.**

* Business segment contributes 61.6% of revenue while Luxury segment (higher margin) remains underdeveloped at 38.4%. **Increase luxury segment marketing investment in high-performing cities (Mumbai, Bangalore), develop premium packages targeting leisure travelers and celebrations, and enhance luxury property amenities to justify price premiums - target luxury revenue growth from 38% to 45% of total mix.**

* Current ADR of ₹12.7K shows -0.2% decline while occupancy remains moderate at 57.9%, suggesting suboptimal revenue management. **Invest in automated revenue management system (RMS) implementing real-time dynamic pricing based on demand forecasting, competitor rates, and booking pace - successful RMS implementation typically yields 5-10% revenue improvement (₹85-170M annually).**

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
