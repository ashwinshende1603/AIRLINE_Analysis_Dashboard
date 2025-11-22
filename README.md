# Airline Operational and Performance Analysis

## 1. Project Overview

This Power BI project provides a comprehensive analysis of flight operations, punctuality, and fleet performance using flight data from 2023 to 2025. The core goal is to enable stakeholders to quickly identify bottlenecks, benchmark carrier performance, and understand seasonal trends impacting flight delays and cancellations.

The project is structured into four distinct dashboards, offering views ranging from executive summary to deep-dive operational analysis.

## 2. Data Source & Scope

* **Dataset:** `flight_dataset_2023_2025.xlsx`
* **Scope:** Analyzes flight data across various domestic and international routes, covering key metrics such as volume, status, and delay duration over a three-year period.

## 3. Key Dashboards

The analysis is segmented across four interactive dashboards for focused insights:

| Dashboard Title | Goal | Key Visuals |
| :--- | :--- | :--- |
| **Operational Overview** | High-level summary of performance and primary KPIs for executive review. | Flight Volume, OTP %, Total Cancellations, Average Flight Delay Time, Monthly Flight Volume. |
| **Delay & Punctuality Analysis** | Deep dive into the time, origin, and magnitude of flight delays. | Avg. Delay by Origin Airport, Total Monthly Delay Impact, Delay Magnitude Distribution. |
| **Carrier Performance Benchmarking** | Comparative analysis of the operational reliability and market share across competing airlines. | Market Share by Carrier, Flight Status Breakdown by Carrier, Carrier Volume & Delay Benchmarking. |
| **Route & Network Analysis** | Focus on geographic traffic flow, route-specific performance, and fleet utilization. | Route Traffic Volume, Fleet Utilization by Aircraft, Fleet Performance by Origin (OTP %). |

## 4. Core Metrics & Key Insights

The dashboard uses professionally defined metrics to ensure clarity and industry relevance:

### **Primary Key Performance Indicators (KPIs)**

* **On-Time Performance (OTP) %:** The percentage of flights arriving on schedule.
* **Average Flight Delay Time:** Mean duration of delays across all flights.
* **Total Cancellations:** Raw count of flights that were cancelled.
* **Flight Volume:** Total number of flights operated.

### **Initial Key Insights (Derived from Sample Data)**

Based on the initial data analysis, the following observations were identified:

1.  **Delay Magnitude is Highly Skewed:** A significant majority of delayed flights (**~67%**) fall into the "Greater than 60 Minutes" bucket, suggesting that when delays occur, they tend to be severe and high-impact.
2.  **Top Delay Airports:** Airports such as **DXB, FRA, DOH, and DEL** were flagged as having the highest average delay times, indicating potential operational bottlenecks at these key hubs (Visual: `Avg. Delay by Origin Airport`).
3.  **Major Carrier Impact:** When measured by total accumulated delay minutes, **United Airlines, Emirates, and IndiGo** were the highest contributors to system-wide delay impact. *(Further analysis is required to separate volume effect from poor performance.)*

## 5. Technical Requirements

* **Software:** Power BI Desktop (Developed using the provided `.pbit` template file: `AIRLINE_Analysis_ Project.pbit`).
* **Data Model:** Includes necessary relationships and calculated columns (e.g., `Delay Bucket` for histogram replacement) to support the analysis.
