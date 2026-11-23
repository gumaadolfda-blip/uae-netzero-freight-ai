# UAE NetZero Freight: Multi-Source Supply Chain & Maritime Decarbonization Engine

**Author:** Guma Adolf | Founder & Lead Data Architect, NG Advisory Co.  
**Live Interactive App:** [gumadolffofficial.streamlit.app](https://streamlit.app)  
**LinkedIn:** [://linkedin.com](https://www.://linkedin.com)  
**Policy Alignment:** UAE Net Zero 2050 Strategy | Federal Decree-Law No. 11/2023 (Carbon Reporting)  

---

## Executive Summary
**UAE NetZero Freight** is an end-to-end machine learning and generative AI pipeline analyzing **43,020 port-day records** across **15 UAE maritime ports** (including Fujairah, Jebel Ali, Khalifa Port, and Khor Fakkan). By integrating high-frequency vessel traffic with macroeconomic trade figures and supply chain delay benchmarks, the engine quantifies both **environmental abatement (metric tons of CO₂ reduced)** and **commercial ROI (AED saved)**.

![UAE NetZero Freight Executive Summary](UAE%20NetZero%20Freight%20SUMMARY%20.png)

### Key Quantified Outcomes
* **6,487,570 AED** in projected annual marine fuel savings across UAE ports via a 15% reduction in offshore vessel idling (*"Just-in-Time"* arrival scheduling).
* **~9,287 Metric Tons of CO₂** abated annually across UAE maritime corridors.
* **81.1% Classification Accuracy** on a Random Forest Early-Warning model flagging high-congestion port surge days before bottlenecks form.
* **24,522 Metric Tons MAE** on national daily cargo volume forecasting across 15 ports simultaneously.

---

## Core Research & Policy Questions Answered
1. **Operational Forecasting (Predictive ML):** Can daily cargo tonnage and vessel surges be predicted 7 days in advance across major UAE ports using historical momentum and UAE calendar patterns?
2. **Carbon Baseline & Hotspots (Sustainability Auditing):** Which UAE ports generate the highest vessel-weighted anchorage emissions across tanker, container, dry bulk, and Ro-Ro traffic?
3. **Financial & Environmental ROI (Scenario Modeling):** How much CO₂ and marine fuel (AED) can be saved annually by cutting offshore idling by 15%?
4. **Macro-Economic Efficiency (Multi-Source Integration):** How does maritime emissions intensity relate to monthly UAE non-oil trade volume (~134.6B AED benchmark)?
5. **Executive Decision Automation (Generative AI):** How can grounded LLM workflows (`gemini-2.5-flash`) translate raw ML forecasts into instant, hallucination-free executive briefings?

---

## Multi-Source Data Architecture
* **Spine Dataset:** *United Arab Emirates: Daily Port Activity Data and Shipment Estimates* (IMF PortWatch / UN Global Platform via HDX).
* **Macro Trade Layer:** *UAE Foreign Trade Volume per Month* (Bayanat.ae — UAE Official Open Data Portal).
* **Delay Risk Layer:** *DataCo Smart Supply Chain Dataset* (Empirical late-delivery risk benchmarking).

---

## Tech Stack
* **Data Engineering & Analysis:** Python (`pandas`, `numpy`, `openpyxl`)
* **Machine Learning & Explainability:** `scikit-learn` (`RandomForestRegressor`, `RandomForestClassifier`, Feature Importance, Decision Tree Visualization, Confusion Matrix)
* **Visualization:** `matplotlib`, `seaborn`
* **Generative AI Reporting:** Google GenAI SDK (`gemini-2.5-flash` with grounded KPI prompts)

---

## How to Run Locally
1. Clone this repository:
   ```bash
   git clone https://github.com
   ```
2. Install required packages:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn openpyxl google-genai
   ```
3. Open `UAE_NetZero_Freight.ipynb` in JupyterLab or VS Code and run all cells sequentially.
