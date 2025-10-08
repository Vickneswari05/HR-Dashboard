# HR Dashboard — Power BI

## Overview
An interactive **HR Dashboard** built in **Power BI** to track employee attendance, work-from-home (WFH) trends, and sick leave (SL). The dashboard helps HR teams monitor workforce engagement and quickly identify attendance patterns across dates and weekdays.

## Key Features
- KPI tiles: Total working days, Present days, Present %, WFH %, SL count, SL %.  
- Employee-level table: Present %, WFH %, SL % per employee.  
- Trend charts: Present % by date, WFH % by date, SL % by date.  
- Day-of-week summary tables for Present %, WFH %, and SL %.  
- Month slicer to filter April / May / June 2022 (or other months if data updated).  
- Responsive visuals and drill-through support (if enabled in PBIX).

## Demo / Preview
![HR Dashboard Preview](images/dashboard_preview.png)


## Data & Measures
- Source: Attendance dataset (CSV/Excel) containing employee, date, attendance type (Present/SL/WFH/etc.), and other metadata.  
- Important DAX measures (examples):
  - `Present % = DIVIDE([Present Days], [Total Working Days], 0)`  
  - `WFH % = DIVIDE([WFH Days], [Total Working Days], 0)`  
  - `SL % = DIVIDE([SL Days], [Total Working Days], 0)`


