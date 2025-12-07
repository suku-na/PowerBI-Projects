<h1 align="center">🔍 Karnataka Crime Analysis Power BI Dashboard</h1>

<p align="center">
  <i>End-to-end crime analytics and reporting for the state of Karnataka</i>
</p>

<p align="center">
  <img src="./Karnataka_Crime_Dashboard.png" alt="Karnataka Crime Dashboard" width="800"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Tool-Power%20BI-F2C811?logo=power%20bi&logoColor=black" />
  <img src="https://img.shields.io/badge/Focus-Crime%20Analytics-blue" />
  <img src="https://img.shields.io/badge/Domain-Public%20Safety-red" />
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen" />
</p>

---

## 📌 Project Overview

The **Karnataka Crime Dashboard** is an interactive Power BI report that helps analyze crime patterns across districts in Karnataka.  

It enables stakeholders (police departments, policy makers, and analysts) to:

- Track **overall crime trends** over time  
- Compare **crime intensity across districts & regions**  
- Analyze **crime types** (e.g., theft, assault, cyber crime, etc.)  
- Identify **high-risk zones & peak periods**  
- Support **data-driven policing & resource allocation**

---

## 🎯 Objectives

- Provide a **single, interactive view** of crime data for Karnataka  
- Identify **hotspots** where crime incidents are concentrated  
- Understand **which types of crimes are increasing or decreasing**  
- Support **faster decision-making** using visual insights instead of raw tables  

---

## 🗂️ Dataset Description

> _Note: Adjust these points as per your actual dataset columns._

Typical fields used in this dashboard include:

- **Location details**  
  - State, District, Police Station / City  
- **Crime details**  
  - Crime Category (e.g., Theft, Assault, Cyber Crime, Fraud, etc.)  
  - Sub-category / IPC Sections (if available)  
- **Time dimensions**  
  - Year, Month, Quarter  
  - Date of Incident / FIR Date  
- **Case details**  
  - Case Status (Open / Closed / Pending)  
  - Number of Cases / FIR Count  

---

## 📊 Dashboard Pages & Features

> _Customize to exactly match your report pages._

1. ### 🔹 Overview Page
   - Total Crime Cases
   - Year-on-Year trend of reported crimes  
   - Top 5 high-crime districts  
   - KPI cards for:
     - Total Cases  
     - Closed Cases  
     - Pending / Under Investigation  

2. ### 🔹 Crime by District
   - Map / bar charts showing crime distribution across districts  
   - Filters for:
     - Year  
     - Crime Category  
   - District comparison visuals

3. ### 🔹 Crime Type Analysis
   - Breakdown of cases by **crime category & sub-category**  
   - Trend lines to see which crime types are **rising or falling**  
   - Stacked bar / column charts to compare categories across years

4. ### 🔹 Time Analysis
   - Crimes by:
     - Year, Quarter, Month  
   - Seasonal patterns in crime  
   - Helps identify **spikes in particular periods**

5. ### 🔹 Case Status & Closure
   - Cases by **status** (Open, Closed, Pending)  
   - Closure rate % over time  
   - District-wise performance on case closure

---

## 🧮 Key Measures (DAX – Conceptual)

Some example measures that can be used in this report:

```DAX
Total Cases = COUNTROWS(CrimeData)

Closed Cases = 
CALCULATE(
    [Total Cases],
    CrimeData[Case Status] = "Closed"
)

Open Cases =
CALCULATE(
    [Total Cases],
    CrimeData[Case Status] = "Open"
)

Closure Rate % =
DIVIDE([Closed Cases], [Total Cases])

