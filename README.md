<!--
  DRAFT profile README — paste into the PUBLIC repo `rosscyking1115`
  (github.com/rosscyking1115/rosscyking1115) as README.md.
  Rewritten 2026-07-12 for the consolidated portfolio: new slugs
  (uk-housing-decision-support, community-energy-flex), marketing-lab absorbed/archived
  (dropped), aerospace strengthened, DE-primary ordering. All facts drawn from the public
  repos. Supersedes ecosystem-map.md §1.
-->

# Cheng-Yuan (Ross) King

**Data & ML Engineering · AI Safety & Evaluation** — MSc AI @ University of Sheffield 🇬🇧

I build data and ML systems whose decisions are **auditable** — tested pipelines, honest
evaluation, and evidence you can trace. From Spark-scale data engineering to release-gates
for AI agents, the throughline is the same: verifiable over impressive.

🔗 [rosscyking.com](https://rosscyking.com) · 💼 [linkedin.com/in/rosscyking](https://www.linkedin.com/in/rosscyking) · ✉️ rosscyking@gmail.com

---

### 🛠️ Data & ML Engineering

| Project | What it is |
|---|---|
| **[tfl-data-engineering](https://github.com/rosscyking1115/tfl-data-engineering)** | Living workflow quantifying how London transport disruption shifts cycle-hire demand — a **41.4M-journey** PySpark backfill → dbt → DuckDB/Parquet, a LightGBM forecast, and an MCP server, run daily on GitHub Actions with no warehouse to keep alive. → **[Live demo](https://tfl-data-engineering.streamlit.app/)** |
| **[uk-housing-decision-support](https://github.com/rosscyking1115/uk-housing-decision-support)** | Explainable UK where-to-live decision-support — the **MoveIn** web app over 7 official open-data sources → 5 transparent indicators across **7,264** neighbourhoods. Tested dbt + DuckDB engine (197 dbt tests), Dagster orchestration, public API + site. → **[MoveIn live site](https://uk-housing-decision-support.vercel.app)** · [API docs](https://uk-housing-decision-support-api.fly.dev/docs) |
| **[community-energy-flex](https://github.com/rosscyking1115/community-energy-flex)** | When to run flexible electricity loads to cut cost and carbon, from live UK grid data — the **After Midnight** web app, with an LP/MILP optimiser, a typed end-to-end contract, and a forecast-vs-actual retro that checks whether yesterday's plan actually saved. dbt/Snowflake + Power BI. → **[After Midnight app](https://after-midnight-beta.vercel.app/)** · [API docs](https://community-energy-flex-api.fly.dev/docs) |
| **[aerospace-prognostics](https://github.com/rosscyking1115/aerospace-prognostics)** | Deployable, end-to-end PHM MLOps — NASA C-MAPSS RUL + spacecraft anomaly detection wrapped in a production-envelope serving API, signed release evidence (model card, SBOM, provenance), and **453 tests**. Evaluation layer extracted as the standalone **[telemeval](https://github.com/rosscyking1115/telemeval)** library (PyPI + Zenodo DOI). |

### 🛡️ AI Safety & Evaluation

| Project | What it is |
|---|---|
| **[agent-release-gates](https://github.com/rosscyking1115/agent-release-gates)** | Release-readiness gates for AI agents — replay incidents, policy-as-code, produce `ship`/`warn`/`block` evidence before an agent, prompt, model, or tool-policy change ships. Runs under Inspect (UK AISI). → **[Live dashboard](https://agent-release-gates.streamlit.app/)** · [PyPI](https://pypi.org/project/agent-release-gates/) |
| **[redteam-foundry](https://github.com/rosscyking1115/redteam-foundry)** | LLM red-team evaluation harness — prompt-injection, refusal, leakage and staleness testing with attack-corpus audits and judge-validated, reproducible reports. The upstream that feeds agent-release-gates. → **[PyPI](https://pypi.org/project/redteam-foundry/)** |
| **[cited-market-brief-agent](https://github.com/rosscyking1115/cited-market-brief-agent)** | Audit-ready market-brief engine — every claim validated against a stored source span before it ships, enforced by a CI eval gate. Next.js + FastAPI + pgvector. → **[Live demo](https://cited-market-brief-agent.vercel.app)** |

### 🏦 Applied Fintech & Decision-Support

| Project | What it is |
|---|---|
| **[responsible-neobank-growth](https://github.com/rosscyking1115/responsible-neobank-growth)** | Synthetic fintech decision-support where customer-outcome guardrails dominate commercial uplift — release-gate verdicts, fairness gaps, experimentation (CUPED, DiD, synthetic control). dbt · DuckDB/BigQuery · Streamlit. → **[Live dashboard](https://neobank-appuct-analytics.streamlit.app/)** |
| **[cashflow-risk](https://github.com/rosscyking1115/cashflow-risk)** | Which unpaid UK-SME invoices threaten cash runway, when, and the week's action — leakage-safe risk scoring behind a STRIDE threat model, DPIA, and tested multi-tenant RBAC. FastAPI · Postgres · Next.js. → **[Live demo](https://cashflow-web-sidu.onrender.com/)** |

---

### 🧰 Tech
`Python` · `FastAPI` · `PySpark` · `dbt` · `DuckDB` · `Snowflake` · `Dagster` · `Streamlit` · `scikit-learn` · `LightGBM` · `MLflow` · `TypeScript` · `Next.js` · `Docker` · `GitHub Actions` · `PyPI`

<sub>Focus: making model and data decisions verifiable — evidence, evaluation, and honest guardrails over raw capability.</sub>
