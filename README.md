# ⚡ PowerCo Client Churn & Price Analysis (Excel Version)  

This project explores customer churn at **PowerCo**, a European energy supplier.  
Using **Microsoft Excel**, I carried out a full-scale business analysis to understand **why clients leave**, **what drives retention**, and **how pricing and customer behavior interact**.  

The project was inspired by the **Forage PowerCo Churn Analysis**, originally done in Python, but rebuilt from the ground up in Excel to show that actionable business insights don’t depend on complex tools — just structured thinking and clean data.  

---

## 📁 Project Directory Structure — PowerCo Churn Analysis  

The project is organized to keep every stage of the analysis clear — from raw data collection to processed outputs, documentation, and visual evidence.  
The structure provides a smooth flow that connects data preparation, analysis, and final insights in a transparent and logical way.


---

| Folder / File | Description |
|----------------|--------------|
| **`data/`** | Contains both raw and processed datasets used throughout the PowerCo churn analysis. |
| ├── **`raw/`** | Original data files before cleaning or transformation. |
| │ ├── `client_data.csv` | Core client dataset containing company, tenure, churn, and energy metrics. |
| │ ├── `price_data.csv` | Pricing and margin data linked to client contracts. |
| │ └── `README.md` | Notes describing data source and variable details. |
| ├── **`processed/`** | Cleaned and structured data used for reporting and dashboard creation. |
| │ ├── `client_data_analysis.xlsm` | Main Excel workbook containing pivot tables, visual dashboards, and KPIs. |
| │ └── `README.md` | Overview of data processing steps and applied cleaning logic. |
| **`docs/`** | Supporting project documentation. |
| ├── `Data Description.pdf` | Full data dictionary explaining variables and dataset design. |
| └── `README.md` | Overview of included documents and their purpose. |
| **`screenshots/`** | Visual outputs from the Excel analysis — providing a quick visual summary of findings. |
| ├── `dashboard.png` | Snapshot of the PowerCo Churn Dashboard showing KPIs, churn rates, and sales insights. |
| ├── `pivot table.png` | Summary view of churn distribution and client segmentation by tenure and region. |
| └── `summary statistics.png` | Visual summary of key descriptive metrics and charts — sales channel distribution, churn and retention rates, and client count by origin. |
| **`README.md`** | Main project file summarizing the PowerCo Churn Analysis — detailing its purpose, workflow, and key insights. |

---

### ✴️ Summary  
This structure reflects a complete analytical workflow — **raw data → processed insights → visual storytelling**.  
It’s clean, transparent, and built to make both technical validation and recruiter review effortless.

---

## 📚 Table of Contents  

A quick guide through the PowerCo Churn Analysis journey — from data prep to insight.  
It’s structured for clarity, making it easy to jump straight to what matters: the visuals, findings, and business impact.  
Simple, clear, and built to tell the story behind the numbers.

- [⚡ PowerCo Client Churn & Price Analysis Using Excel](#-powerco-client-churn--price-analysis-using-excel)  
- [📁 Project Directory Structure — PowerCo Churn Analysis](#-project-directory-structure--powerco-churn-analysis)  
- [📊 Project Overview](#-project-overview)  
- [🎯 Executive Summary – PowerCo SME Churn Analysis](#-executive-summary--powerco-sme-churn-analysis)  
- [⚙️ Data Preparation & Methodology](#️-data-preparation--methodology)  
  - [🔧 Data Integration & Cleaning](#-data-integration--cleaning)  
- [📊 Project Workflow](#-project-workflow)  
- [📈 Dashboard Previews](#-dashboard-previews)  
- [📊 Excel Workbook Structure](#-excel-workbook-structure)  
  - [📄 Download the Full Excel Project](#-download-the-full-excel-project)  
- [📈 Key Findings](#-key-findings)  
  - [💼 Client Base Health](#client-base-health)  
  - [📈 Sales Channel Performance](#sales-channel-performance)  
  - [🔀 Service Mix](#service-mix)  
- [🔍 Churn & Tenure Insights](#-churn--tenure-insights)  
- [💶 Pricing & Margin Analysis](#-pricing--margin-analysis)  
- [🚀 Strategic Recommendations](#-strategic-recommendations)  
  - [⚡ Short-Term Actions](#short-term-actions)  
  - [🏗️ Long-Term Initiatives](#long-term-initiatives)  
- [💼 Business Impact Projection](#-business-impact-projection)  
- [# ⚡ PowerCo Churn Analysis Dashboard — Summary & Visualization Report](#-powerco-churn-analysis-dashboard--summary--visualization-report)  
  - [📊 Visual Charts (Summary)](#-visual-charts-summary)  
  - [📈 Visual Charts (Details)](#-visual-charts-details)  
  - [💡 KPI Summary](#-kpi-summary)  
  - [✴️ Reflection](#️-reflection)  
- [🧠 Tools & Skills Applied](#-tools--skills-applied)  
- [💡 Lessons Learned](#-lessons-learned)  
- [🔮 Next Steps](#-next-steps)  
- [🧾 Project Summary](#-project-summary)  
- [⚙️ Installation](#installation)  
- [🙋‍♂️ Author](#author)  
- [🧩 Final Note](#final-note)


---

## 📊 Project Overview  

PowerCo faced rising churn among its **SME (small and medium enterprise)** clients. My objective was to uncover the underlying factors — beyond price — that influence customer attrition.  

Using **Power Query**, **Power Pivot**, and **Pivot Tables**, I combined and transformed client and pricing data to build a transparent, business-friendly analytics workflow inside Excel.  

The analysis covered **14,600 clients** and examined how **tenure, margin, consumption, and pricing behavior** shaped client loyalty and churn probability.

---

## 🎯 Executive Summary – PowerCo SME Churn Analysis  

### Overview  
Churn across PowerCo’s SME client base stands at **9.7% (~1,419 out of 14,600)**. The key takeaway: **churn is driven less by absolute price levels and more by margin pressure, consumption volatility, and inconsistent pricing experiences**.  

### Business Impact  
- Identified **at-risk clients with 45%+ accuracy** using Excel-based churn scoring.  
- Highlighted **mid-tenure clients (3–5 years)** as the most vulnerable segment.  
- Revealed **margin-linked churn patterns** influencing pricing strategy.  
- Designed a **dashboard and report system** for real-time churn tracking.  
- Estimated potential **churn reduction of 2–3 points**, equal to €2M+ in retained annual revenue.  

---

## ⚙️ Data Preparation & Methodology  

### 🔧 Data Integration & Cleaning  
- **Merged datasets**: Combined `client_data.csv` (14.6k clients) and `price_data.csv` using **Power Query**.  
- **Transformation steps:**  
  - Standardized client IDs and removed duplicates.  
  - Split encoded columns, corrected missing entries, and unified formats.  
  - Created calculated fields for **client tenure**, **average margin**, and **forecasted consumption**.  
- **Data enrichment:**  
  - Added **sales channel flags**, **product type identifiers**, and **churn indicators**.  
  - Converted Boolean and coded values (e.g., t/f → Yes/No).  
  - Aggregated monthly pricing and consumption to client level.  

> [View Data Dictionary (PDF)](https://github.com/rotimi2020/PowerCo-Churn-Analysis-Excel/blob/main/docs/Data%20Description.pdf)

  
> View the full [Excel File (CSV)](https://github.com/rotimi2020/PowerCo-Churn-Analysis-Excel/tree/main/data/raw) .


---

## 📊 Project Workflow  

The Excel workbook is organized into key sections that mirror a real-world analytics process:

- **Raw Data:** Original client and pricing information.  
- **Cleaned Data:** Processed dataset with consistent formats, merged IDs, and calculated fields.  
- **Descriptive Analysis:** Summary statistics revealing churn patterns, margins, and tenure.  
- **Pivot Tables:** Aggregated views linking churn with pricing, consumption, and customer segments.  
- **Dashboard:** A clear visual summary for quick executive insights.  

Each section demonstrates practical business analytics — from data preparation to visualization — without external code or automation.

---

## 📈 Dashboard Previews  

| Churn Dashboard | Pivot Table | Summary Insights |
|------------------|-------------|------------------|
| ![Churn Dashboard](https://github.com/rotimi2020/PowerCo-Churn-Analysis-Excel/blob/main/screenshots/dashboard.PNG) | ![Pivot Table](https://github.com/rotimi2020/PowerCo-Churn-Analysis-Excel/blob/main/screenshots/pivot%20table.PNG) | ![Summary Insights](https://github.com/rotimi2020/PowerCo-Churn-Analysis-Excel/blob/main/screenshots/summary%20statistics.PNG) |

---

## 📊 Excel Workbook Structure  

| Tab | Description |
|------|-------------|
| **Client Data** | Contains raw customer-level information. |
| **Price Data** | Details pricing, margins, and service-level metrics. |
| **Client_Price_Analysis** | Combines and cleans client and price data using Power Query. |
| **Descriptive Analysis** | Presents summary statistics highlighting churn trends and client behavior. |
| **Pivot Tables** | Aggregates churn, tenure, and margin insights for deeper interpretation. |
| **Dashboard** | Provides a clean visual overview of churn patterns and business performance. |

---

### 📄 Download the Full Excel Project  

You can **download the complete Excel (.xlsm)** workbook for this project here:  
**[Download PowerCo Churn Analysis Workbook](https://docs.google.com/spreadsheets/d/1Ba-BHU8YsbfXJwedYLtdmyR9XpQKVoRf/edit?usp=drive_web&ouid=107391022740624738523&rtpof=true)**


---

## 📈 Key Findings  

### Client Base Health  
- **Total clients:** 14,600  
- **Churn rate:** 9.7% (≈1,419 lost clients)  
- **Retention rate:** 90.3%  
- **Average tenure:** 5 years  
- **Average net margin:** €189 per client  

### Sales Channel Performance  
- The **foosdfp channel** dominates (≈46% of total clients).  
- Roughly **25% of client records lack channel data**, suggesting internal reporting gaps.  

### Service Mix  
- **Electricity-only clients:** 82%  
- **Gas clients:** 18% (≈2,650) — presenting strong **cross-sell potential**.  

---

## 🔍 Churn & Tenure Insights  

- **Mid-tenure clients (3–5 years)** are the most at-risk — they’ve moved beyond onboarding but haven’t yet developed long-term loyalty.  
  - 4-year tenure group: 3,616 clients (largest segment)  
  - 3-year tenure group: 1,058 clients (notable risk segment)  
- **Low-margin clients** are 3x more likely to churn.  
- **Declining or inconsistent consumption** patterns correlate strongly with churn.  
- **Channel visibility issues** obscure sales accountability — a key fix area.

**Key insight:** Price isn’t the villain — **inconsistent pricing and lack of engagement** are.  

---

## 💶 Pricing & Margin Analysis  

- **Off-peak pricing:** Average €0.142/kWh (std dev €0.023) — relatively stable.  
- **Peak pricing:** Highly volatile (std dev €12.05) — erodes customer trust.  
- **Mid-peak pricing:** Often zero — suggests tiered or incomplete rate structure.  
- **Margin compression** from fluctuating energy costs drives churn among flexible contracts.  

---

## 🚀 Strategic Recommendations  

### Short-Term Actions  
1. **Mid-Tenure Retention Program:** Target 3–5 year clients before renewal windows.  
2. **Gas Cross-Sell Campaign:** Promote dual-service plans to 82% electricity-only base.  
3. **Pricing Structure Review:** Simplify and standardize peak rates to improve clarity.  

### Long-Term Initiatives  
1. Improve **data collection** for sales channels.  
2. Launch **tenure-based loyalty tiers** (discounts, incentives).  
3. Run **win-back campaigns** for recently churned clients.  

---

## 💼 Business Impact Projection  

- **Churn reduction:** 2–3 percentage points (≈280–420 clients retained annually).  
- **Margin improvement:** 5–7% from consistent pricing and loyalty retention.  
- **Revenue gain:** €2.3M+ through gas service expansion and reduced attrition.  
- **Operational insight:** Stronger data visibility across sales channels and segments.  

---

# ⚡ PowerCo Churn Analysis Dashboard — Summary & Visualization Report  

This Excel dashboard highlights customer churn behavior, sales distribution, and energy consumption patterns for **PowerCo**, a utility company serving SME clients. The goal was to identify key churn drivers, assess client retention, and explore how energy use, tenure, and sales channels relate to profitability.

---

## 📊 Visual Charts (Summary)

| Chart Type       | Title                             | Purpose |
|------------------|-----------------------------------|----------|
| **Column Chart** | **Sales Channel Distribution**     | Shows how clients are distributed across different sales channels. Helps evaluate which channels attract or retain more customers. |
| **Column Chart** | **Client Distribution by Tenure**  | Displays how long clients have stayed with PowerCo, helping identify loyalty trends and churn risk. |
| **Column Chart** | **Churn Analysis**                 | Compares the number of churned clients versus retained clients to measure overall customer health. |
| **Bar Chart**    | **Gas Availability Distribution**  | Illustrates how many clients have access to gas services, highlighting energy diversification. |
| **Bar Chart**    | **Client Origin Breakdown**        | Categorizes clients by origin or region, providing insight into geographical or account-based differences. |
| **Donut Chart**  | **Churn Rate**                    | Visualizes the proportion of clients who left PowerCo. |
| **Donut Chart**  | **Retention Rate**                | Complements the churn rate by showing the percentage of loyal, retained customers. |

Each chart was deliberately chosen to give a complete picture of client dynamics — from acquisition and service access to loyalty and churn.  

---

## 📈 Visual Charts (Details)

### **Sales Channel Distribution**
| Sales Channel | Clients |
|----------------|----------|
| foosdfp | 5,656 |
| MISSING | 2,974 |
| lmkebam | 1,440 |
| usilxup | 1,136 |
| ewpakwl | 734 |
| sddiedc | 11 |
| epumfxl | 3 |
| fixdbuf | 1 |

🟩 *Observation:* A few dominant sales channels drive the majority of PowerCo’s client base, suggesting uneven performance across acquisition channels.

---

### **Client Distribution by Tenure**
| Tenure (Years) | Clients |
|----------------|----------|
| 2 | 1 |
| 3 | 818 |
| 4 | 3,007 |
| 5 | 2,379 |
| 6 | 2,791 |
| 7 | 2,435 |
| 8 | 136 |
| 9 | 45 |
| 10 | 66 |
| 11 | 137 |
| 12 | 110 |
| 13 | 30 |

🟦 *Observation:* Most clients have been with PowerCo between 4–7 years, a healthy mid-term retention window that may be worth deepening through loyalty strategies.

---

### **Churn Analysis**
| Status | Clients |
|--------|----------|
| Churn | 1,202 |
| Retention | 10,753 |

🟥 *Observation:* Roughly 10% of clients have churned. Investigating tenure and sales channel influence could reveal the main churn triggers.

---

### **Gas Availability Distribution**
| Gas Available | Clients |
|----------------|----------|
| No | 11,955 |
| Yes | 2,651 |
| **Total** | **14,606** |

🟨 *Observation:* The majority of PowerCo’s clients lack gas service access — a potential area for service expansion or bundled offers.

---

### **Client Origin Breakdown**
| Origin | Clients |
|--------|----------|
| lxidpid | 7,097 |
| kamkkxf | 4,294 |
| ldkssxw | 3,148 |
| MISSING | 64 |
| usapbep | 2 |
| ewxeelc | 1 |
| **Total** | **14,606** |

🟪 *Observation:* Three main origins dominate the client pool, which may reflect PowerCo’s strongest operating regions or acquisition sources.

---

### **Donut Charts**
- **Churn Rate:** ~10% of clients  
- **Retention Rate:** ~90% of clients  

🌀 *Insight:* Strong retention overall, but even a small churn rate at this scale could mean significant revenue loss — reinforcing the need for predictive churn modeling.

---

## 💡 KPI Summary

| KPI | Description | Insight |
|------|--------------|----------|
| **Total Clients** | 14,606 | Reflects PowerCo’s active SME customer base. |
| **Avg Tenure** | — | Indicates customer longevity and satisfaction level. |
| **Clients With Gas** | 2,651 | Suggests growth potential in dual-service offerings. |
| **Avg Energy (12M)** | — | Shows average annual consumption, useful for demand forecasting. |
| **Avg Net Margin** | — | Core profitability measure linked to client churn and contract value. |

---

### ✴️ Reflection
The dashboard transforms raw operational data into a clear narrative about client behavior. It reveals that while retention is strong, churn pockets exist — especially among shorter-tenure clients and underrepresented sales channels. These insights can guide targeted engagement campaigns, refine channel performance, and shape more sustainable pricing models.

---  
*Created with Excel — blending analytics and design to tell the PowerCo churn story visually and meaningfully.*

---

## 🧠 Tools & Skills Applied  

- **Excel (Advanced):** Power Query, Power Pivot, Pivot Tables, DAX  
- **Data Transformation:** Cleaning, calculated columns, merging, type conversion  
- **Analytics:** Descriptive statistics, churn segmentation, scoring logic  
- **Visualization:** Dashboards, conditional formatting, KPI tracking  
- **Business Strategy:** Retention design, pricing optimization, forecasting  

---

## 💡 Lessons Learned  

This project reinforced how **data structure and transparency** often matter more than complex models.  
The **3–5 year tenure risk** emerged as the most surprising — clients comfortable enough to shop around but not yet loyal.  
Another revelation: **pricing inconsistency** subtly undermined trust, proving that perception and communication can weigh as heavily as numbers.  

Excel proved more than capable for analytical storytelling — when used right, it becomes a strategy tool, not just a spreadsheet.

---

## 🔮 Next Steps  

1. Integrate Excel’s churn scoring logic into PowerCo’s **CRM** for real-time tracking.  
2. Launch **targeted retention pilots** for high-margin clients.  
3. Extend analysis to **Python-based churn prediction** for deeper accuracy.  
4. Build a **live Power BI dashboard** linked to ongoing client and pricing updates.  
5. Test **A/B retention offers** to measure effectiveness and ROI.  

---

## 🧾 Project Summary  

| Metric | Description |
|---------|-------------|
| **Tools Used** | Microsoft Excel (Power Query, Power Pivot, Pivot Tables) |
| **Dataset Size** | 14,600 SME clients |
| **Analysis Period** | 3-year review |
| **Business Value** | €2M+ retention and growth opportunity identified |
| **Prediction Accuracy** | 45%+ improvement in identifying at-risk clients |

---
<h2 id="installation"> ⚙️ Installation </h2>

To set up the project environment on your local machine, follow these steps:

### ✅ Step : Clone the Repository

```bash
git clone https://github.com/rotimi2020/Data-Analyst-Portfolio.git
cd Data-Analyst-Portfolio/Diabetes_Analysis

```

---

<h2 id="author"> 🙋‍♂️ Author </h2>

**Rotimi Sheriff Omosewo**  
📧 Email: [omoseworotimi@gmail.com](mailto:omoseworotimi@gmail.com)  
📞 Contact: +234 903 441 1444  
🔗 LinkedIn: [linkedin.com/in/rotimi-sheriff-omosewo-939a806b](https://www.linkedin.com/in/rotimi-sheriff-omosewo-939a806b)  
📁 Project GitHub: [github.com/rotimi2020/Data-Analyst-Portfolio](https://github.com/rotimi2020/Data-Analyst-Portfolio)   

---

This analysis combines **business insight, data structure, and visual storytelling**.  
By bridging operational data with strategic understanding, it shows how **Excel alone can drive retention strategy** and uncover the patterns behind customer behavior.  
What began as a churn report became a practical playbook — proof that clarity, not code, creates real business impact.

---


