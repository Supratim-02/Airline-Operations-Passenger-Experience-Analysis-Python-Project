# Airline Operations & Passenger Experience Analysis

## 📘 Project Overview
This project presents an **end-to-end analysis of airline operations and passenger experience** using Python.  
The analysis focuses on understanding **flight punctuality, regional and seasonal performance, passenger demographics, and operational risk** to identify inefficiencies and improvement opportunities.

By combining operational data with passenger attributes, this project demonstrates how **data-driven insights** can support better planning, reduce disruptions, and enhance overall passenger experience.

---

## 🎯 Project Objectives
The key objectives of this project are to:

1. Analyze the overall distribution of flight statuses (On Time, Delayed, Cancelled)
2. Examine how flight delays vary across continents and regions
3. Identify seasonal patterns in flight delays using monthly trend analysis
4. Study how flight disruptions affect different passenger age groups
5. Detect high-risk countries, airports, and routes
6. Quantify operational risk using composite risk indicators
7. Build a clear and informative dashboard summarizing key operational metrics
8. Derive actionable insights for data-driven airline operations management

---

## 🧩 Business Problem
Airline operations are highly sensitive to **delays and cancellations**, which directly impact:

- Passenger satisfaction
- Operational costs
- Brand reputation
- Resource utilization

Despite large volumes of available data, airlines often struggle to identify:
- Where disruptions occur most frequently
- When delays are most likely to happen
- Which passenger groups are most affected

This project addresses these challenges by transforming raw operational data into **actionable intelligence**.

---

## 🗂️ Dataset Description
The dataset represents **airline operational records combined with passenger information**.

- Each row corresponds to a **single flight–passenger interaction**
- Includes operational, geographic, temporal, and demographic attributes
- Contains both categorical and numerical variables

---

## 📊 Table Structure (Data Dictionary)

| Column Name | Data Type | Description | Analytical Relevance |
|------------|----------|-------------|----------------------|
| `Age` | Numeric | Age of the passenger | Used to create age groups |
| `Gender` | Categorical | Passenger gender | Gender-based impact analysis |
| `Nationality` | Categorical | Passenger nationality | Demographic segmentation |
| `Airport Name` | Categorical | Departure airport | Airport-level performance |
| `Arrival Airport` | Categorical | Arrival airport | Route-level risk analysis |
| `Country Name` | Categorical | Country of departure | Country-level disruption risk |
| `Airport Continent` | Categorical | Continent of airport | Infrastructure-based insights |
| `Continents` | Categorical | Passenger continent | Regional performance analysis |
| `Pilot Name` | Categorical | Assigned pilot | Operational reference |
| `Flight Status` | Categorical | On-time / Delayed / Cancelled | Core operational outcome |
| `Departure Date` | Date | Flight departure date | Seasonality analysis |

---

## 🧹 Data Cleaning & Standardization
To ensure consistency and analytical reliability:

- Missing categorical values replaced with `"unknown"`
- Text columns standardized (lowercase and trimmed)
- Dates converted to datetime format
- Duplicate records removed

This step ensures **data quality, consistency, and reproducibility**.

---

## 🧠 Feature Engineering

### 🔹 Age Groups
Passengers were segmented into meaningful age categories:

| Age Range | Group |
|---------|-------|
| 0–18 | Teen |
| 19–30 | Young Adult |
| 31–45 | Adult |
| 46–60 | Senior |
| 60+ | Elderly |

Used to analyze **passenger vulnerability to disruptions**.

---

### 🔹 Delay & Cancellation Flags
Binary indicators created:
- `delay_flag` → delayed flights
- `cancel_flag` → cancelled flights

Used for **risk modeling and aggregation**.

---

## 📈 Analytical Components

### 🔹 Flight Status Distribution
- Overall breakdown of on-time, delayed, and cancelled flights
- Measures general airline punctuality

---

### 🔹 Continental Performance Analysis
- Percentage distribution of flight statuses across continents
- Highlights regional infrastructure and operational differences

---

### 🔹 Country & Airport Risk Analysis
- Countries and airports ranked by delay and cancellation rates
- Identifies **high-risk operational zones**

---

### 🔹 Passenger Demographic Impact
- Flight outcomes compared across age groups and gender
- Reveals which passenger segments are most affected

---

### 🔹 Seasonality Analysis
- Monthly delay trends derived from departure dates
- Identifies **seasonal peaks and operational stress periods**

---

### 🔹 Route-Level Risk Analysis
- Delay and cancellation risk across airport-to-airport routes
- Supports network-level optimization

---

### 🔹 Extreme Risk Zone Detection
- Airports flagged where delays or cancellations frequently occur
- Used to identify chronic disruption hotspots

---

### 🔹 Composite Airline Risk Index
A custom **Composite Risk Index** was created using:


**Purpose**
- Quantify overall operational risk
- Compare risk levels across continents
- Support proactive planning

---

## 📊 Dashboard & Visual Analytics
A consolidated dashboard was developed to visualize:

- Flight status distribution
- Delay percentage by continent
- Monthly delay trends
- Age group vs flight status impact

Designed for **management-level decision support**.

---

## 🔍 Key Insights
1. A significant proportion of flights experience delays
2. Delay rates vary widely across continents
3. Seasonal peaks reveal predictable disruption periods
4. Certain airports and routes consistently show higher risk
5. Senior and elderly passengers are more affected by disruptions
6. Operational performance, seasonality, and passenger impact are strongly interconnected

---

## ✅ Business Recommendations
- Prioritize operational improvements in high-delay regions
- Increase staffing and buffers during peak-delay months
- Enhance communication and support for vulnerable passenger groups
- Monitor dashboards regularly for early warning signals
- Use historical trends for proactive operational planning
- Extend future analysis with delay duration and root-cause data

---

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

---

## 📁 Suggested Project Structure

---

## 👤 Author
**Supratim Maity**   

---

⭐ If you find this project insightful, consider starring the repository.
