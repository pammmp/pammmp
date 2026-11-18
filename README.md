# Hi, I'm Pamela 👋

I work with **data, integrations and applied AI**, backed by 15 years in supply chain and
manufacturing: from ELT pipelines on AWS and BigQuery to full-stack web apps integrated with
ERP systems, with security designed in from the database up.

📫 [LinkedIn](https://www.linkedin.com/in/pamelamendesp) · [pamelamendespereira@gmail.com](mailto:pamelamendespereira@gmail.com)

---


## 🛠️ Stack

| Area | Tools |
|---|---|
| **Languages** | Python, SQL, TypeScript |
| **Data** | BigQuery, PostgreSQL, DuckDB, MySQL, Oracle, **dbt**, ELT, data testing and data quality, pandas, NumPy, Plotly |
| **Cloud** | AWS (Lambda, EventBridge, CloudWatch), Google Cloud (Cloud Functions, Cloud Run, Vertex AI) |
| **Full-stack** | React 19, TanStack Start, Tailwind CSS, Bun (40 automated tests) |
| **Machine Learning** | Transaction fraud detection, demand forecasting (walk-forward validation), cosine-similarity recommender system |
| **AI** | Google ADK, Gemini, multi-agent systems, LLM response evaluation |
| **Integrations** | Omie API (ERP), webhooks, polling, REST, OAuth2, Google Sheets, Microsoft Graph |
| **Security** | PostgreSQL RLS, MFA (TOTP) and access roles, HTTP security headers (CSP, HSTS), Secret Manager, LGPD |
| **Full-stack** | React 19, TanStack Start, Tailwind CSS, Bun (tests) |
| **BI** | Looker Studio, Power BI |
| **Management** | ServiceNow (workflows), Jira, Kanban, GitHub Projects |

---

## 🧰 Platforms and systems I've worked with

- **Cloud:** AWS (Lambda, API Gateway, RDS), Google Cloud
- **Systems (ERP and processes):** Omie, SAP Ariba, Microsoft Dynamics NAV (Navision), Senior, ServiceNow, SoftExpert, Argo, Logcomex
- **Databases:** PostgreSQL, MySQL, Oracle, BigQuery
- **Other:** GitHub Actions, Power Query

---

## 📂 Featured projects

### [supplier-performance-dbt](https://github.com/pammmp/supplier-performance-dbt)

One trusted definition of supplier OTIF. dbt + DuckDB project with staging, intermediate and
mart layers, 25 data tests, an SCD2 snapshot, an A/B analysis of supplier onboarding and CI
that publishes the docs to GitHub Pages. [Live docs](https://pammmp.github.io/supplier-performance-dbt/)

### Omie → BigQuery pipeline · private client code

Event-driven ELT on AWS. A Lambda receives Omie webhooks, answers within the 7-second limit
and triggers an async sync of 9 ERP endpoints into BigQuery. EventBridge runs the same sync
every 4 hours as a safety net. Each record gets a SHA-256 hash, so only changed records are
written, building an append-only change history. Failures are isolated per endpoint and logged.

### [Negócio do Bem](https://github.com/fabsreis/Negocio-do-bem)

Volunteer project with 50+ developers, plus designers and UX. I'm the **PM (Product & Project)**: I run project management on my own and work on product with the project's owner. I keep the pull request and issue flow organized:

- **GitHub Projects board** with Status and Next action fields, including a QA status for reviewed PRs waiting to be tested before merge.
- **CI tracking through to merge:** lint, type checks, tests, CodeQL and dependency audit.
- **Priority and label rules**, with each issue mirroring the status of its linked PR.
- **AI-assisted triage:** a skill reads each PR's history and proposes status changes, always subject to my approval.
- **Product and growth:** I support the project's product and growth strategy.

### [elt-bigquery-data-quality](https://github.com/pammmp/elt-bigquery-data-quality)

ELT pipeline on BigQuery with data quality tests and CI.

### [Aureon website](https://aureonconsulting.com.br/) · private code

Bilingual (PT/EN) website with SSR and an admin panel.

---

## 🔌 Integrations

- **Two systems integrated with the Omie ERP:** I built a web app for a client with two-way sync between the app and their ERP, so a change on one side shows up on the other. It combines webhooks through AWS Lambda, direct calls to the v1 API and polling, with consistency checks. It covers production orders, items, bills of materials and stage progress, as well as accounts payable and receivable and customers.
- **API throttling protection:** an internal layer with a shared cache and rate limiting on calls to Omie.
- **Data for BI:** token-authenticated export to BigQuery, feeding reports and dashboards in Looker Studio and Google Sheets.
- **System-to-system authentication:** OAuth2 (Google and Microsoft Graph), with credentials stored in Secret Manager.
- **Data pipeline (AWS):** Omie webhooks plus a 4-hour schedule feed BigQuery through Python Lambdas.
- **Production web app:** two-way sync. It reads production orders on demand and sends stages
  and completions back to the ERP, with per-field ownership rules and concurrency control.
---

## 🔐 Security

- **Database:** Row-Level Security enabled on every table.
- **Access:** operator, planning and admin roles, with mandatory TOTP MFA for admin accounts; Google OAuth login on the website's admin panel.
- **Integrity and authenticity:** SHA-256 hashing to detect changed records, a unique ERP key with upserts in the web app, a lock against parallel syncs, and a token on the data export endpoint.
- **Web:** strict Content-Security-Policy, HSTS, X-Frame-Options, Permissions-Policy and COOP on every response; `security.txt` published.
- **Privacy:** LGPD consent banner, with Google Analytics loaded only after the visitor accepts.

---

## 🌐 Programs and communities

- **Google Developers**
- **Microsoft Student Ambassadors**
- **GitHub Developers**
- **Google Cloud Skills Boost:** multi-agent system challenge lab with ADK, A2A and Cloud Run.
- **Copilot Pioneers:** ambassador for a corporate AI program.
- **AI Data Trainer:** LLM response evaluation and prompt refinement on international projects.
- **Postgraduate degree in AI and Leadership:** Conquer Business School.

---

## 🎓 Education

- **Data Science (associate degree, in progress):** UNINTER
- **Bachelor in Business Administration:** Universidade Positivo (2006–2009)

---

## 📊 GitHub stats

![GitHub stats](./profile/stats.svg)
