# NYC 311 Service Requests — API Data Cleaning & Analysis

This project demonstrates **professional API data extraction, JSON flattening, data cleaning, and analytics** using **Python (Requests, Pandas, NumPy, Matplotlib, Seaborn)**.  
It’s designed as a portfolio example to showcase my **API handling, data wrangling, visualization, and reporting** skills for **freelance projects**.

---

## Overview

The dataset was collected directly from the **NYC 311 Service Requests API (Socrata Open Data API)**.  
The raw API response consisted of **nested JSON**, inconsistent formatting, missing values, and duplicated records.

This project shows how I:

- Pulled **5,000+ live records** from a public API  
- Converted unstructured JSON into a clean DataFrame  
- Cleaned and standardized column names and formats  
- Parsed multiple date fields correctly  
- Produced exploratory summaries  
- Built visualizations  
- Exported all results into a **multi-sheet Excel report**

This mimics a **real-world client workflow**, where raw API data must be turned into clean, analyzable, and visual formats.

---

## Key Steps

1. **API Extraction**
   - Used `requests` to fetch recent records.
   - Converted nested JSON using `pandas.json_normalize()`.

2. **Data Cleaning**
   - Removed duplicate rows and duplicate columns.
   - Standardized 60+ column names (title case, removed symbols).
   - Converted date columns (`Created Date`, `Closed Date`, etc.) to usable datetimes.
   - Removed invalid rows lacking both `Unique Key` and `Created Date`.
   - Filled missing values consistently across the dataset.

3. **Exploratory Analysis**
   - Identified the **Top 20 complaint types**.
   - Summarized case distribution across **NYC boroughs**.

4. **Visualization**
   - Bar charts for:
     - Top complaint types  
     - Borough-level counts  

5. **Excel Integration**
   - Saved cleaned data to a new Excel file.
   - Added a separate sheet for analysis summaries.
   - Stored all generated plots inside `/outputs`.

---

## Project Structure
- NYC 311 API — Data Cleaning & Reporting 
  - 311_API_cleaning.ipynb (Jupyter notebook with code & analysis)
  - outputs (Folder containing a multi-sheet Excel report and plots)
    - cleaned_311_data.xlsx (cleaned data)
    - borough_counts.png
    - top_complaints.png
  - README.md (Project documentation)

---

## Insights

- API data had multiple inconsistencies: missing values, invalid dates, and structural variations.  
- After cleaning:
  - All date fields became usable for time-based analysis.
  - Complaint types were standardized and categorized.
  - Borough-level patterns became clear and interpretable.
- The cleaned dataset is ready for **dashboards, reporting, or further modeling**.

---

## Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Python** | Full data pipeline |
| **Requests** | API extraction |
| **Pandas** | Data cleaning, JSON flattening, exporting |
| **NumPy** | Numerical operations |
| **Matplotlib / Seaborn** | Data visualization |
| **OpenPyXL** | Excel automation |
| **Jupyter Notebook** | Development environment |

---

## Outputs

| File | Description |
|------|-------------|
| `cleaned_311_data.xlsx` | Cleaned and standardized dataset in Excel |
| `top_complaints.png` | Top 20 complaint type visualization |
| `borough_counts.png` | Borough-level case summary |

---

## Skills Demonstrated

✅ API Data Extraction (SODA API)  
✅ JSON → DataFrame Normalization  
✅ Data Cleaning & Standardization  
✅ Date Parsing & Handling Missing Data  
✅ Exploratory Data Analysis  
✅ Visual Reporting (client-ready)  
✅ Excel Automation (multi-sheet output)  
✅ Reproducible Jupyter Notebook Workflow  


