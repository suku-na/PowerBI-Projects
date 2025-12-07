<h1 align="center">🔍 Karnataka Crime Analysis Power BI Dashboard</h1>

---

## 🧰 Tech Stack
<p align="center">
  <!-- PowerBI -->
  <img src="https://upload.wikimedia.org/wikipedia/commons/c/cf/New_Power_BI_Logo.svg" width="45" height="45" alt="Power BI"/> 
  <!-- Excel -->
  <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/microsoftexcel.svg" width="45" height="45" alt="Excel" style="filter: invert(52%) sepia(96%) saturate(322%) hue-rotate(83deg) brightness(90%) contrast(85%);"/>
  <!-- GitHub -->
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="50" alt="GitHub"/>
  <!-- Windows -->
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/windows8/windows8-original.svg" width="50" alt="Windows"/>
</p>

---
---
<p align="center">
  <i>End-to-end crime analytics and reporting for the state of Karnataka</i>
</p>

<p align="center">
  <img width="1057" height="711" alt="image" src="https://github.com/user-attachments/assets/4e146aac-1bbd-4087-9e42-f41d46bd85cb" />
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
```

## 🚀 How to Use
1. Download the file Karnataka Crime Dashboard.pbix
2. Open in Power BI Desktop
3. Recommended: Latest version of Power BI Desktop
4. Connect / Refresh Data (if applicable)
5. Update the data source path if you’re using local Excel/CSV files
6. Click on Refresh to load the latest data
7. Interact with the visuals
8. Use slicers (Year, District, Crime Type, Status, etc.)
9. Hover over charts for detailed tooltips

---

---

## 📂 Repository Structure

```
📁 Karnatka crime analytics
│
├── Karnataka Crime Analytics (2023-2025).pbix
├── README.md
└── 📁 images
```
---

## 🔗 References
- Microsoft Power BI — [https://learn.microsoft.com/power-bi](https://learn.microsoft.com/power-bi)  
- Power Query M Language — [https://learn.microsoft.com/powerquery-m](https://learn.microsoft.com/powerquery-m)

---

## ✨ Author
**Sumit Kumar**  
📎 [GitHub Profile](https://github.com/suku-na)  
📂 [Project Repository](https://github.com/suku-na/PowerBI-Projects)

---
