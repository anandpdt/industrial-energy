# Industrial Energy Consumption Analysis — Power BI

<p align="center">
  <h1 align="center">Industrial Energy Consumption Analysis</h1>
  <p align="center">
    U.S. Industrial Combustion Energy Analysis — 2014
  </p>
</p>

---

## 📊 Project Overview

This project presents an interactive **Power BI dashboard for analyzing U.S. industrial combustion energy consumption in 2014**.

The analysis explores energy consumption across:

- Fuel types
- Industrial sectors
- States
- Facilities
- Combustion unit types
- Geographic regions
- Facility-level operations

The project transforms raw industrial energy data into an interactive Business Intelligence solution using **Power Query, DAX, and Power BI**.

### Analytics Workflow

**Raw Dataset → Data Cleaning → Data Transformation → DAX Measures → Dashboard Development → Energy Insights**

---

# 🎯 Project Objectives

The main objectives of this project are to:

- Analyze total industrial energy consumption.
- Compare energy consumption across different fuel types.
- Identify the industries with the highest energy demand.
- Compare industrial energy consumption across U.S. states.
- Analyze regional energy distribution.
- Identify the largest energy-consuming facilities.
- Analyze energy consumption by combustion unit type.
- Examine the relationship between facility size, number of units, and energy consumption.
- Provide an interactive dashboard for exploring industrial energy patterns.

---

# 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| **Microsoft Power BI** | Dashboard development and visualization |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Measures, KPIs and calculations |
| **CSV** | Source dataset |
| **GitHub** | Project documentation and version control |

---

# 📁 Dataset

The project uses a **2014 U.S. industrial combustion energy dataset**.

The dataset contains information related to industrial facilities, energy consumption, fuel types, industries, states, and combustion units.

### Important fields used in the analysis

- `FACILITY_ID`
- `FACILITY_NAME`
- `STATE`
- `GROUPING`
- `UNIT_TYPE`
- `UNIT_NAME`
- `FUEL_TYPE`
- `MMBtu_TOTAL`
- `GWht_TOTAL`

### Energy Measures

Two primary energy measures were used:

- **MMBtu_TOTAL** — Total energy consumption in million British thermal units.
- **GWht_TOTAL** — Total energy consumption in gigawatt-hours thermal.

---

# 🧹 Data Cleaning & Transformation

The raw dataset was prepared using **Power Query** before building the dashboard.

The cleaning process included:

- Removing unnecessary columns.
- Removing index/unusable fields.
- Handling columns containing large amounts of missing information.
- Correcting data types.
- Cleaning categorical fields.
- Preparing geographic information.
- Preparing fuel-type information.
- Preparing industrial grouping information.
- Preparing facility and combustion-unit information.
- Retaining the main energy consumption measures.

The cleaned data was then used to create the Power BI data model and dashboard calculations.

---

# 📐 DAX Measures

Several DAX measures were created to calculate the major KPIs used throughout the dashboard.

### Total Energy (MMBtu)

```DAX
Total Energy (MMBtu) =
SUM('Industrial Energy'[MMBtu_TOTAL])
