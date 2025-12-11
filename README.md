# 🌍 Global Earthquake Analysis Dashboard (2015–2025)

An interactive **Power BI dashboard** built using **80,000+ global earthquake records** from the **USGS Earthquake Catalog**.  
This project analyzes seismic activity over a decade, uncovering trends in **magnitude**, **depth**, **yearly patterns**, and **geographical impact**.

---

## 📊 Project Overview

This dashboard provides a deep-dive into global earthquake behavior using various analytical visuals.  
The goal is to deliver clear insights into:

- Year-wise earthquake frequency  
- Magnitude category distribution (Low, Medium, High)  
- Depth vs Magnitude relationship  
- Country-level impact  
- Magnitude distribution patterns  
- Categorization of shallow, intermediate, and deep earthquakes  

The project also includes a cinematic **Welcome Page UI** designed for a smooth user experience.

---

## 📁 Dataset Information

**Source:** USGS Earthquake Catalog  
**Records:** ~80,000 earthquakes  
**Time Period:** 2015–2025  
**Columns Used:**  
- Time  
- Latitude  
- Longitude  
- Depth  
- Magnitude  
- Place  
- Country  
- Year  
- Month  
- Magnitude Category (DAX-created)  
- Depth Category (DAX-created)

Custom DAX Columns:
DAX
MagCategory =
IF([Magnitude] < 5, "Low",
IF([Magnitude] < 7, "Medium", "High"))
DAX
Copy code
DepthCategory =
IF([Depth] < 70, "Shallow",
IF([Depth] < 300, "Intermediate", "Deep"))


---

## 🛠️ Tools & Technologies
  Power BI Desktop
  
  DAX (Data Analysis Expressions)
  
  Data Modeling
  
  Data Cleaning & Transformation
  
  Visualization Design
  
  USGS Earthquake Dataset


---

## 🚀 Features of the Dashboard
1. Welcome Page
  A cinematic landing screen with a clickable navigation button to the main dashboard.

2. Key Performance Indicators (KPIs)
  Total Earthquakes
  
  Average Magnitude
  
  Maximum Magnitude
  
  Average Depth

✔ 3. Visualizations Included
  Earthquakes by Magnitude Category (Bar Chart)
  
  Earthquakes by Year (Line Chart)
  
  Earthquakes by Country (Custom Bar Chart)
  
  Depth vs Magnitude Relationship (Scatter Plot)
  
  Magnitude Distribution (%) (Pie Chart)
  
  Distribution of Earthquake Magnitudes (Histogram-Style Visual)
  
  Data Table with detailed event records

✔ 4. Filtering
  Year slicer allows viewing data selectively.


---

## 🔍 Insights Gained
  Most earthquakes recorded in this dataset fall under the Low magnitude category.
  
  Shallow earthquakes are the most frequent globally.
  
  The scatter plot shows no strict relationship but highlights clustering around shallow depths.
  
  Countries like Indonesia, Japan, Chile, and Alaska region have the highest number of events.
  
  Yearly patterns show fluctuations but overall consistent seismic activity.
