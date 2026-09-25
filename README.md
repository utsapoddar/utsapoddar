# Utsa Poddar

**Applied ML & AI engineer.** Physics-trained. I build LLM-powered systems and data pipelines where the model's output is advisory and a deterministic, tested component stays authoritative — so when something goes wrong, you can see why.

Calgary, AB · Open to ML engineering, AI engineering, and data science roles · **[utsapoddarjobs@gmail.com](mailto:utsapoddarjobs@gmail.com)** · **[LinkedIn](https://www.linkedin.com/in/utsa-poddar)** · **[Portfolio](https://utsapoddar.github.io)**

---

## Featured work

**[Engram](https://github.com/utsapoddar/engram)** · Python, SQLite FTS5
Long-term memory for AI coding agents. Notes live as reviewable Markdown under a typed schema; the search index is disposable and rebuilt from them. Corrections are journaled so a crash mid-write can't corrupt the store, and credentials are rejected on every write.
→ 71 tests. Retrieval is gated on recall@5 ≥ 90% across a 20-query eval set, so ranking quality is measured, not assumed.

**[Alpha Digest](https://github.com/utsapoddar/alpha-digest)** · Python, GitHub Actions
A weekly investor briefing that runs unattended. It pulls SEC EDGAR Form 4 and 13F filings, crypto-treasury data, commodity prices, and news, joins them to a 25-entity watchlist, and has an LLM summarize only that evidence into structured JSON. A Gemini → NVIDIA fallback chain keeps one failing provider from breaking the run.
→ Ships every Monday via cron to email subscribers and a public archive. **[Read the latest issue](https://utsapoddar.github.io/alpha-digest)**

**[MSDS Time Estimator](https://github.com/utsapoddar/msds-time-estimator)** · Python, Bayesian modeling
Predicts how many hours a CU Boulder MSDS course will take *you*, anchored on the courses you've already finished. Course posteriors update from crowdsourced reviews under a tempered likelihood, so heavily reviewed courses tighten without drowning your personal prior. Output is an 80% interval, not a point guess.
→ Full derivation in [MODEL.md](https://github.com/utsapoddar/msds-time-estimator/blob/main/MODEL.md).

**[Leafmark](https://github.com/utsapoddar/leafmark)** · TypeScript, Next.js
Private book summaries that run in your browser. PDF and EPUB parsing and a baseline extractive summarizer run on-device, and every summary item cites its source page or EPUB section. Readers can optionally plug in their own model (free, paid, or self-hosted) for richer summaries. No app database, and no API key ships with the site.
→ 31 tests. **[Try it](https://utsapoddar.github.io/leafmark/)**

## Also built

| Project | What it shows |
|---|---|
| [PCOS Food Scanner](https://github.com/utsapoddar/pcos-scanner) | Barcode/photo → nutrient score. Scoring is rule-based and tested; the LLM only explains it. Streamlit + Supabase. |
| [DopaKernel](https://github.com/utsapoddar/dopa-kernel) | Stops coding agents from declaring "done" early: completion requires re-run verifier evidence, not the model's own claim. 225 tests. |
| [Cadence](https://github.com/utsapoddar/cadence) | Browser sound therapy via Web Audio, limited to frequencies with peer-reviewed support; JS output checked against a NumPy/SciPy reference. **[Try it](https://utsapoddar.github.io/cadence/)** |
| [Sift Work Timer](https://github.com/utsapoddar/sift-work-timer) | Cross-platform Flutter app (iOS, Android, macOS, Windows), distributed via Google Play and AltStore. |
| [Fraud detection](https://github.com/utsapoddar/Fintech-Project) | Credit-card fraud detection: transaction data exploration and a modeling pipeline. |
| [Physics simulations](https://github.com/utsapoddar/physics-python-projects) · [Fluid dynamics](https://github.com/utsapoddar/fluid_dynamics) | Numerical methods from my physics training, in Python and MATLAB. |

## Stack

**Core:** Python · SQL · TypeScript/JavaScript
**Data & ML:** pandas · NumPy · SciPy · PyMC · scikit-learn · Jupyter
**LLM systems:** structured output validation · multi-provider fallback · retrieval (BM25, hybrid) · evaluation harnesses · Gemini · NVIDIA NIM · Groq
**Backend & infra:** FastAPI · Streamlit · Next.js · SQLite/FTS5 · Supabase · GitHub Actions
**Also:** Dart/Flutter · MATLAB
