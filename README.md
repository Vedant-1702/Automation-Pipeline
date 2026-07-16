# Automated-Data-Pipeline-Analytics-Dashboard

> A complete end-to-end **Global Economic Intelligence & Investment Analytics Platform** that automates data ingestion, transformation, risk modeling, and dashboard-driven investment decision support.

---

##  Overview  
This project covers the **full data analytics & automation lifecycle**:

- **Data Engineering** – automated file ingestion, format standardization, ETL pipeline  
- **Cloud Automation** – Google Drive + Google Apps Script hourly triggers  
- **Data Transformation** – Power Query cleaning, unpivoting, modeling  
- **Investment Risk Modeling** – Misery Index, Sweet Spot Score, Fiscal Risk scoring  
- **Dashboarding** – dynamic Excel dashboard for global investment insights  

---

##  Dataset  

- Source: International Monetary Fund – World Economic Outlook Database  
- Coverage: 196 Countries  
- Records: 40,000+ rows  
- Indicators:
  - Inflation (Average Consumer Prices)
  - GDP Growth (Constant Prices)
  - Unemployment Rate
  - Gross National Savings
  - Government Net Borrowing/Lending
  - Investment (% of GDP)

---

##  System Architecture  

Data Source 
      ↓  
Google Drive Upload Folder  
      ↓ (Hourly Trigger)  
Google Apps Script Automation  
      ↓  
Master Google Sheet  
      ↓ (Published as CSV)  
Excel Power Query  
      ↓  
Interactive Investment Dashboard  

---

##  Tech Stack  

- **Automation**: Google Apps Script  
- **Cloud Storage**: Google Drive  
- **Data Processing**: Microsoft Excel  
- **Transformation**: Power Query  
- **Modeling**: Advanced Excel (AVERAGEIFS, FILTER, INDEX, UNIQUE)  
- **Visualization**: Pivot Tables, Column Charts, Pie Charts  
- **Data Source**: IMF World Economic Outlook  

---

##  Automation Pipeline  

### 1️ Data Ingestion  
- Files uploaded to Google Drive  
- Supports multiple formats (.xlsx, .xls)  
- Automatic conversion to Google Sheets  

### 2️ Consolidation Engine (Apps Script)  
- Detects file MIME type  
- Converts Excel → Google Sheet (temporary)  
- Extracts data  
- Appends to master sheet (without duplicate headers)  
- Moves processed files to archive  
- Logs execution  
- Runs every 1 hour via trigger  

✔ Fully automated  
✔ Zero manual download  
✔ Scalable pipeline  

---

##  Dashboard Modules  

### 1️ KPI Cards (2025 Snapshot)  
-  Average Global Inflation  
-  Average Investment (% of GDP)  
-  Gross National Savings  
-  Total Countries Counted  

---

### 2️ Economic Trend Analyzer  
Interactive Pivot Chart with:  
- Year Selector  
- Country Group Filter  
- Average indicator comparison  

---

### 3️ Misery Index (Investment Risk Indicator)  

Formula:

Misery Index = Unemployment Rate + Inflation

Higher Misery → Higher Economic Risk → Lower Investment Stability  

---

### 4️ Sweet Spot Countries  

Sweet Spot Score = GDP Growth – Inflation

Criteria:
- Score > 3  
- Identifies high-growth, low-inflation economies  
- Best investment candidates  

---

### 5️ Global Contributors  
Top 10 economies contributing to global output.

---

### 6️ Growth Champions  
Countries with explosive GDP growth (Top 10).

---

### 7️ Fiscal Risk Monitor  
Identifies high borrowing nations (Bottom 10 based on Net Borrowing/Lending).

---

##  Business Impact  


- Enabled real-time economic monitoring  
- Built structured global investment scoring model  
- Eliminated file-format inconsistencies  
- Improved decision confidence using risk indicators  

---

- Source: International Monetary Fund – World Economic Outlook Database  

