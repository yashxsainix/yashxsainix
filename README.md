# 🧠 Data Engineer & BI Specialist – Yash Saini

```
                                 ______
                                /\  __\
                               /  \ \_/_ _  _ _
                              / /\ \__\ /\`'/\`\
                             / / /_/ / \ \_/\ \ \
                             \ \___\ \  \_\ \ \_\
                              \/___/\/   \/_/ \/_/
                               DATA   PIPELINE
```

Welcome! This README is a technical journey through my data projects. It’s designed not just to tell you what I know but to show you how I think. Recruiters often skim GitHub profiles to see clean documentation and structured projects【482062626803306†L121-L139】, so this is part résumé, part engineering notebook.

---

## 🛠️ Technical Highlights

- **SQL & Python:** Author of dozens of optimized queries and scripts that cut hours from reporting processes.  
- **BigQuery, dbt & GCP:** Architect of cloud‑native pipelines with staging, core and presentation layers.  
- **Kafka & Spark:** Built streaming ingestion and classification models on MTA turnstile data.  
- **R & Quarto:** Designed spatial analysis workflows with reproducible reports and tidyverse pipelines.  
- **BI tools:** Power BI, Tableau, Looker and Excel dashboards that drive decisions.

A professional README should make your skills easy to scan and understand【482062626803306†L159-L184】, which is why I visualised them below.

```
Skill Proficiency (0–10)
SQL       ██████████  10
Python    ██████████  10
R         ████████    8
BigQuery  █████████   9
GCP       █████████   9
dbt       ████████    7
Prefect   ██████      6
Kafka     █████       5
Spark     █████       5
Power BI  ██████████  10
Tableau   █████████   9
Looker    ██████      6
Excel     ██████████  10
```

---

## 📊 Project Impact Visualized

Below is a quick bar chart in plain text showing the relative impact of my four major projects (scores scaled 0–100). Visuals like this help non‑technical stakeholders understand results quickly【364094732692674†L202-L215】.

```
Impact Score (% – higher is better)
Churn Prediction       [████████████████████░░] 84
Housing Equity         [███████████████░░░░░] 54
Retail Analytics       [███████████████████░] 80
Turnstile Engineering  [█████████████████░░] 75
```

---

## 🚀 Deep Dives

Each of these repositories is pinned on my profile so you can find them easily【482062626803306†L48-L83】. Click the project name to explore code, documentation and dashboards.

### 1. [Customer Churn Prediction](https://github.com/yashxsainix/Customer_Churn_Analysis)

- **Goal:** Predict which telecom customers will leave next month.  
- **Tech:** Python, SQL, Scikit‑learn, Random Forest, Power BI.  
- **Key Results:** Month‑to‑month contracts churn **3×** as often as annual contracts. Tenure >12 months strongly reduces churn. Model accuracy **84 %**.  
- **Highlight:** Self‑serve dashboard for retention teams — no analyst needed to run scenarios.

*Sample pipeline code (dbt model)*

```sql
-- models/churn_by_contract.sql
WITH churn_base AS (
  SELECT customer_id,
         contract_type,
         tenure,
         monthly_charge,
         CASE WHEN churned = 'Yes' THEN 1 ELSE 0 END AS churn_flag
  FROM telecom_customers
),
contract_agg AS (
  SELECT contract_type,
         COUNT(*) AS total_customers,
         SUM(churn_flag) AS churn_count
  FROM churn_base
  GROUP BY 1
)
SELECT contract_type,
       churn_count / total_customers AS churn_rate
FROM contract_agg
ORDER BY churn_rate DESC;
```

### 2. [NYC Housing Equity & Policy Analytics](https://github.com/yashxsainix/STA9750-2025-FALL)

- **Goal:** Does neighbourhood income influence how the city resolves housing complaints?  
- **Tech:** R, Quarto, Random Forest, Spatial analysis, NYC Open Data APIs.  
- **Key Results:** Lower‑income neighbourhoods experience longer resolution times across heating, water and structural complaints. Random Forest predicting median income achieves **R² = 0.54**.  
- **Highlight:** Reproducible report with interactive maps and code notebooks.

*Sample analysis snippet*

```r
library(sf)
library(randomForest)
# Merge 311 complaints with census tract income
data <- merge(complaints_sf, census_income, by = "tract_id")
# Fit Random Forest to predict log income from complaint features
model <- randomForest(log(median_income) ~ complaint_type + resolution_time + building_age,
                      data = data,
                      ntree = 500)
print(model$r.squared)
```

### 3. [Online Retail Analytics](https://github.com/yashxsainix/Online-Retail-Data-Analytics-Project-with-Python-SQL-and-Power-BI)

- **Goal:** Understand sales drivers in a two‑year e‑commerce dataset.  
- **Tech:** Python, SQL, SQLite, Power BI, DAX.  
- **Key Results:** Top **27 %** of customers generate **80 %** of revenue (~$13.4 M).  
- **Highlight:** Dual‑theme dashboard (light & dark) with DAX documentation.

*Sample SQL snippet*

```sql
-- Identify high-value customers
temp AS (
  SELECT customer_id,
         SUM(quantity * unit_price) AS total_spent
  FROM orders
  GROUP BY customer_id
)
SELECT customer_id,
       total_spent,
       NTILE(4) OVER (ORDER BY total_spent DESC) AS quartile
FROM temp
ORDER BY total_spent DESC;
```

### 4. [MTA Turnstile Engineering](https://github.com/yashxsainix/turnstile-engineering)

- **Goal:** Build a production‑style pipeline on MTA turnstile data.  
- **Tech:** Python, BigQuery, dbt, Prefect, Kafka, Spark.  
- **Key Results:** Morning ridership at high‑volume stations is **2–3×** midday levels; stations in lower‑income tracts see lower evening/weekend traffic.  
- **Highlight:** ETL, streaming, and classification layers documented with clear architecture diagrams.

*Sample Kafka consumer snippet*

```python
from kafka import KafkaConsumer
import json

consumer = KafkaConsumer(
    'turnstile-events',
    bootstrap_servers=['broker1:9092','broker2:9092'],
    value_deserializer=lambda m: json.loads(m.decode('utf-8'))
)
for message in consumer:
    event = message.value
    process_turnstile_event(event)  # custom function to validate and load data
```
```

---

## 🔄 Future Enhancements

I’m always exploring new ways to make my profile more engaging. Ideas include:

- A **guestbook** powered by GitHub Actions where visitors can leave comments【664671821327278†L82-L93】.  
- A **live hit counter** displaying visitor counts【664671821327278†L98-L103】.  
- A **self‑updating section** showing recent blog posts or commits【664671821327278†L148-L153】.  
- Mini‑games like **Connect‑4** or **Chess** embedded in the README via issue comments【664671821327278†L107-L123】.  

---

## 📬 Connect

- **LinkedIn:** [linkedin.com/in/yash-saini-analyst](https://www.linkedin.com/in/yash-saini-analyst/)  
- **Email:** [yashsaini30668@gmail.com](mailto:yashsaini30668@gmail.com)  
- **GitHub:** [github.com/yashxsainix](https://github.com/yashxsainix)

If you’re building data products and need someone who starts with the question rather than the model, let’s chat. A professional photo and concise bio help create a strong first impression on your profile【482062626803306†L85-L118】.

