# UAE NetZero Freight: Multi-Source Supply Chain & Maritime Decarbonization Engine

**Author:** Guma Adolf | Founder & Lead Data Architect, NG Advisory Co.  
**Live Interactive App:** [gumadolffofficial.streamlit.app](https://gumadolffofficial.streamlit.app)  
**LinkedIn:** [linkedin.com/in/gumadolf](https://www.linkedin.com/in/gumadolf)  
**Policy Alignment:** UAE Net Zero 2050 Strategy | Federal Decree-Law No. 11/2023 (Carbon Reporting)

---

## Executive Summary

![UAE NetZero Freight Executive Summary](UAENetZero%20Executive%20Summary.png)

### 1. Key Decarbonization & Fuel Impact
* **JIT Idling Reduction:** 15%
* **Projected Annual CO2 Abated:** 94,395.7 tons
* **Projected Annual Fuel Savings:** AED 65,927,158
* **Scope:** 15 ports analyzed

### 2. Priority Port Hotspots
* **Fujairah:** 216,053 predicted tons per day
* **Jebel Ali:** 59,012 predicted tons per day

### 3. Ongoing Refinement Note
* **Status:** Ongoing work in progress; features and assumptions are being refined.

---

## Data Architecture & Analytical Highlights

This pipeline integrates **43,110 port-day observations** across **15 UAE ports** by combining:
* **IMF PortWatch Maritime Activity:** Daily vessel arrivals (`portcalls`, `portcalls_cargo`) and cargo volumes (`import`, `export`, `total_tonnage`).
* **Bayanat UAE Foreign Trade Data:** Monthly UAE foreign trade benchmarks (`uae_monthly_trade_aed` and `trade_per_call_aed`) aligned to port operations.
* **Supply Chain & Congestion Benchmarks:** Delay and idling multipliers used to model Just-In-Time (JIT) arrival fuel and $\text{CO}_2$ impacts.
* **Out-of-Sample Evaluation & Feature Drivers:** Evaluates 60-day actual vs. predicted cargo tonnage for **Jebel Ali** and **Fujairah** alongside `RandomForestRegressor` feature importances (`tonnage_roll_mean_7d`, `import`, `export`, vessel calls, lag/rolling indicators, calendar features, and trade intensity).

---

## Repository Structure

```text
uae-netzero-freight-ai/
├── UAE_NetZero_Freight.ipynb           # End-to-end data ingestion, feature engineering, ML modeling & JIT simulation
├── UAENetZero Executive Summary.png    # Executive summary visual dashboard
├── README.md                           # Project documentation, summary metrics, and executive conclusion
└── .gitignore                          # Excludes local .env credentials and temporary artifacts
