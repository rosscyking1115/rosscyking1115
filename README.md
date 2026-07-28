<h1 align="center">Cheng-Yuan (Ross) King</h1>

<p align="center">
  <b>AI Evaluation &amp; Reliability</b> &nbsp;·&nbsp; Data &amp; ML Engineering<br>
  <sub>MSc Artificial Intelligence · University of Sheffield 🇬🇧 · Available full time from October 2026</sub>
</p>

<p align="center">
  <a href="https://rosscyking.com"><img src="https://img.shields.io/badge/Portfolio-rosscyking.com-111827?style=flat-square&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/rosscyking"><img src="https://img.shields.io/badge/LinkedIn-rosscyking-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:rosscyking@gmail.com"><img src="https://img.shields.io/badge/Email-rosscyking%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/PyPI_packages-3-3775A9?style=flat-square&logo=pypi&logoColor=white" alt="3 PyPI packages">
</p>

---

I build software that checks whether AI systems actually work: evaluation harnesses, release
gates, and numbers you can trace back to the test that produced them. Three of these ship as
installable packages on PyPI; most run as live services you can open right now.

> **A test can pass because the system is right, or because the test cannot fail.**
> I keep finding the second case in my own work, and I publish those rather than quietly
> repairing them.

---

## 🛡️ AI Evaluation &amp; Reliability

### [agent-release-gates](https://github.com/rosscyking1115/agent-release-gates)

[![PyPI](https://img.shields.io/pypi/v/agent-release-gates?style=flat-square&logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/agent-release-gates/)
[![CI](https://img.shields.io/github/actions/workflow/status/rosscyking1115/agent-release-gates/ci.yml?style=flat-square&label=CI)](https://github.com/rosscyking1115/agent-release-gates/actions/workflows/ci.yml)
[![Live dashboard](https://img.shields.io/badge/dashboard-live-2ea44f?style=flat-square)](https://agent-release-gates.streamlit.app/)
[![Inspect](https://img.shields.io/badge/runs_under-Inspect_(UK_AISI)-6f42c1?style=flat-square)](https://github.com/UKGovernmentBEIS/inspect_ai)

Release-readiness gates for AI agents: replay incidents, apply policy-as-code, and produce
`ship` / `warn` / `block` evidence before an agent, prompt, model or tool-policy change ships.
Side-effecting tools require explicit approval, and every verdict leaves an audit trail.

### [redteam-foundry](https://github.com/rosscyking1115/redteam-foundry)

[![PyPI](https://img.shields.io/pypi/v/redteam-foundry?style=flat-square&logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/redteam-foundry/)
[![Upstream](https://img.shields.io/badge/feeds-agent--release--gates-6f42c1?style=flat-square)](https://github.com/rosscyking1115/agent-release-gates)

LLM red-team evaluation harness: prompt-injection, refusal, leakage and staleness tests with
attack-corpus audits and cross-judge validation. **Six metrics in this repo turned out to be
satisfied by the absence of the thing they measured — three of them introduced while fixing
the previous one.** All documented rather than quietly repaired.

### [cited-market-brief-agent](https://github.com/rosscyking1115/cited-market-brief-agent)

[![CI](https://img.shields.io/github/actions/workflow/status/rosscyking1115/cited-market-brief-agent/ci.yml?style=flat-square&label=CI)](https://github.com/rosscyking1115/cited-market-brief-agent/actions/workflows/ci.yml)
[![Live demo](https://img.shields.io/badge/demo-live-2ea44f?style=flat-square)](https://cited-market-brief-agent.vercel.app)

Audit-ready market-brief engine: every claim validated against a stored source span before it
ships, enforced by a CI eval gate. Held-out **precision 0.400, recall 1.000, zero false
negatives** — measured once on a corpus authored after the rules were frozen. Next.js ·
FastAPI · pgvector.

---

## 🛠️ Data &amp; ML Engineering

| Project | What it is | Live |
|---|---|---|
| **[tfl-data-engineering](https://github.com/rosscyking1115/tfl-data-engineering)** <br> [![CI](https://img.shields.io/github/actions/workflow/status/rosscyking1115/tfl-data-engineering/ci.yml?style=flat-square&label=CI)](https://github.com/rosscyking1115/tfl-data-engineering/actions/workflows/ci.yml) | Quantifies how London transport disruption shifts cycle-hire demand: a **41.4M-journey** PySpark backfill → dbt → DuckDB/Parquet, a LightGBM forecast, and an MCP server, run daily on GitHub Actions with no warehouse to keep alive. Strike days run **~1.4× median demand (95% CI 1.2–1.6), up to ~2.3×** on the worst full-network strike day, against a weather-adjusted baseline. | [![demo](https://img.shields.io/badge/demo-live-2ea44f?style=flat-square)](https://tfl-data-engineering.streamlit.app/) |
| **[england-wales-housing-decision-support](https://github.com/rosscyking1115/england-wales-housing-decision-support)** <br> [![CI](https://img.shields.io/github/actions/workflow/status/rosscyking1115/england-wales-housing-decision-support/ci.yml?style=flat-square&label=CI)](https://github.com/rosscyking1115/england-wales-housing-decision-support/actions/workflows/ci.yml) | Explainable where-to-live decision support over nine official open-data sources → five 0–100 indicators across **7,264** neighbourhoods, each score shown beside the figure it came from. Tested dbt + DuckDB engine (**222 dbt tests**), Dagster orchestration, a public API and a Next.js site. | [![site](https://img.shields.io/badge/site-live-2ea44f?style=flat-square)](https://uk-housing-decision-support.vercel.app) [![API](https://img.shields.io/badge/API-docs-0b7285?style=flat-square)](https://uk-housing-decision-support-api.fly.dev/docs) |
| **[community-energy-flex](https://github.com/rosscyking1115/community-energy-flex)** <br> [![CI](https://img.shields.io/github/actions/workflow/status/rosscyking1115/community-energy-flex/ci.yml?style=flat-square&label=CI)](https://github.com/rosscyking1115/community-energy-flex/actions/workflows/ci.yml) | Works out when to run flexible electricity loads to cut cost and carbon, from live UK grid data — the web app, with an LP/MILP optimiser, a typed end-to-end contract, and a forecast-vs-actual retro that checks whether yesterday's plan actually saved. dbt/Snowflake + Power BI. | [![app](https://img.shields.io/badge/app-live-2ea44f?style=flat-square)](https://after-midnight-beta.vercel.app/) [![API](https://img.shields.io/badge/API-docs-0b7285?style=flat-square)](https://community-energy-flex-api.fly.dev/docs) |
| **[aerospace-prognostics](https://github.com/rosscyking1115/aerospace-prognostics)** <br> [![CI](https://img.shields.io/github/actions/workflow/status/rosscyking1115/aerospace-prognostics/ci.yml?style=flat-square&label=CI)](https://github.com/rosscyking1115/aerospace-prognostics/actions/workflows/ci.yml) | End-to-end PHM MLOps: NASA C-MAPSS RUL and ESA spacecraft anomaly detection carried through their real protocols, wrapped in a serving API, signed release evidence (model card, SBOM, provenance), and **461 tests**. The evaluation layer is extracted as **[telemeval](https://github.com/rosscyking1115/telemeval)**. | [![PyPI](https://img.shields.io/pypi/v/telemeval?style=flat-square&logo=pypi&logoColor=white&label=telemeval)](https://pypi.org/project/telemeval/) |

---

## 🏦 Applied Fintech &amp; Decision-Support

| Project | What it is | Live |
|---|---|---|
| **[responsible-neobank-growth](https://github.com/rosscyking1115/responsible-neobank-growth)** | Synthetic fintech decision-support where customer-outcome guardrails drive the commercial call: release-gate verdicts, fairness gaps, and experimentation (CUPED, DiD, synthetic control). Every governance rule is proved to fire by an invalid fixture that makes it fail. dbt · DuckDB/BigQuery · Streamlit. | [![dashboard](https://img.shields.io/badge/dashboard-live-2ea44f?style=flat-square)](https://responsible-neobank-growth.streamlit.app/) |
| **[cashflow-risk](https://github.com/rosscyking1115/cashflow-risk)** <br> [![CI](https://img.shields.io/github/actions/workflow/status/rosscyking1115/cashflow-risk/ci.yml?style=flat-square&label=CI)](https://github.com/rosscyking1115/cashflow-risk/actions/workflows/ci.yml) | Which unpaid UK-SME invoices threaten cash runway, when, and the week's action — leakage-safe risk scoring behind a STRIDE threat model, a DPIA, and tested multi-tenant RBAC. FastAPI · Postgres · Next.js. | [![demo](https://img.shields.io/badge/demo-live-2ea44f?style=flat-square)](https://cashflow-web-sidu.onrender.com/) |

---

## 🧰 Tech

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat-square&logo=snowflake&logoColor=white)
![Dagster](https://img.shields.io/badge/Dagster-4F43DD?style=flat-square&logo=dagster&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)

---

<p align="center">
  <sub>Real open data where I have it, synthetic where I don't — and I say which.<br>
  What I care about: evidence, honest evaluation, and guardrails you can check — over raw capability.</sub>
</p>
