# Hi, I'm Yash 👋

<!-- Typing animation -->
<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=1A56DB&center=true&vCenter=true&width=600&lines=Data+Analyst+%26+BI+Engineer;SQL+%7C+Python+%7C+BigQuery+%7C+Power+BI;Turning+raw+data+into+real+decisions;MSBA+%40+Baruch+College+%C2%B7+New+York" alt="Typing SVG" />
</div>

<br/>

<!-- Profile views + followers -->
<div align="center">
  <img src="https://komarev.com/ghpvc/?username=yashxsainix&label=Profile+Views&color=1A56DB&style=flat" />
  <img src="https://img.shields.io/github/followers/yashxsainix?label=Followers&style=flat&color=1A56DB" />
</div>

---

## The Short Version

I started in Delhi in 2019 writing Python scripts to replace manual reporting at an auto firm. Nobody asked me to. I just could not watch people spend three hours on work a well-structured query could finish in forty seconds.

That has been the through line ever since.

Five years later I have built analytics infrastructure across industries, run A/B experiments on 1M+ customer records, founded and operated an e-commerce platform for six years using behavioral data to make every growth call, and moved to New York to finish my MS in Business Analytics at Baruch College.

I care about one thing in data work: does the output actually change a decision? If the dashboard sits in a folder nobody opens, or the model prediction never reaches the person who needs it, the work did not matter. Everything I build is designed around closing that gap.

---

## What I Am Working With

<table>
<tr>
<td valign="top" width="33%">

**Query & Code**
```
SQL          ████████████  Advanced
Python       ████████████  Advanced
R            █████████░░░  Proficient
```

</td>
<td valign="top" width="33%">

**Cloud & Pipelines**
```
BigQuery     ████████████  Daily use
GCP          ██████████░░  Proficient
dbt          ████████░░░░  Proficient
Prefect      ███████░░░░░  Working knowledge
Kafka        ██████░░░░░░  Working knowledge
```

</td>
<td valign="top" width="33%">

**BI & Visualization**
```
Power BI     ████████████  Advanced
Tableau      ██████████░░  Proficient
Looker       ██████░░░░░░  Familiar
Excel        ████████████  Advanced
```

</td>
</tr>
</table>

---

## Four Projects. All Real Data. All Public.

> Every project below uses real public datasets. The findings are what actually came out of the analysis, not what I expected going in.

<br/>

### 01 &nbsp; Customer Churn Prediction
`Python` &nbsp; `Scikit-learn` &nbsp; `SQL` &nbsp; `SSMS` &nbsp; `Power BI` &nbsp; `Random Forest`

The goal was to predict which telecom customers were about to leave. The answer turned out to be simpler than most models make it look.

Month-to-month contract customers churned at over **3x** the rate of customers on annual contracts. Customers past the **12-month** tenure mark were significantly less likely to leave regardless of billing amount. The Random Forest classifier hit **84% accuracy** on held-out test data.

The Power BI dashboard was built specifically so a retention team could act on the findings without pulling an analyst each time. Churn risk by contract type, tenure band, and monthly charge, filterable and refreshable.

**[View Project](https://github.com/yashxsainix/Customer_Churn_Analysis)**

---

### 02 &nbsp; NYC Housing Equity and Policy Analytics
`R` &nbsp; `Quarto` &nbsp; `Random Forest` &nbsp; `Spatial Analysis` &nbsp; `tidycensus` &nbsp; `NYC Open Data APIs`

The research question: does neighborhood income shape how the city responds to housing complaints?

Pulled 2023 data from four public APIs (NYC 311, HPD, DOB, American Community Survey), used spatial joins to aggregate complaint rates and resolution times at the census tract level, and trained a Random Forest to predict neighborhood median income from complaint system features alone.

Out-of-sample **R² = 0.54**. Outperformed OLS and Elastic Net baselines.

The finding that drives the whole project: lower-income neighborhoods wait longer for housing complaint resolutions across heating, water, and structural categories. The gap is widest for complaints that go unresolved entirely. Income inequality is not just external context in this data. It is baked into how the system responds.

**[View Project](https://github.com/yashxsainix/STA9750-2025-FALL)**

---

### 03 &nbsp; Online Retail Analytics
`Python` &nbsp; `SQL` &nbsp; `SQLite` &nbsp; `Power BI` &nbsp; `DAX`

Two years of UK e-commerce transaction data from the UCI repository. Cleaned and merged raw Excel files in Python, loaded to SQLite, ran SQL analysis across sales trends, product returns, and customer behavior, and connected structured outputs to Power BI.

The top **27%** of customers by activity generated roughly **80%** of total revenue, **$13.4M of $17.4M**. The dashboard surfaces this as a filterable slicer so a marketing team can work directly with the segmentation without rerunning the analysis.

Built two dashboard themes, light and dark, with full DAX documentation and a recorded walkthrough.

**[View Project](https://github.com/yashxsainix/Online-Retail-Data-Analytics-Project-with-Python-SQL-and-Power-BI)**

---

### 04 &nbsp; MTA Turnstile Data Engineering
`Python` &nbsp; `GCP` &nbsp; `BigQuery` &nbsp; `dbt` &nbsp; `Prefect` &nbsp; `Kafka` &nbsp; `Spark`

This one is less about findings and more about infrastructure. The goal was to build a production-style data pipeline on real MTA turnstile records and document every layer properly.

Ingested entry and exit counts from public sources, applied Python-based validation, loaded to BigQuery via Prefect-orchestrated ETL, modeled the warehouse in dbt with staging and core layers. Weekday morning windows at high-volume stations carry **2 to 3x** the ridership of midday periods. Stations near lower-income census tracts show consistent ridership drops on evenings and weekends.

Extended with a Kafka and Spark streaming layer and a foot-traffic classification model. Full architecture walkthrough in the repo.

**[View Project](https://github.com/yashxsainix/turnstile-engineering)**

---

## GitHub Activity

<div align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=yashxsainix&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&title_color=1A56DB&icon_color=0EA5E9" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=yashxsainix&layout=compact&theme=tokyonight&hide_border=true&langs_count=6&title_color=1A56DB" />
</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com?user=yashxsainix&theme=tokyonight&hide_border=true&ring=1A56DB&fire=0EA5E9&currStreakLabel=1A56DB" />
</div>

---

## A Few Things Worth Knowing

**On how I work**

I do not start with the model. I start with the question. Half the time the answer is a well-structured SQL query and a clean chart. The other half it is a pipeline problem before it is an analytics problem. Knowing which one you are dealing with early saves a lot of wasted effort.

**On the projects above**

These are not tutorial follow-alongs. They are built on real public datasets with real analytical questions. Some findings confirmed what I expected. Some did not. The NYC housing project in particular changed how I think about what administrative data actually captures.

**On where I am headed**

I am finishing my MSBA at Baruch in May 2026 and looking for full-time roles in data analytics, BI, or data science in New York. If you are building a data team that has to move fast on real problems, I would like to talk.

---

## Background

```
2019        Junior Data Analyst · Daijex Auto Industries · New Delhi
            First real data role. Built Python and Excel pipelines
            to replace manual reporting. Learned that clean data
            is a design problem before it is a technical one.

2020        Founded Gharstuff
            E-commerce platform. Six years. Every growth decision
            made by reading behavioral data with a limited budget
            and no safety net.

2020-2021   Digital Marketing Intern · JOJA Surgical · Delhi
            Google Ads, paid social, SEO. 55k+ customer dataset.
            Where I learned that data without a decision attached
            to it is just noise.

2022-2024   Data Analyst · i3 Infosoft · Noida
            A/B experiments, Python segmentation models,
            automated SQL pipelines, Power BI dashboards.
            1M+ CRM records. Real production work.

2024        Moved to New York
            MS in Business Analytics · Baruch College
            Pliner Bloom Scholar. GPA 3.6.

2025        Data Specialist Intern · RF CUNY · New York
            SQL and BigQuery pipelines across 26 institutions.
            55% faster reporting. 37% accuracy improvement.
            Still going.
```

---

## Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-1A56DB?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yash-saini-analyst/)
[![Email](https://img.shields.io/badge/Gmail-Say+Hello-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:yashsaini30668@gmail.com)
[![Portfolio](https://img.shields.io/badge/GitHub-Projects-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/yashxsainix)

</div>

<br/>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:1A56DB,100:0EA5E9&height=100&section=footer&text=Open+to+Full-Time+Roles+%C2%B7+Summer+2026&fontSize=14&fontColor=ffffff&fontAlignY=65" />
</div>
