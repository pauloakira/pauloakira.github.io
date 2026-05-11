---
title: "Multi-Agent Data Scientist"
excerpt: "A desktop app for building visual, node-based LLM workflows for data analysis — drag-and-drop pipelines that stream live agent reasoning, hypothesis-to-plan recommenders, and dual DS / Senior-DS execution."
collection: portfolio
date: 2024-10-01
---

A desktop application for building and running AI-powered data analysis workflows.
The main screen is a node-based canvas where you wire together data sources,
context, and agents; runs stream live thoughts, tool calls, and observations into
an event log.

**Node types**

| Node | Purpose |
|------|---------|
| Connector         | Connects to a CSV folder or Athena warehouse |
| Context           | Injects markdown documentation into the agent's prompt |
| Metrics Extraction| Reads chart images / CSVs and extracts descriptions with a vision LLM |
| Recommender       | Converts product hypotheses into a structured analysis plan |
| DS Agent          | The data scientist — asks a question, reasons over data, streams thinking |

**Recommender agent.** Instead of asking a precise analytical question, you state
a product hypothesis. The Recommender profiles the connected tables (row counts,
date ranges, column stats, grain), detects experiment-assignment columns, estimates
sample sizes and statistical power, and emits a structured `AnalysisPlan` — typed
hypotheses, scored candidate analyses, agent assignment (DS vs. Senior DS),
execution order, and guardrails. The DS Agent then executes the plan and produces
a markdown report.

**Stack**

Tauri + React desktop front-end, FastAPI + SSE backend, Python multi-agent
orchestration. Plugs into OpenAI, Anthropic, and POE for model access; AWS Athena
and CSV warehouse connectors; DuckDB-backed warehouse tools; markdown retrieval
system for in-domain context.

**MLOps / engineering choices**

Auto-saving canvas with named workflow snapshots, JSON export/import, validation
banner that distinguishes errors (block run) from warnings (allow run), live
event-log streaming with one-shot cancellation, end-to-end pipelines from data
ingestion through model deployment and monitoring.
