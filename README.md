Equipment Failure & Predictive Maintenance Analysis

Project Overview
This project analyses equipment operating conditions, failures, and downtime to identify patterns that can support proactive maintenance decisions.
The analysis combines SQL, Power Query, Power BI and DAX to transform equipment data into operational and predictive maintenance insights.
The project focuses on understanding equipment performance, identifying failure patterns, evaluating operating conditions, and highlighting early indicators that may require maintenance attention.

Business Problem

Unplanned equipment failures can lead to production downtime, increased maintenance costs, reduced equipment availability, and operational inefficiencies.
A maintenance team needs more than a record of previous failures. It needs to understand:
- Which equipment experiences the greatest failure or downtime exposure?
- What operating conditions are associated with equipment problems?
- Which equipment shows elevated operating conditions?
- Are operating conditions becoming more demanding over time?
- Which assets may require closer monitoring or preventive intervention?

This project uses historical equipment observations to provide a data-driven view of these questions.
Project Objectives

The main objectives were to:
- Analyse equipment operating conditions and performance.
- Identify failure and downtime patterns.
- Diagnose equipment with higher maintenance exposure.
- Analyse relationships between operating variables and equipment condition.
- Develop predictive/condition indicators for maintenance monitoring.
- Provide actionable insights that can support preventive maintenance decisions.

Dataset
The dataset contains observations for:
- 50 equipment assets
- 12-day observation period (15000 rows)

The dataset includes equipment operating and maintenance-related variables such as:
- Temperature
- Vibration
- Pressure
- Humidity
- Energy Consumption
- Failure information
- Downtime
- Equipment condition indicators
- Remaining-life/risk-related measures

The analysis is based on the available observation period and should therefore be interpreted as a condition-monitoring analysis rather than a long-term failure prediction model.

Tools & Technologies

SQL
Used for querying, filtering, aggregating and analysing the equipment data before dashboard development.

Power Query
Used for data cleaning, transformation and preparation.

Power BI
Used to build the interactive dashboards and communicate equipment performance and maintenance insights.

DAX
Used to create calculated measures, KPIs and derived analytical indicators.


Project Workflow
The project followed a data-to-insight workflow:

SQL → Power Query → Power BI/DAX → Equipment Analysis → Maintenance Insights

1. Data Analysis with SQL
The equipment data was queried and analysed to understand equipment behaviour, failures, downtime and operating conditions.

2. Data Preparation with Power Query
The data was cleaned, transformed and structured for analysis.

3. Data Modelling & Analysis
The prepared data was loaded into Power BI, where calculated measures and analytical indicators were developed using DAX.

4. Dashboard Development
Interactive dashboards were created to move from overall equipment performance to failure diagnosis and predictive maintenance analysis.

Dashboard Structure

1. Equipment Overview
Provides a high-level view of equipment performance and maintenance exposure.

The page helps identify:
- Overall equipment condition
- Failure patterns
- Downtime exposure
- Equipment requiring attention

2. Failure Diagnosis
Focuses on understanding where and how equipment failures occur.

The analysis examines:
- Failure frequency
- Downtime
- Equipment-level performance
- Operating conditions
- Failure patterns across equipment categories

3. Predictive Maintenance
The predictive maintenance analysis focuses on identifying equipment conditions that may indicate increased maintenance attention.

Rather than relying only on historical failure counts, the analysis incorporates operating variables such as:
- Temperature
- Vibration
- Pressure
- Humidity
- Energy Consumption

Derived condition indicators are used to identify elevated or changing operating conditions.

Predictive & Condition Indicators
The predictive analysis includes derived indicators designed to provide additional information about equipment condition.

Operating Stress
Operating variables are combined after accounting for differences in their measurement scales to identify equipment operating under relatively higher overall stress.

Temperature Deviation
Temperature is compared with the observed operating baseline to identify equipment operating significantly above the overall temperature level.

Elevated Operating Conditions
Multiple operating variables are evaluated together to identify observations where several conditions are simultaneously elevated.

Operating Condition Change
Changes in operating conditions across the observation period are analysed to identify whether equipment conditions are increasing, stable or decreasing.
These indicators are intended to support condition monitoring and maintenance prioritisation, rather than claim certainty that a specific equipment failure will occur.

Key Findings
The dashboard analysis identified differences in equipment operating conditions and maintenance exposure across the observed assets.
The analysis showed that some equipment exhibited relatively higher operating temperatures and/or other elevated operating conditions compared with the broader equipment population.
The predictive analysis was then used to identify equipment requiring closer monitoring based on combinations of operating conditions rather than relying on a single KPI.


Maintenance Recommendations

Based on the analysis, maintenance teams can use the identified condition indicators to:
- Prioritise equipment for inspection.
- Investigate assets showing multiple elevated operating conditions.
- Monitor equipment with increasing operating-condition trends.
- Investigate abnormal temperature or vibration behaviour.
- Combine condition indicators with historical failure and downtime information when prioritising maintenance activities.
- Use continuous monitoring data to improve future predictive maintenance models.

Project Limitations
The analysis is based on a 12-day observation period.

Therefore:
- The results represent the conditions observed during the available period.
- The derived indicators should not be interpreted as guaranteed failure predictions.
- Longer historical datasets would provide stronger evidence for identifying long-term trends.
- Additional variables could improve future predictive modelling.

Future Improvements
Future development could include:
- Longer historical equipment datasets.
- Real-time sensor data integration.
- Machine learning-based failure prediction.
- More advanced remaining useful life modelling.
- Automated maintenance alerts.
- Integration of maintenance work-order history.
- Additional equipment health and sensor variables.
- Model validation using future failure events.

Conclusion
This project demonstrates how SQL, Power Query, Power BI and DAX can be combined to transform equipment data into practical maintenance insights.
The analysis moves beyond simply reporting historical failures by examining equipment operating conditions and developing additional condition indicators that can help identify assets requiring closer monitoring.
The overall objective is to support a more data-driven and proactive approach to equipment maintenance and operational decision-making.
