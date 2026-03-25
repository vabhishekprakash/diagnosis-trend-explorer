# Diagnosis Trend Explorer — Insights into Treatment Demand

An interactive **Power BI** dashboard that analyses diagnosis patterns and treatment demand across hospitals in Telangana and Andhra Pradesh. The report surfaces trends in disease categories, patient load, departmental throughput, and treatment costs to support data-driven decisions in healthcare operations.

---

## Dashboard Preview

![Data Model](data/DataModel_Poster.svg)

---

## Features

- **Diagnosis Trend Analysis** — track diagnosis frequency by category, severity, and ICD code over time
- **Treatment Demand Overview** — monitor inpatient vs outpatient volumes, length of stay, and readmission rates
- **Hospital & Department Drill-Down** — compare performance across 8 hospitals and multiple specialisations
- **Cost Breakdown** — analyse treatment, medication, and procedure costs by diagnosis and ward type
- **Doctor Performance** — view caseload distribution by specialisation and experience

---

## Data Model

| Table | Description |
|---|---|
| `Fact_Treatments` | Core fact table — 687 treatment records with costs, dates, and outcomes |
| `Dim_Diagnoses` | 20 diagnoses with ICD codes, categories, severity, and department mapping |
| `Dim_Patients` | 542 patient records with demographics |
| `Dim_Doctors` | Doctor details including specialisation, qualification, and consultation fees |
| `Dim_Hospitals` | 8 hospitals across Telangana and Andhra Pradesh with bed and accreditation info |

---

## Getting Started

**Requirements:** Power BI Desktop (free download at [powerbi.microsoft.com](https://powerbi.microsoft.com))

1. Clone or download this repository
2. Open `Ignite2 - 07 - Diagnosis Trend Explorer - Insights into Treatment Demand.pbix` in Power BI Desktop
3. The report loads with pre-embedded data — no additional setup required

> If prompted to refresh data sources, point them to the CSV files in the `/data` folder.

---

## Tech Stack

- **Power BI Desktop** — report authoring and data modelling
- **DAX** — custom measures and KPIs
- **CSV** — flat-file data sources (star schema)
