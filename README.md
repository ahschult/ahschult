Data engineer and systems developer. I build production-grade data pipelines, intelligence frameworks, and algorithmic trading infrastructure primarily in **Rust** and **Python**.

Most of my active work lives on a self-hosted Gitea instance and is mirrored here. Private repos are noted where operational security or client data is a factor.

---

## Active Projects

**[charcoal](https://github.com/ahschult/charcoal)** — Declarative, DataFrame-native chart library for Polars. No browser, no Python bridge, no C FFI. SVG, HTML, and PNG/JPEG/WEBP output via pure-Rust rendering. Built because the Rust ML ecosystem had no first-class visualization story for DataFrames.

**[stellar_voyage](https://github.com/ahschult/stellar_voyage)** — Multi-stage Rust data pipeline ingesting ESA Gaia DR3 (~1.8B stars) and NASA Exoplanet Archive via ADQL. Zero-copy binary deserialization via rkyv for sub-millisecond runtime asset loads. Includes a field-level data provenance classification system tagging every record by observation quality, and a Bevy-based space exploration front end built on the processed catalog.

**[citp-public](https://github.com/ahschult/citp-public)** — Congressional intelligence and statistical arbitrage platform. Post-ingestion intelligence layer converting raw regulatory filings and congressional disclosures into confidence-scored, workflow-ready signals. Includes a cointegration-based crypto pairs arbitrage engine with walk-forward backtesting and Sharpe-gated live execution, an options pricing system with full Black-Scholes Greeks and Newton-Raphson IV solver, and a multi-source weighted signal aggregator with entity relationship modeling. Live trading infrastructure kept private by design; model layer sanitization in progress.

**SwimDB** *(private — client data)* — Analytics platform for competitive swimming organizations. Three-layer medallion architecture in DuckDB and Parquet with a Polars/Python ETL pipeline. Delivers athlete performance tracking, national rankings comparisons, and development trend reporting to club clients. Replaced manual spreadsheet workflows with automated, queryable data infrastructure.

**[meridian](https://github.com/ahschult/meridian)** *(private)* — Real-time computer vision analytics system built in Rust. Ingests live and recorded video, runs an ML inference pipeline, and produces structured per-object metrics - all within a single binary using a data-driven ECS architecture.

---

## Stack

- **Systems & pipelines:** Rust (tokio, axum, polars, arrow, rkyv, bevy), Python (Polars, DuckDB, FastAPI)
- **Data:** Apache Arrow, Parquet, DuckDB, TimescaleDB, PostgreSQL, Medallion Architecture
- **Infrastructure:** Proxmox VE, Kubernetes (Talos), TrueNAS/ZFS, Linux, Docker, CI/CD

---

## Background

Twelve years running data-driven performance programs in competitive sport before moving full-time into software and data engineering. That background shows up in how I approach systems: operational reliability matters, complex findings need to be communicable to non-technical stakeholders, and things need to hold up outside of controlled conditions.

---

*Public repos here are either open source projects or sanitized mirrors of private Gitea work. Commit history is preserved on migration.*
