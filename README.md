## Cybersecurity-Risk-Tracker
A Power BI dashboard that visualizes and tracks cybersecurity incidents by severity, threat type, response time, and department impact.
## Overview
This Power BI dashboard project is designed to monitor, analyze, and visualize cybersecurity incidents within an organization. It provides valuable insights into threat types, severity levels, response times, and the operational impact across departments.
## Dataset Description
File Used: cyber_incidents.csv
The dataset contains the following key fields:
Incident_ID: Unique identifier for each incident
Date & Time: When the incident was detected
Threat_Type: Type of cybersecurity threat (e.g., Malware, Phishing)
Severity_Level: Critical, High, Medium, Low
Status: Resolved or In Progress
Response_Time_mins: Time taken to resolve the issue
Department: Department affected
A calculated column was added to combine Date and Time as Detected_Timestamp.
## Objectives
1)Track total and resolved cybersecurity incidents
2)Analyze threat types and their severity
3)Measure and visualize average response times
4)Identify departments most affected by threats
5)Enable filtering by incident date for deeper analysis
## Dashboard Features
## KPI Cards
1)Total Cyber Incidents: Displays total number of incidents
2)Resolved Incidents: Count of incidents marked as resolved
3)Departments Affected: Number of departments impacted
4)Avg. Response Time (in mins): Average of the Response_Time_mins column
## Daily Trends - Incidents vs Response Time
1)Visual: Line and Clustered Column Chart
2)X-Axis: Day (from Detected_Timestamp)
3)Bars: Count of Incident_ID
4)Line: Sum of Response_Time_mins
5)Shows correlation between volume and response efficiency over time
## Threat Types Breakdown by Severity
1)Visual: Stacked Column Chart
2)X-Axis: Threat_Type
3)Legend: Severity_Level
4)Compares the impact of various threats by severity
## Incidents by Severity (Donut Chart)
Shows overall proportion of incidents based on severity levels (Critical, High, Medium, Low)
## Incident Status by Department
1)Visual: Stacked Bar Chart
2)X-Axis: Count of Incident_ID
3)Y-Axis: Department
4)Legend: Status
5)Helps identify which departments are most vulnerable and how efficiently issues are resolved
## Date Filter (Slicer)
Users can filter the entire dashboard based on the selected incident date(s)
## DAX Measures Used
Resolved_Incidents = CALCULATE(COUNT('cyber_incidents'[Incident_ID]), 'cyber_incidents'[Status] = "Resolved")
Avg_Response_Time_mins = AVERAGE('cyber_incidents'[Response_Time_mins])
## Design and Theme
Theme: Dark Blue Background for better contrast
## Colors:
1)Critical: Red
2)High: Orange
3)Medium: Yellow
4)Low: Green
5)Status: In Progress (Blue), Resolved (Purple)
6)Font: Light-colored text for better readability
## Tools Used
1)Power BI Desktop
2)Excel (For Incident data)
## Conclusion
This dashboard provides a clear and actionable overview of cybersecurity incidents. It helps in identifying high-risk areas, reducing response times, and allocating resources more effectively.
## Files:
1)dashboard.pbix – https://1drv.ms/u/c/6ee679fb17cb7e45/EWpVaqjaq9NErNb3fXPYsjwBAiA8_Mdyeuc0TXe27yyBUA?e=Bc9NOy
2)dashboard.png – https://1drv.ms/i/c/6ee679fb17cb7e45/EXj7AzLP3DBMuRbkbZPRXX4BPtwnPw9ggG1n4NqLpgb11Q?e=ziqy9n
3)incident_data.xlsx – https://1drv.ms/x/c/6ee679fb17cb7e45/Ec6QJY1xaXROukclj-VaoW0BZYjMhANzvhl4OFukD41uRQ?e=fcMjPw



