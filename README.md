# Reducing costs per delivery for a logistics company's Metro Manila operations
## Objective
Lower **cost per successful delivery** for Metro Manila delivery van operations by identifying key cost drivers across hubs and routes.

## Scope
Focused on **Metro Manila hubs** (Mm-East, Mm-West, Mm-North, Mm-South) to keep operating conditions comparable (delivery density + traffic patterns).

## Files
- Raw data: `data/raw/delivery_van_ops_raw.xlsx`
- Clean KPI table: `data/processed/kpi_table_powerbi_filled_plausible_final.csv`
- Cleaning notebook: `notebooks/datacleanup.ipynb`
- Power BI dashboard: `powerbi/portfolio.pbix`

## Core KPIs (4)
1. **KPI 1: Cost per Successful Delivery (PHP)** = Total Cost / Successful Deliveries  
2. **KPI 2: First-Attempt Success Rate (%)** = Parcels Delivered / Delivery Attempts  
3. **KPI 3: On-Time Delivery Rate (%)** = On-time Deliveries / Parcels Delivered  
4. **KPI 4: Fuel Efficiency vs Standard (ratio)** = Actual km/L / Typical km/L

## Data Cleaning Summary
- Standardized mixed date formats for weekly reporting.
- Normalized hub/route labels.
- Addressed “impossible zeros” (activity present but fields recorded as 0) using rule-based fills from typical hub/route behavior; adjusted rows were flagged for transparency.
- Reduced scope from nationwide to Metro Manila region only

## Dashboard Pages
- **Page 1 — Executive Summary**
- **Page 2 — Diagnostics**
- **Page 3 — Fuel & Efficiency**
- **Page 4 — Drilldown Heatmap**

## Screenshots
![Page 1](Screenshots/page1_executive.png)  
![Page 2](Screenshots/page2_diagnostics.png)  
![Page 3](Screenshots/page3_fuel_productivity.png)  
![Page 4](Screenshots/page4_drilldown.png)  

## Reproduce
1. Run the notebook in `notebooks/`
2. Open `powerbi/portfolio.pbix`
3. If needed, repoint the data source to `data/processed/kpi_table_powerbi_filled_plausible_final.csv` and refresh.
