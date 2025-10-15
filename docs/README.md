## 📘 Data Description

This section provides a summary of the datasets used in the **PowerCo SME Churn Analysis** project, as documented in the *Data Description.pdf* file.  
The analysis is based on two main datasets: **client_data.csv** and **price_data.csv**, both containing information about customer behavior, energy usage, and pricing.

---

### 🧩 client_data.csv

Contains company-level client information, energy consumption history, and contract details.  
Each row represents one client company, uniquely identified by the `id` field.

Key columns include:
- **id** – Client company identifier  
- **activity_new** – Type of business activity  
- **channel_sales** – Sales channel code  
- **cons_12m / cons_gas_12m / cons_last_month** – Energy and gas consumption over time  
- **date_activ / date_end / date_renewal** – Contract activation, end, and renewal dates  
- **forecast_cons_12m / forecast_cons_year** – Predicted energy consumption  
- **margin_gross_pow_ele / margin_net_pow_ele / net_margin** – Profitability metrics  
- **nb_prod_act** – Number of active products and services  
- **has_gas** – Indicates if the client also purchases gas  
- **origin_up** – Original electricity campaign source  
- **pow_max** – Subscribed maximum power  
- **churn** – Target variable (1 if the client churned within 3 months, 0 otherwise)

---

### 💡 price_data.csv

Contains time-based energy and power pricing information for each client.

Key columns include:
- **id** – Client company identifier  
- **price_date** – Reference date  
- **price_off_peak_var / price_peak_var / price_mid_peak_var** – Variable energy prices for different time periods  
- **price_off_peak_fix / price_peak_fix / price_mid_peak_fix** – Fixed power prices for different time periods  

---

🔒 **Note:**  
Some text-based fields (like `channel_sales`, `origin_up`, and `activity_new`) are hashed to protect client confidentiality.  
The anonymization preserves their predictive meaning for modeling purposes.
