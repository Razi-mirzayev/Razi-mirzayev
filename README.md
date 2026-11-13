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

### 2. 🎮 [Steam Video Games Ecosystem – 3NF SQL, Statistical & Automated Excel BI Analytics](https://github.com/Razi-mirzayev/steam-sql-excel-analytics)
> **End-to-End 3NF Relational Database, SQL Window Analytics, SciPy Hypothesis Testing & OpenPyXL Automated BI across 22,608 Games**

- **3NF Relational Database (`steam_games.db`):** Built a Python ETL pipeline normalizing **22,608 Steam games** and **21,221 Wikidata records** into a 6-table **Third Normal Form (3NF)** SQLite database (`games`, `genres` [49], `game_genres` [64,146], `categories` [144], `game_categories` [134,841], `game_metadata` [21,221]).
- **Advanced SQL & Market Insights:** Executed multi-table `JOIN`, `CTE`, `LAG()`, and `RANK()` queries revealing that **Action (`$59.8B`)**, **Adventure (`$42.7B`)**, and **RPG (`$32.4B`)** lead gross revenue while **Indie (`12,821` paid titles)** dominates catalog volume; benchmarked top publishers (**Valve: `90.2%` positive**, **PlayStation Publishing: `84.8%`**, **Capcom: `83.0%`**) and game engines (**Essence Engine: `84.3` Metacritic**, **id Tech 3: `82.5`**).
- **Statistical Hypothesis Testing:** Validated pricing and sentiment dynamics across `17,773` established games via **Kruskal-Wallis ($H = 342.23, p < 0.0001$)** across price tiers (showing the `$10–$19.99` tier peaks at **84.31%** median approval vs. **78.40%** for `<$5` titles), **Spearman correlation ($\rho = +0.581$)** between Metacritic and player reviews, and **Mann-Whitney $U$ ($p < 0.0001$)** comparing Paid (**81.21%**) vs. Free-to-Play (**79.77%**) approval.
- **Automated Excel BI Workbook (`steam_games_dashboard.xlsx`):** Programmatically generated a 7-sheet executive Excel dashboard featuring live `INDEX/MATCH/MAX` KPI cards, conditional formatting, and embedded charts.

---

### 3. 🛡️ [Audit Analytics Toolkit (CAATs) – ISA-Aligned Financial Audit & Forensic ML](https://github.com/Razi-mirzayev/audit-analytics-toolkit)
> **Automated Financial Statement Auditing (ISA 240 / 520 / 530), Forensic ML Risk Scoring & P2P Three-Way Match in Python & SQLite**

- **ISA 240 Fraud Risk & Benford's Law:** Tested `1,223` General Ledger entries (`$4.89M` total value) via **Benford's Law First-Digit Analysis** ($\chi^2 = 17.623, p = 0.0242, \text{MAD} = 0.00883$), uncovering a **+1.80% excess spike in Leading Digit 9 (`6.38%` vs. `4.58%` expected)** driven by split-invoice structuring (`$9,700–$9,999`) below the `$10,000` approval limit.
- **Journal Entry Testing (JET) & Unsupervised Forensic ML:** Combined 6 deterministic red-flag rules (`341` weekend postings, `258` manager overrides, `17` period-end cutoffs, `13` near-limit splits) with a **Multivariate & Isolation-Projection Forensic ML Scorer** (`59.17` mean risk score on injected fraud seeds vs. `18.15` on normal entries).
- **ISA 530 Monetary Unit Sampling (MUS) & P2P Three-Way Match:** Demonstrated that **MUS (`55` sampled items)** audits **41.03% (`$2.01M`)** of total ledger value (**10x higher monetary coverage** than Simple Random Sampling at `4.12%`), and reconciled `150` Purchase Orders against Invoices and Payments, isolating **48 control exceptions (`32.0%`)**.
- **Automated Audit Deliverables:** Generates an **SQLite Audit Warehouse (`audit_warehouse.db`)**, a **7-sheet Excel Working Paper (`audit_findings_report.xlsx`)**, an executive **PDF Audit Memorandum (`audit_memo.pdf`)**, and an interactive **Streamlit Web App**.

---

## 📊 Analytical Approach & Core Principles

1. **Data Integrity First:** Rigorous auditing of missing values, duplicate keys, and domain semantics before writing a single analytical query.
2. **Statistical Rigor:** Backing visual trends with formal hypothesis tests ($p$-values and effect sizes) and context-aware outlier detection.
3. **Strict Anti-Leakage ML:** Designing validation splits that mirror real-world production constraints (`GroupShuffleSplit` and out-of-fold encoding).
4. **Business-Driven Storytelling:** Translating technical outputs into concrete financial and operational recommendations.
