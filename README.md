# FUTURE_DS_03
FUTURE_DS_03
🚦 Road Accident Dashboard
📊 This project contains a Power BI dashboard that analyzes road accident data, along with SQL queries for data cleaning, processing, and insights. The dataset consists of 307,973 rows of road accident records.

🛠 Tools Used
Excel & SQL for data preprocessing
Power BI for dashboard creation
GitHub for project management
🔍 SQL Queries Implemented
Below are the key SQL queries used in this analysis:

✅ Data Cleaning
UPDATE Road_Accidents  
SET Junction_Control = 'Unknown'  
WHERE Junction_Control = 'Data missing or out of range';  
📊 Severity Analysis
SELECT Severity, COUNT(*) AS Accident_Count  
FROM Road_Accidents  
GROUP BY Severity  
ORDER BY FIELD(Severity, 'Fatal', 'Serious', 'Slight');  
🌍 Identifying High-Risk Zones
SELECT Latitude, Longitude, Region, COUNT(*) AS Accident_Count  
FROM Road_Accidents  
GROUP BY Latitude, Longitude, Region  
ORDER BY Accident_Count DESC  
LIMIT 10;  
📂 GitHub Repository & File Links:

Road Accident Dashboard: Road Accident Dashboard.pbit
SQL Queries: road_accident_analysis.sql
🔗 GitHub Clone Link:

git clone https://github.com/Gyanankur23/FUTURE_DS_03.git
🚀 Dive into the data and explore insights! Let me know if you need any refinements. 💡
