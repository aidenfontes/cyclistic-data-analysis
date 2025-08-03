# 🚴 **Divvy Bike Share Analysis (2021)**  
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)  
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)  
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)  

### **Exploratory Data Analysis of Divvy bike share trips (Jan–Dec 2021) to understand how annual members and casual riders use the service differently.**  
*Following the Google Data Analytics 6-step process.*  

---

## **📑 Table of Contents**  
1. [Project Overview](#-project-overview)  
2. [Business Task](#-business-task)  
3. [Dataset](#-dataset)  
4. [Process](#-process)  
5. [Key Insights & Actions](#-key-insights--actions)  
6. [Visualizations](#-visualizations)  
7. [Tools Used](#-tools-used)  
8. [How to Use](#-how-to-use-this-project)  
9. [Future Work](#-future-work)  
10. [Author](#-author)  

---

## **📌 Project Overview**  
This project analyzes **2021 Divvy bike share trip data** to uncover **how annual members and casual riders use the service differently**.  
The goal: **Provide actionable recommendations** to increase memberships and optimize bike allocation.  

**Framework used:** Google Data Analytics 6-step process  
> **Ask → Prepare → Process → Analyze → Share → Act**

---

## **🎯 Business Task**  
**Key Question:**  
> *How do annual members and casual riders use Divvy bikes differently?*  

**Objective:**  
- Identify **behavioral differences** between user groups.  
- Develop **data-driven recommendations** to:  
  - Increase casual-to-member conversions.  
  - Improve bike availability across stations and times.  

**Stakeholders:**  
- Divvy Marketing Team.  
- Divvy Operations Team.  

---

## **📂 Dataset**  
- **Source:** [Divvy System Data](https://divvybikes.com/system-data) (Jan–Dec 2021).  
- **Files:** 12 monthly CSVs combined into one dataset (~5.5M rows).  
- **Key columns:**  
  - `ride_id` – Unique trip identifier.  
  - `rideable_type` – Type of bike (classic, docked, e-bike).  
  - `started_at`, `ended_at` – Trip timestamps.  
  - `start_station_name`, `end_station_name`.  
  - `member_casual` – User type: *member* or *casual*.  

---

## **🛠 Process**  
### 1. **Data Cleaning & Preparation:**  
- Combined 12 monthly datasets into a single DataFrame.  
- Converted timestamps to datetime.  
- Removed missing & invalid entries (null stations, negative/zero durations).  
- Created new features:  
  - **Ride duration (minutes)**.  
  - **Day of week**, **month**, **hour of day**.  

### 2. **Exploratory Analysis:**  
- Ride counts by **user type**, **day**, **month**, **hour**, and **bike type**.  
- **Top stations** for members vs casual riders.  
- **Seasonality** trends across the year.  

### 3. **Visualization:**  
- Created bar charts, line plots, and heatmaps using **Seaborn** & **Matplotlib**.  

---

## **🔑 Key Insights & Actions**  

### 1. **Members ride mostly on weekdays during commute hours.**  
> **Action:** Launch **weekday commuter loyalty programs** & ensure **bike availability at business districts during 7–9 AM & 5–7 PM**.  

### 2. **Casual riders peak on weekends and take longer rides.**  
> **Action:** Create **weekend/day pass packages** & offer **discounts for long-duration rides** to target leisure users and tourists.  

### 3. **Casual riders favor e-bikes; members prefer classic bikes.**  
> **Action:** **Redistribute e-bikes** to tourist stations & **stock classic bikes** near workplaces.  

### 4. **Seasonal spikes in summer usage (June–Sept).**  
> **Action:** **Increase fleet size & maintenance capacity** in peak months. Offer **winter promotions** to encourage off-season ridership.  

### 5. **Top stations differ significantly between members & casuals.**  
> **Action:** **Prioritize rebalancing & maintenance** at busiest stations. Deploy **QR-code marketing campaigns** at tourist-heavy stations.  

---

## **📊 Visualizations**  
- Rides by Day of Week & User Type (Bar chart)  
- Average Ride Duration by Day of Week & User Type  
- Ride Count by Hour of Day & User Type (Line chart)  
- Rides by Bike Type (Bar chart)  
- **Monthly Ride Trends** (Bar chart)  
- **Top 10 Stations by User Type** (Horizontal bar chart)  
- **Heatmaps**: Ridership by Day & Hour for members vs casuals  

*(See full notebook for all charts.)*  

---

## **🧰 Tools Used**  
- **Python:** Pandas, Seaborn, Matplotlib  
- **Environment:** Jupyter Notebook  

---

## **🚀 How to Use This Project**  
1. Clone this repository.  
2. Download Divvy trip data for 2021 from [Divvy System Data](https://divvybikes.com/system-data).  
3. Update the file paths in the notebook to match your data location.  
4. Run the Jupyter Notebook to reproduce the analysis & visualizations.  

---

## **🔮 Future Work**  
- Build a **predictive model** (e.g., logistic regression or random forest) to classify rides as member vs casual.  
- Develop an **interactive Tableau or Power BI dashboard** for stakeholder reporting.  
- Perform **clustering analysis** to segment casual riders (e.g., tourists vs occasional weekend users).  

---

## **👤 Author**  
**Aiden Fontes**  
*Data Analyst | Python | SQL | Tableau*  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue.svg)](https://www.linkedin.com/)  
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black.svg)](https://github.com/)  
