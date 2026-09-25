# Utsa Poddar

**Data & AI Engineer.** I build LLM integrations, retrieval systems, and tooling for AI agents, with deterministic code that checks what a model returns before anything ships.

Proof you can inspect: a [scheduled LLM pipeline](https://github.com/utsapoddar/alpha-digest) that has published every Monday since I rebuilt its summarizer as a cross-provider fallback chain, and [agent memory](https://github.com/utsapoddar/engram) whose test suite fails if retrieval drops below recall@5 = 0.90.

Looking for **AI Engineer** roles, and AI-enabled data engineering: on-site or hybrid in Calgary, AB, or remote in Canada · **[utsapoddarjobs@gmail.com](mailto:utsapoddarjobs@gmail.com)** · [LinkedIn](https://www.linkedin.com/in/utsa-poddar) · [Portfolio](https://utsapoddar.github.io)

---

## Selected work

### [Alpha Digest](https://github.com/utsapoddar/alpha-digest): scheduled LLM pipeline over financial filings

Every Monday, GitHub Actions pulls SEC EDGAR Form 4 and 13F filings, corporate crypto-treasury data, commodity prices, and 12 RSS feeds. It joins them to a 25-entity watchlist, has an LLM summarize only that evidence into structured JSON, then emails the issue and publishes it to a public archive.

- **Reliability fix:** four weekly issues were missed in a row after a model was retired and long responses truncated the JSON. I pinned models across two providers (Gemini, then NVIDIA NIM), split transient errors (retry) from permanent ones (fall through), and sized the job timeout to the real retry path. Every scheduled run since has succeeded: [run history](https://github.com/utsapoddar/alpha-digest/actions/workflows/weekly-digest.yml).
- [Latest issue](https://utsapoddar.github.io/alpha-digest) · [Design walkthrough](https://github.com/utsapoddar/alpha-digest/blob/main/docs/design-walkthrough.md)

### [Engram](https://github.com/utsapoddar/engram): auditable memory and retrieval for AI coding agents

Markdown notes under a typed truth model are the source of record. A SQLite FTS5 index ranks them with BM25, optionally fused with local embeddings by reciprocal-rank fusion, and can be rebuilt from the notes at any time. Corrections go through a crash-recoverable journal, and every write rejects credentials. An installer wires it into Claude Code and Codex.

- **Evaluation:** 71 tests, including a 20-query retrieval evaluation that fails the suite below recall@5 = 0.90.

### [DopaKernel](https://github.com/utsapoddar/dopa-kernel): completion control for AI agents

Freezes a task into explicit requirements, picks the next action from recorded progress, and won't report "done" until every requirement passes a fresh run of its verifier, rather than the model's own account. Runs as Claude Code hooks.

- **Proof:** the current kernel passes 90 unit tests and 54 structural checks, and a replay harness asserts that protocol changes don't alter the controller's decisions.

## More projects

| Project | What it shows |
|---|---|
| [Leafmark](https://github.com/utsapoddar/leafmark) · [live](https://utsapoddar.github.io/leafmark/) | In-browser PDF/EPUB reading guides. A local extractive engine cites a page or section for every item. An optional provider layer connects your own model through Gemini or any OpenAI-compatible API, retries transient failures, repairs and validates structured output, and checkpoints each chunk so a model switch resumes instead of restarting. Next.js + TypeScript, 31 tests. |
| [PCOS Food Scanner](https://github.com/utsapoddar/pcos-scanner) | Prototype. Barcode, label photo, or meal photo → deterministic nutrient score; the LLM reads photos and personalizes the explanation but never sets the base score. Streamlit + Supabase, 30 tests. |
| [MSDS Time Estimator](https://github.com/utsapoddar/msds-time-estimator) | Bayesian estimates, with 80% intervals, of how long a CU Boulder MSDS course will take you, anchored on courses you've finished. |
| [Fraud detection](https://github.com/utsapoddar/Fintech-Project) | Class-weighted Random Forest on 284,807 transactions: 96% precision and 74% recall on the fraud class, plus a note on what those numbers don't show. |

## Background

- **Data & AI Engineer (independent)**, Sep 2025 – present
- **Online Department Supervisor**, Canadian Tire, 2024 – 2025: supervised 11 associates; raised order fulfilment from 90% to 98%
- **Business Intelligence Analyst**, Next Generation Graphics Ltd (remote, Singapore), 2022 – 2023: SQL extraction and KPI reporting, presented to non-technical teams across time zones
- **MS Data Science**, including the Artificial Intelligence graduate certificate, University of Colorado Boulder (both in progress) · **BSc Physics**, University of Calgary (2022)

**Tools:** Python · TypeScript · SQL · LLM APIs (Gemini, NVIDIA NIM, OpenAI-compatible) · structured output validation · retrieval (BM25, embeddings, RRF) · retrieval evaluation · SQLite FTS5 · Supabase · Streamlit · Next.js · GitHub Actions · pandas · NumPy · scikit-learn
