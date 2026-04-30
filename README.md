# End-to-End Algorithmic Market Anomaly Detector

## Project Overview
This project is an automated, multi-asset data pipeline designed to detect severe market volatility. Built entirely in Python, the algorithm fetches live financial time-series data, establishes statistical baselines, and flags anomalous price drops. The processed data is then exported and connected to a Tableau dashboard, bridging the gap between raw algorithmic output and executive-level business intelligence.

This project demonstrates core competencies in applied computer science, specifically in API integration, algorithmic logic, and data visualization.

## Key Features
* **Automated Data Ingestion:** Utilizes the `yfinance` API to pull one year of daily historical data for diverse assets, including cryptocurrency and traditional equities.
* **Algorithmic Detection:** Calculates a rolling 20-day Simple Moving Average (SMA) and applies a threshold algorithm to automatically flag sudden drops (price falling >5% below the SMA).
* **Multi-Asset Processing:** Currently configured to iterate through a diverse portfolio profile:
  * Bitcoin (`BTC-USD`)
  * HDFC Bank (`HDFCBANK.NS`)
  * Cyient Ltd (`CYIENT.NS`)
  * Tata Consultancy Services (`TCS.NS`)
* **End-to-End Pipeline:** Automatically exports cleaned, annotated datasets as `.csv` files for seamless integration into enterprise BI tools.
* **Business Intelligence Dashboarding:** Includes a synced Tableau interface to visually isolate volatility periods, allowing non-technical stakeholders to rapidly interpret market crashes.

## Tech Stack
* **Language:** Python
* **Data Processing:** `pandas`
* **API Integration:** `yfinance`
* **Quick Visuals:** `matplotlib`
* **Business Intelligence:** Tableau Desktop

## Visual Output
*(Replace this text and the placeholder link below with your actual Tableau screenshot once uploaded to GitHub)*

<img width="1919" height="1079" alt="Screenshot 2026-04-30 160536" src="https://github.com/user-attachments/assets/441940ed-6221-4e04-a36d-a4109207009b" />


## How to Run the Pipeline

1. **Clone the repository and install dependencies:**
   Ensure Python is installed on your system, then run:
   ```bash
   pip install pandas matplotlib yfinance
