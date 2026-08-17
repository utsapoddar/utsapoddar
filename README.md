# Utsa Poddar

Physics-trained developer building data pipelines, applied ML, and LLM-powered systems. I like problems where a model has to survive contact with messy real-world data — and where the reasoning is auditable rather than a black box.

**[Portfolio](https://utsapoddar.github.io)** · **[LinkedIn](https://www.linkedin.com/in/utsa-poddar)** · **[utsapoddarjobs@gmail.com](mailto:utsapoddarjobs@gmail.com)**

---

## What I Work On

- **Data & ML** — Bayesian modeling, uncertainty-aware estimation, classification pipelines
- **LLM Systems** — treating model output as advisory and keeping a deterministic component authoritative
- **Automation & Backend** — scheduled pipelines, multi-source ingestion, APIs, CI

## Selected Work

**[Alpha Digest](https://github.com/utsapoddar/alpha-digest)** — A weekly investor-intelligence pipeline that runs itself. Ingests SEC EDGAR Form 4 and 13F filings, corporate crypto treasuries, commodity prices, and 12 financial RSS feeds; cross-references them against a 25-entity watchlist; summarizes with an LLM behind a three-model retry chain; renders with Jinja2; then emails subscribers and publishes to GitHub Pages — every Monday, on GitHub Actions cron. **[Read the current issue →](https://utsapoddar.github.io/alpha-digest)**

**[LiDAR Room Designer](https://github.com/utsapoddar/ai-interior-designer)** — Turns an iPhone RoomPlan scan into a furniture plan for your *actual* room. The USDZ mesh is parsed into structured geometry, a vision LLM extracts taste and constraints, and a deterministic Python solver owns final placement — checking clearances, door swings, and walking paths. FastAPI backend, React/Three.js preview, CI on every push.

**[MSDS Time Estimator](https://github.com/utsapoddar/msds-time-estimator)** — Bayesian estimator predicting how long a CU Boulder MSDS course will take *you*, anchored on courses you've already finished. Course posteriors update from crowdsourced review data under a tempered weight so heavily-reviewed courses tighten confidence without drowning the prior; outputs are uncertainty-aware with 80% intervals. Full derivation in [MODEL.md](https://github.com/utsapoddar/msds-time-estimator/blob/main/MODEL.md).

**[PCOS Food Scanner](https://github.com/utsapoddar/pcos-scanner)** — Scan a barcode or a photo, get a PCOS-aware score and serving advice. Nutrient scoring is deterministic and rule-based; the LLM only personalizes and explains it against your profile. Streamlit + Supabase, with tests over scoring, vision, barcode parsing, and migrations.

**[Engram](https://github.com/utsapoddar/engram)** — Durable, auditable memory for AI coding agents. Markdown notes under a typed schema, SQLite FTS5 retrieval, a replacement-first correction journal that recovers from a crash mid-write, and a recall@5 harness so retrieval quality is measured rather than assumed. Credential rejection and reasoning-stripping run on every write. 71 tests.

**[DopaKernel](https://github.com/utsapoddar/dopa-kernel)** — A control kernel for AI coding agents that keeps the authorized objective as a hard gate rather than a weighted score, so a perceived "better idea" can't silently replace the instruction. Separates adherence, verified progress, and completion evidence.

**[Cadence](https://github.com/utsapoddar/cadence)** — Eight therapeutic sound modules synthesized live in the browser with the Web Audio API: AM-modulated 40 Hz gamma, binaural beats, and a user-calibrated notch filter for tinnitus. Every module is gated on peer-reviewed clinical support with an evidence tier and DOI as structured fields, and the exclusions are documented as deliberately as the inclusions. A NumPy/SciPy script regenerates each spec as reference WAVs to check the JS synthesis against an independent implementation. **[Try it →](https://utsapoddar.github.io/cadence/)**

**[Sift Work Timer](https://github.com/utsapoddar/sift-work-timer)** — Cross-platform Flutter work timer (iOS / Android / macOS / Windows) with alarms, phase transitions, and streak tracking. Distributed via AltStore and Google Play.

## Stack

**Languages** Python · SQL · JavaScript · Dart · TypeScript · MATLAB
**Data & ML** pandas · NumPy · SciPy · PyMC · scikit-learn · Jupyter
**Backend & Infra** FastAPI · Streamlit · SQLite/FTS5 · Supabase · GitHub Actions
**LLM** Gemini · Groq · NVIDIA NIM · prompt/tool design · retrieval

## Elsewhere

[Physics simulations](https://github.com/utsapoddar/physics-python-projects) · [SQL analytics](https://github.com/utsapoddar/SQL-queries) · [n8n workflows](https://github.com/utsapoddar/n8n-projects) · [Fraud detection](https://github.com/utsapoddar/Fintech-Project) · [Fluid dynamics](https://github.com/utsapoddar/fluid_dynamics)

---

I'm open to data science, ML, and backend/automation roles. Based in Calgary, Alberta. If something here is relevant to your team, reach out at **[utsapoddarjobs@gmail.com](mailto:utsapoddarjobs@gmail.com)**.
