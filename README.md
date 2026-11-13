# Hi there, I'm Razi Mirzəyev 👋
### Data Analyst & Business Intelligence Developer | SQL • Python • Power BI • Excel • Machine Learning

I specialize in transforming large-scale, complex datasets into actionable business strategies through **Relational Database Engineering (MySQL)**, **Statistical Data Analysis (Python)**, **Business Intelligence (Power BI, DAX & Advanced Excel)**, **Audit Analytics**, and **Predictive Machine Learning (Scikit-Learn)**.

---

## 🛠️ Technical Skills & Stack

- **Databases & SQL:** MySQL 8.0, Relational Database Design (3NF & Star Schema), CTEs, Window Functions, Views, Stored Procedures, Query Optimization
- **Programming & Data Analysis:** Python, Pandas, NumPy, PyArrow (Parquet Processing), SciPy (Parametric & Non-Parametric Hypothesis Testing, ANOVA, Kruskal-Wallis)
- **Data Visualization & BI:** Power BI Desktop, DAX Measures, Star Schema Data Modeling, Advanced Excel, Matplotlib, Seaborn
- **Machine Learning:** Scikit-Learn, Feature Engineering, Anti-Leakage Validation (`GroupShuffleSplit` / `GroupKFold`), Ridge Regression, Random Forest, Gradient Boosting (GBDT), Hyperparameter Tuning, Permutation Importance
- **Tools & Workflow:** Git, GitHub, Audit & Financial Data Analytics, Java

---

## 🚀 Featured Data Analytics Portfolio Projects

### 1. ✈️ [Airfare Time Machine – US Domestic Flight Price Analytics & ML](https://github.com/Razi-mirzayev/Airfare-Time-Machine)
> **End-to-End Data Engineering, SQL, Python, Power BI & Machine Learning Project on 38,584,829 Flight Observations**

- **Database Architecture (MySQL 8.0):** Engineered a 5-table normalized **3NF + Star Schema** database (`dim_airports`, `dim_routes`, `dim_airlines`, `fact_daily_fares`, `fact_flight_prices`) across **38.58M granular flight observations** and **1.68M daily route summaries** covering 16 US hub airports and 50 directional routes.
- **Analytical SQL & Aviation Economics:** Wrote 10 production SQL analyses uncovering the **31–60 Day Booking Sweet Spot** (`$185.40` median vs. `$284.07` last-minute, saving **34.7%**), the **Tuesday (`$163.19`) vs. Sunday (`$250.79`)** departure gap, and **Economies of Distance** (`$0.395/mi` Short-Haul vs. `$0.110/mi` Long-Haul; Spearman $\rho = -0.929$).
- **Statistical Python & EDA:** Implemented Route-Contextual IQR outlier detection (`80,574` true surge outliers), validated findings via Welch's $t$-test ($t=245.34, p<0.0001$, Cohen's $d=1.077$) and One-Way ANOVA ($F=24,055.60, p<0.0001$), and discovered **ATPCO 21-day, 14-day, and 7-day Advance Purchase** tariff cliffs.
- **Power BI Executive Dashboard:** Built a Star Schema model with an 18-measure **DAX Library** and interactive executive reporting.
- **Machine Learning (Zero Data Leakage):** Engineered 22 pre-booking features and trained a hyperparameter-tuned **Gradient Boosting Regressor** using strict `itinerary_id` group isolation (`0` overlapping flights between Train and Test), achieving **$R^2 = 0.515$** and a **Median Absolute Error of `$34.70`** on unseen flight itineraries.

---

### 2. 🎮 [Steam SQL & Excel Analytics](https://github.com/Razi-mirzayev/steam-sql-excel-analytics)
> **Gaming Market, Pricing & Player Engagement Analysis using SQL, Python, and Excel**

- Comprehensive analytical pipeline exploring game pricing strategies, genre performance, release trends, and review sentiment across the Steam ecosystem using relational SQL queries, Python data processing, and interactive Excel dashboards.

---

### 3. 🔍 [Audit Analytics Toolkit](https://github.com/Razi-mirzayev/audit-analytics-toolkit)
> **Automated Data Auditing, Anomaly Detection & Risk Assessment in Python**

- Python-based analytical toolkit designed for internal audit workflows, data quality validation, outlier detection, and automated risk profiling on transactional datasets.

---

## 📊 Analytical Approach & Core Principles

1. **Data Integrity First:** Rigorous auditing of missing values, duplicate keys, and domain semantics before writing a single analytical query.
2. **Statistical Rigor:** Backing visual trends with formal hypothesis tests ($p$-values and effect sizes) and context-aware outlier detection.
3. **Strict Anti-Leakage ML:** Designing validation splits that mirror real-world production constraints (`GroupShuffleSplit` and out-of-fold encoding).
4. **Business-Driven Storytelling:** Translating technical outputs into concrete financial and operational recommendations.
