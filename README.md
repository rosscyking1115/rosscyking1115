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
| **[tfl-data-engineering](https://github.com/rosscyking1115/tfl-data-engineering)** · [demo](https://tfl-data-engineering.streamlit.app/) | Living workflow quantifying how London transport disruption shifts cycle-hire demand — a **41.4M-journey** PySpark backfill → dbt → DuckDB/Parquet, a LightGBM forecast, and an MCP server, run daily on GitHub Actions with no warehouse to keep alive. |
| **[uk-housing-decision-support](https://github.com/rosscyking1115/uk-housing-decision-support)** *(web app: MoveIn)* | Explainable UK where-to-live decision-support — 7 official open-data sources → 5 transparent indicators across **7,264** neighbourhoods. Tested dbt + DuckDB engine (197 dbt tests), Dagster orchestration, public API + site. |
| **[community-energy-flex](https://github.com/rosscyking1115/community-energy-flex)** *(web app: After Midnight)* · [demo](https://after-midnight-beta.vercel.app/) | When to run flexible electricity loads to cut cost and carbon, from live UK grid data — an LP/MILP optimiser, a typed end-to-end contract, and a forecast-vs-actual retro that checks whether yesterday's plan actually saved. dbt/Snowflake + Power BI. |
| **[aerospace-prognostics](https://github.com/rosscyking1115/aerospace-prognostics)** | Deployable, end-to-end PHM MLOps — NASA C-MAPSS RUL + spacecraft anomaly detection wrapped in a production-envelope serving API, signed release evidence (model card, SBOM, provenance), and **453 tests**. Its evaluation layer is the standalone **[telemeval](https://github.com/rosscyking1115/telemeval)** library (PyPI + Zenodo DOI). |

### 🛡️ AI Safety & Evaluation

| Project | What it is |
|---|---|
| **[agent-release-gates](https://github.com/rosscyking1115/agent-release-gates)** · [PyPI](https://pypi.org/project/agent-release-gates/) | Release-readiness gates for AI agents — replay incidents, policy-as-code, produce `ship`/`warn`/`block` evidence before an agent, prompt, model, or tool-policy change ships. Runs under Inspect (UK AISI). |
| **[redteam-foundry](https://github.com/rosscyking1115/redteam-foundry)** · [PyPI](https://pypi.org/project/redteam-foundry/) | LLM red-team evaluation harness — prompt-injection, refusal, leakage and staleness testing with attack-corpus audits and judge-validated, reproducible reports. The upstream that feeds agent-release-gates. |
| **[cited-market-brief-agent](https://github.com/rosscyking1115/cited-market-brief-agent)** · [demo](https://cited-market-brief-agent.vercel.app) | Audit-ready market-brief engine — every claim validated against a stored source span before it ships, enforced by a CI eval gate. Next.js + FastAPI + pgvector. |

### 🏦 Applied Fintech & Decision-Support

| Project | What it is |
|---|---|
| **[responsible-neobank-growth](https://github.com/rosscyking1115/responsible-neobank-growth)** | Synthetic fintech decision-support where customer-outcome guardrails dominate commercial uplift — release-gate verdicts, fairness gaps, experimentation (CUPED, DiD, synthetic control). dbt · DuckDB/BigQuery · Streamlit. |
| **[cashflow-risk](https://github.com/rosscyking1115/cashflow-risk)** · [demo](https://cashflow-web-sidu.onrender.com/) | Which unpaid UK-SME invoices threaten cash runway, when, and the week's action — leakage-safe risk scoring behind a STRIDE threat model, DPIA, and tested multi-tenant RBAC. FastAPI · Postgres · Next.js. |

---

### 🧰 Tech
`Python` · `FastAPI` · `PySpark` · `dbt` · `DuckDB` · `Snowflake` · `Dagster` · `Streamlit` · `scikit-learn` · `LightGBM` · `MLflow` · `TypeScript` · `Next.js` · `Docker` · `GitHub Actions` · `PyPI`

<sub>Focus: making model and data decisions verifiable — evidence, evaluation, and honest guardrails over raw capability.</sub>
