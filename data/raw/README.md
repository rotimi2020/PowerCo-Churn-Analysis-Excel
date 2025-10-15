## 📊 Dataset Overview

The **PowerCo Churn Analysis** project is built on two main datasets — `client_data.csv` and `price_data.csv`.  
Together, they capture customer details, consumption behavior, contract timelines, and pricing patterns.

---

### 🧾 client_data.csv

This dataset contains one record per client and includes information about their energy usage, contract activity, and churn status.

**Main columns:**
- **id** – Unique client identifier  
- **channel_sales** – Sales channel code  
- **cons_12m / cons_gas_12m / cons_last_month** – Electricity and gas consumption metrics  
- **date_activ / date_end / date_modif_prod / date_renewal** – Contract start, end, modification, and renewal dates  
- **forecast_cons_12m / forecast_cons_year** – Forecasted electricity consumption for future periods  
- **forecast_discount_energy / forecast_meter_rent_12m** – Predicted discounts and meter rental costs  
- **forecast_price_energy_off_peak / forecast_price_energy_peak / forecast_price_pow_off_peak** – Forecasted energy and power prices  
- **has_gas** – Indicates if the client also uses gas services  
- **imp_cons** – Current paid consumption  
- **margin_gross_pow_ele / margin_net_pow_ele / net_margin** – Profit and margin-related metrics  
- **nb_prod_act** – Number of active products  
- **num_years_antig** – Years of customer relationship  
- **origin_up** – Code for the initial campaign the client joined from  
- **pow_max** – Subscribed maximum power  
- **churn** – Target variable (1 = churned, 0 = retained)

---

### 💰 price_data.csv

This dataset provides energy and power pricing by time period for each client.

**Main columns:**
- **id** – Client identifier (links to `client_data.csv`)  
- **price_date** – Reference date for pricing  
- **price_off_peak_var / price_peak_var / price_mid_peak_var** – Variable energy prices for different time periods  
- **price_off_peak_fix / price_peak_fix / price_mid_peak_fix** – Fixed power prices for different time periods  

---

🔒 **Note:**  
Some text-based fields (like sales channels and campaign origins) are hashed for privacy.  
Their encoded values still retain meaningful differences useful for churn prediction.
