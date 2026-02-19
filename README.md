# Project-Cost-Saving-Dashboard-Semicon-Company-XYZ

## 📌 Project Overview

As an Advanced Manufacturing Engineer and Data Analytics enthusiast, I developed this dynamic Excel dashboard to monitor, track, and forecast cost-saving initiatives for 50+ active projects.

The primary goal is to provide a centralized "Source of Truth" for management to visualize financial impacts across three core pillars: **Material**, **Yield (Defect Reduction)**, and **Labor**.

## ⚙️ The Ecosystem: Integration with Finance & IE
This dashboard does not exist in a vacuum. It is powered by a collaborative data pipeline:
* **Product Cost Estimation (PCE):** I designed a separate [Product-Cost-Estimation-Simulator](LINK_TO_YOUR_OTHER_REPO) to calculate cost saving improvement estimates.
* **Collaborative Inputs:** Developed in partnership with **Finance** (for standard costing) and **Industrial Engineering** (for validated labor hour data).

## 🚀 Key Features
* **Main Dynamic Dashboard:** Real-time filtering by Project Category and Value Creation (VC) type. It provides an immediate breakdown of savings by Material, Yield, and Labor.
* **Quarterly Savings Summary:** A dedicated sheet for executive reporting, showcasing fiscal performance and quarterly trends (Q1–Q4).
* **Volume Integration:** Incorporates actual (latest) and forecasted production volumes in a year to ensure savings are grounded in real-world output. It is update every month

## 🏗️ Data Architecture & Workflow
The tool is built with a structured data-modeling approach to ensure scalability for 50+ projects:

1.  **Proj_Reg:** The registry for all project-specific metadata.
2.  **Rec_Vol & Vam_Vol:** Monthly volume tracking sheets for actuals and forecasts.
3.  **Data_Model (The Core):** This is the analytics engine. It maps project numbers to part numbers and calculates savings ($) by multiplying volume by the PCE unit-saving (Material/Labor/Yield). 
    * *Note: Overhead costs are tracked but currently zeroed out per management directive.*
4.  **Data_Trans:** An intermediary transformation sheet that summarizes `Data_Model` tables into pivot-ready formats for the visual graphs.

## 📊 Visualizations
* **Cost Saving Per Category:** Stacked bar charts showing the contribution of Material vs. Yield vs. Labor.
* **Project Ranking:** Vertical bar charts identifying the highest-impact projects
* **Forecast vs. Target:** High-level cards tracking Annual Operating Plan (AOP) vs. Actual Calendar Savings.

## 🛠️ Tech Stack
* **Microsoft Excel:** Advanced Data Modeling, Table Referencing, and Dashboard Design.
* **Business Logic:** Manufacturing Finance, Labor Productivity Analysis, and Volume-Weighted Forecasting.

---
*Developed by [Marlon / https://github.com/Marlon-001] – Advanced Manufacturing Engineer*
