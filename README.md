# Cheng-Yuan (Ross) King

**Data & ML Engineering · AI Safety & Evaluation** — MSc AI @ University of Sheffield 🇬🇧

I build data and ML systems whose decisions you can audit: tested pipelines, honest evaluation,
and numbers you can trace back to the test that produced them. Spark-scale data engineering,
open-data warehouses, ML forecasts, and release-gates for AI agents.

🔗 [rosscyking.com](https://rosscyking.com) · 💼 [linkedin.com/in/rosscyking](https://www.linkedin.com/in/rosscyking) · ✉️ rosscyking@gmail.com

---

### 🛠️ Data & ML Engineering

| Project | What it is |
|---|---|
| **[tfl-data-engineering](https://github.com/rosscyking1115/tfl-data-engineering)** | Quantifies how London transport disruption shifts cycle-hire demand: a **41.4M-journey** PySpark backfill → dbt → DuckDB/Parquet, a LightGBM forecast, and an MCP server, run daily on GitHub Actions with no warehouse to keep alive. Strike days run 1.2–2.6× normal demand against a weather-adjusted baseline. → **[Live demo](https://tfl-data-engineering.streamlit.app/)** |
| **[england-wales-housing-decision-support](https://github.com/rosscyking1115/england-wales-housing-decision-support)** | Explainable where-to-live decision support over nine official open-data sources → five 0–100 indicators across **7,264** neighbourhoods, each score shown beside the figure it came from. Tested dbt + DuckDB engine (**222 dbt tests**), Dagster orchestration, a public API and a Next.js site. → **[Live site](https://uk-housing-decision-support.vercel.app)** · [API docs](https://uk-housing-decision-support-api.fly.dev/docs) |
| **[community-energy-flex](https://github.com/rosscyking1115/community-energy-flex)** | Works out when to run flexible electricity loads to cut cost and carbon, from live UK grid data — the **After Midnight** web app, with an LP/MILP optimiser, a typed end-to-end contract, and a forecast-vs-actual retro that checks whether yesterday's plan actually saved. dbt/Snowflake + Power BI. → **[After Midnight app](https://after-midnight-beta.vercel.app/)** · [API docs](https://community-energy-flex-api.fly.dev/docs) |
| **[aerospace-prognostics](https://github.com/rosscyking1115/aerospace-prognostics)** | End-to-end PHM MLOps: NASA C-MAPSS RUL and ESA spacecraft anomaly detection carried through their real protocols, wrapped in a serving API, signed release evidence (model card, SBOM, provenance), and **453 tests**. The evaluation layer is extracted as **[telemeval](https://github.com/rosscyking1115/telemeval)** (PyPI + Zenodo DOI). |

### 🛡️ AI Safety & Evaluation

| Project | What it is |
|---|---|
| **[agent-release-gates](https://github.com/rosscyking1115/agent-release-gates)** | Release-readiness gates for AI agents: replay incidents, apply policy-as-code, produce `ship`/`warn`/`block` evidence before an agent, prompt, model, or tool-policy change ships. Runs under Inspect (UK AISI). → **[Live dashboard](https://agent-release-gates.streamlit.app/)** · [PyPI](https://pypi.org/project/agent-release-gates/) |
| **[redteam-foundry](https://github.com/rosscyking1115/redteam-foundry)** | LLM red-team evaluation harness: prompt-injection, refusal, leakage and staleness tests with attack-corpus audits and cross-judge-validated, reproducible reports. The upstream that feeds agent-release-gates. → **[PyPI](https://pypi.org/project/redteam-foundry/)** |
| **[cited-market-brief-agent](https://github.com/rosscyking1115/cited-market-brief-agent)** | Audit-ready market-brief engine: every claim validated against a stored source span before it ships, enforced by a CI eval gate. Next.js + FastAPI + pgvector. → **[Live demo](https://cited-market-brief-agent.vercel.app)** |

### 🏦 Applied Fintech & Decision-Support

| Project | What it is |
|---|---|
| **[responsible-neobank-growth](https://github.com/rosscyking1115/responsible-neobank-growth)** | Synthetic fintech decision-support where customer-outcome guardrails drive the commercial call: release-gate verdicts, fairness gaps, and experimentation (CUPED, DiD, synthetic control). dbt · DuckDB/BigQuery · Streamlit. → **[Live dashboard](https://neobank-appuct-analytics.streamlit.app/)** |
| **[cashflow-risk](https://github.com/rosscyking1115/cashflow-risk)** | Which unpaid UK-SME invoices threaten cash runway, when, and the week's action — leakage-safe risk scoring behind a STRIDE threat model, a DPIA, and tested multi-tenant RBAC. FastAPI · Postgres · Next.js. → **[Live demo](https://cashflow-web-sidu.onrender.com/)** |

---

### 🧰 Tech
`Python` · `FastAPI` · `PySpark` · `dbt` · `DuckDB` · `Snowflake` · `Dagster` · `Streamlit` · `scikit-learn` · `LightGBM` · `MLflow` · `TypeScript` · `Next.js` · `Docker` · `GitHub Actions` · `PyPI`

<sub>What I care about: evidence, honest evaluation, and guardrails you can check — over raw capability.</sub>
