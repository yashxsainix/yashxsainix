<!-- Header -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1A56DB,100:0EA5E9&height=180&section=header&text=Yashpal%20Saini&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Data%20Analyst%20%7C%20BI%20Engineer%20%7C%20MSBA%20%40%20Baruch%20College&descAlignY=58&descSize=16&descColor=ffffff" />

</div>

---

## About Me

I started my career doing data work for an auto industry firm in Delhi in 2019. Back then it was mostly Python scripts and Excel dashboards that I built from scratch to replace manual reporting. Nobody asked me to make them — I just hated watching people waste hours on work that a well-structured query could do in seconds.

That instinct has shaped everything since.

I have spent the last five years building pipelines, models, and dashboards across industries — from CRM analytics on 1M+ customer records at a data firm in Noida, to SQL and BigQuery infrastructure supporting KPI reporting across 26 institutions at the Research Foundation of CUNY. In parallel I founded and ran an e-commerce platform for six years, where every growth decision was made by reading behavioral data with limited resources and no margin for error.

Right now I am finishing my MS in Business Analytics at Baruch College in New York (Pliner Bloom Scholar, GPA 3.6) and looking for full-time roles in data analytics, business intelligence, or data science.

The four projects pinned below are the work I am most proud of. They are all built on real public datasets, documented thoroughly, and written for someone who wants to understand not just what I did, but what I found.

---

## Tech Stack

<div align="center">

**Query & Languages**

![SQL](https://img.shields.io/badge/SQL-Advanced-1A56DB?style=for-the-badge&logo=postgresql&logoColor=white)
![Python](https://img.shields.io/badge/Python-Pandas%20%7C%20NumPy%20%7C%20Scikit--learn-1A56DB?style=for-the-badge&logo=python&logoColor=white)
![R](https://img.shields.io/badge/R-Tidyverse%20%7C%20Quarto%20%7C%20ranger-1A56DB?style=for-the-badge&logo=r&logoColor=white)

**Cloud & Pipelines**

![GCP](https://img.shields.io/badge/Google%20Cloud-BigQuery%20%7C%20GCS-0EA5E9?style=for-the-badge&logo=googlecloud&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-Data%20Modeling-0EA5E9?style=for-the-badge&logo=dbt&logoColor=white)
![Prefect](https://img.shields.io/badge/Prefect-Orchestration-0EA5E9?style=for-the-badge&logo=prefect&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-Streaming-0EA5E9?style=for-the-badge&logo=apachekafka&logoColor=white)

**BI & Visualization**

![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboards%20%7C%20DAX-F59E0B?style=for-the-badge&logo=powerbi&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-Visualization-F59E0B?style=for-the-badge&logo=tableau&logoColor=white)

</div>

---

## Projects

### Customer Churn Prediction
`Python` `Scikit-learn` `SQL` `Power BI` `SSMS`

Built an end-to-end churn analytics pipeline on a telecom dataset. SQL-based EDA in SSMS, Random Forest classifier at 84% accuracy, and a Power BI dashboard that segments churn risk by contract type, tenure, and billing — designed so a retention team can act on it without pulling an analyst every time.

The most interesting finding: month-to-month contract customers churned at more than 3x the rate of annual contract customers. Customers past the 12-month tenure mark were significantly less likely to leave regardless of how much they were paying.

---

### NYC Housing Equity & Policy Analytics
`R` `Quarto` `Random Forest` `Spatial Analysis` `tidycensus` `NYC Open Data`

Pulled 2023 data from four public APIs — NYC 311, HPD, DOB, and the American Community Survey — and used spatial joins to aggregate complaint patterns and resolution times at the census tract level.

Trained a Random Forest model that predicted neighborhood median income from housing complaint features alone and reached an out-of-sample R² of 0.54, outperforming OLS and Elastic Net baselines. The finding that drives the whole project: income inequality is not just external context in NYC housing data — it is encoded in the complaint system itself. Lower-income neighborhoods wait longer for resolutions, and the gap is widest for complaints that go unresolved entirely.

---

### Online Retail Analytics
`Python` `SQL` `SQLite` `Power BI` `DAX`

Full pipeline on the UCI Online Retail dataset covering two years of UK e-commerce transactions. Cleaned and merged raw Excel files in Python, loaded to SQLite, ran SQL analysis across sales trends, returns, and customer behavior, and connected structured outputs to a dual-theme Power BI dashboard.

Key finding: the top 27% of customers by activity generated roughly 80% of total revenue ($13.4M of $17.4M). Classic Pareto dynamics surfaced as a filterable slicer so a marketing team can work directly with it.

---

### MTA Turnstile Data Engineering
`Python` `GCP` `BigQuery` `dbt` `Prefect` `Kafka` `Spark`

Production-style data engineering pipeline on real MTA turnstile records. Ingested entry and exit counts from public sources, applied Python-based validation and cleaning, and loaded structured data into BigQuery via Prefect-orchestrated ETL workflows. Modeled the warehouse in dbt with staging and core layers.

Weekday morning windows at high-volume stations carry 2 to 3x the ridership of midday periods. Stations near lower-income census tracts show consistent ridership drops on evenings and weekends. Extended the project with a Kafka and Spark streaming layer and a foot-traffic classification model.

---

## GitHub Stats

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=yashxsainix&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yashxsainix&layout=compact&theme=tokyonight&hide_border=true&langs_count=6" />

</div>

---

## Currently

- Finishing MSBA at Baruch College (expected May 2026)
- Working as Data Specialist Intern at Research Foundation of CUNY
- Looking for full-time roles in data analytics, BI, or data science starting Summer 2026
- Improving the streaming and ML monitoring layer on the MTA project

---

## Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-yashpal--saini-1A56DB?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/yash-sainianalyst)
[![Email](https://img.shields.io/badge/Email-yashsaini30668%40gmail.com-1A56DB?style=for-the-badge&logo=gmail&logoColor=white)](mailto:yashsaini30668@gmail.com)

</div>

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0EA5E9,100:1A56DB&height=100&section=footer" />
</div>
