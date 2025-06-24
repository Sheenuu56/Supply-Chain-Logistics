Exploratory Data Analysis (EDA) Report: Logistics Dataset

1. Objective
The goal of this project is to analyse logistics data to identify factors contributing to delays and propose actionable recommendations for operational improvements. This analysis focuses on exploring relationships between traffic conditions, shipment statuses, user behaviour, and time-based trends to optimise logistics efficiency.

2. Dataset Overview
* Dataset Size: 1000 rows, 21 columns (cleaned version)
* Key Features:
    * Traffic_Status: Levels of traffic (Clear, Detour, Heavy)
    * Waiting_Time: Time in minutes before a shipment is processed
    * Shipment_Status: Delivery status (Delivered, In-Transit, Delayed)
    * Logistics_Delay_Reason: Reasons for delays (e.g., Traffic, Weather)
    * Inventory_Level: Stock levels in units
    * Temperature and Humidity: Weather conditions
    * User_Purchase_Frequency and User_Transaction_Amount: Metrics reflecting customer engagement
    * Asset_Utilisation: Measures how effectively logistics assets are being used
    * Demand_Forecast: Predicted demand for products or services
    * Timestamp: Includes Date, Time, Month, Weekday, and Hour for time-based analysis

3. Key Insights from EDA

3.1 Univariate Analysis

* Traffic Status Distribution:
    * Majority of shipments occurred under Detour Traffic conditions, with very close instances of Low Traffic and High Traffic.
    * Action: Focus route optimisations on periods of high traffic to minimise delays.
* Waiting Time Distribution:
    * Waiting times ranged from 10 to 60 minutes, with peaks at specific intervals (e.g., 20, 50 minutes).
    * Action: Investigate operational factors contributing to peak intervals.
* Logistics Delay Reasons:
    * Weather emerged as the most frequent cause of delays, followed by Traffic and Mechanical failure conditions.
    * Action: Prioritise mitigation strategies for weather-related delays.
* Shipment Status:
    * Majority of shipments were delayed pointing to bottlenecks that need addressing.
    *  Action: Analyse the factors contributing to them (e.g., traffic, time of day).


3.2 Bivariate Analysis
* Traffic Status vs. Waiting Time:
    * Longer waiting times were positively correlated with High Traffic levels.
    * Action: Schedule deliveries during low-traffic periods where possible.
* Shipment Status vs. User Purchase Frequency:
    * Delayed shipments were associated with reduced purchase frequency, highlighting potential customer dissatisfaction.
    * Action: Minimise delays to maintain customer loyalty.
* Hour of Day vs. Waiting Time:
    * Peak waiting times were observed during specific hours (e.g., 7-8 AM, 5-7 PM) and a sudden rush during 2 PM, corresponding to typical rush hours.
    * Action: Allocate additional resources during peak hours to improve efficiency.
* Inventory Level vs. Waiting Time:
    * Delays were more frequent at low inventory levels, suggesting insufficient stock planning.
    * Action: Balance inventory levels to reduce delays.


3.3 Time-Based Trends
* Daily Waiting Times:
    * Delays peaked on specific days, potentially aligning with operational workflows or external factors like weather or traffic patterns.
    * Action: Redistribute resources to address high-delay days effectively.
* Monthly Trends:
    * Certain months showed higher delay frequencies, potentially due to seasonal demand spikes.
    * Action: Plan for increased demand during peak months.


3.4 Correlation Heatmap
* Most features showed weak correlations (<0.1), indicating potential independence between variables except for Logistics Delay with Traffic Status indicating the strong dependence between the two.
* Action: Explore non-linear relationships or feature interactions for deeper insights.


4. Recommendations
1. Traffic Optimisation:
    * Utilise predictive traffic monitoring to identify and avoid congested routes.
    * Leverage GPS-based dynamic routing systems to suggest alternate pathways during high-traffic periods.
2. Operational Adjustments:
    * Redistribute resources to address peak times and days with high delays.
    * Implement a real-time tracking system to monitor delays and adjust schedules proactively.
3. Customer-Centric Strategies:
    * Prioritise shipments for high-value or frequent customers to maintain loyalty.
    * Offer compensations or incentives for delayed deliveries to retain customer trust.
4. Focus on Delay Reasons:
    * Mitigate the most frequent causes of delays (e.g., traffic) through targeted interventions such as predictive analytics and collaboration with local authorities.
    * Address operational inefficiencies by standardising processes and conducting staff training.
5. Advanced Analysis:
    * Conduct clustering or regression analysis to uncover hidden patterns and relationships.
    * Integrate time-series forecasting to predict high-demand periods and plan resources accordingly.
6. Weather-Related Recommendations:
    * Implement predictive analytics using historical weather data to anticipate delays and adjust schedules proactively.
    * Introduce contingency plans, such as alternative routes or additional delivery time buffers, for regions prone to severe weather conditions.
    * Collaborate with meteorological services for real-time weather updates to dynamically optimise logistics operations.


5. Next Steps
1. Dashboard Creation:
    * Develop an interactive dashboard using tools like Power BI, Tableau, or Python libraries to visualise key metrics dynamically.
2. Predictive Model (Optional):
    * Build a model to forecast logistics delays based on current and historical data.
    * Consider features like traffic status, time of day, and inventory levels for model training.
3. Report and Presentation:
    * Use this analysis to inform stakeholders and guide decision-making.
    * Prepare a polished presentation with visual aids (charts, graphs) to communicate insights effectively.
