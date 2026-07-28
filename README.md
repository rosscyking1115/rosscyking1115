# Cheng-Yuan (Ross) King

**Software engineer — AI evaluation and reliability** · MSc Artificial Intelligence, University of Sheffield

I build software that checks whether AI systems actually work: evaluation harnesses,
release gates, and tests that fail when a model or a metric has stopped measuring anything.

A test can pass because the system is right, or because the test cannot fail. I keep
finding the second case in my own work, and I write those up rather than quietly repairing them.

### Evaluation and safety

**[agent-release-gates](https://github.com/rosscyking1115/agent-release-gates)** — a Python
package built on AISI's [Inspect](https://github.com/UKGovernmentBEIS/inspect_ai) framework.
Replays past agent incidents and checks prompt, model and tool-policy changes before release.
Side-effecting tools require explicit approval; every decision leaves an audit trail.

**[redteam-foundry](https://github.com/rosscyking1115/redteam-foundry)** — asks whether the
benchmark behind a safety score still measures anything. Six metrics in this repo turned out
to be satisfied by the *absence* of the thing they measured. Three of them I introduced myself,
while fixing the previous one. All documented rather than quietly repaired.

**[cited-market-brief-agent](https://github.com/rosscyking1115/cited-market-brief-agent)** —
citation validation for LLM-generated briefs. Held-out precision 0.400, recall 1.000, zero
false negatives, measured once on a corpus authored after the rules were frozen.

### Data platforms

Warehouses in dbt, pipelines in Spark and DuckDB, APIs and dashboards on top.
[tfl-data-engineering](https://github.com/rosscyking1115/tfl-data-engineering) unifies 41.4M
journeys across five incompatible schema eras behind a reproducible evidence certificate.
[responsible-neobank-growth](https://github.com/rosscyking1115/responsible-neobank-growth)
proves each governance rule fires by making it fail.

---

Real open data where I have it, synthetic where I don't, and I say which. These are controlled
evaluations, not claims about production behaviour.

Available from October 2026 · [rosscyking.com](https://rosscyking.com) ·
[LinkedIn](https://linkedin.com/in/rosscyking) · rosscyking@gmail.com
