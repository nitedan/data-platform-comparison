# Enterprise Data Platform Advisor — 2026

> An interactive, context-aware scoring engine for data architects, CTOs, and enterprise buyers — comparing 11 major data platforms across 23 criteria.

**Live tool:** [nitedan.github.io/data-platform-comparison](https://nitedan.github.io/data-platform-comparison/)

> Part of a larger **Enterprise Data Intelligence** initiative in progress.

---

## What is this?

Choosing a data platform is one of the highest-impact architectural decisions an organization makes. The wrong choice costs millions in migration, licensing, and lost productivity.

This tool provides a **weighted, context-aware scoring engine** that compares 11 data platforms across 20 criteria — helping data architects, CTOs, and enterprise buyers make an informed decision based on their specific situation.

---

## Platforms Covered

| Tier | Platforms |
|------|-----------|
| **Top 4 Commercial** | ⚡ Databricks · ❄️ Snowflake · 🔷 Microsoft Fabric · 🔵 Google BigQuery |
| **Open Source / Cheapest** | 🧊 Apache Iceberg + S3 |
| **Extended Enterprise** | ☁️ Azure Synapse · 🟠 Teradata Vantage · 🔹 IBM watsonx.data · 🌤️ Cloudera CDP · 🔶 Oracle Auto DW |

---

## The Advisor

### 📡 [Enterprise Data Platform Advisor](data-platform-advisor.html)

Covers the **full global enterprise market** — all 10 major commercial platforms plus Apache Iceberg+S3 as the open-source/lowest-cost reference.

**23 criteria across 5 dimensions:**
- **Capabilities** — Data Engineering · Data Warehousing · ML/AI · GenAI & LLMs · AI Tools · AI Agents · Autonomous Agentic AI · Real-Time · Streaming · SQL · Scalability
- **Operational** — Ease of Use · Power BI Integration · Data Sharing · Multi-ERP Support
- **Economics** — Cost Efficiency · Implementation Speed · Implementation Complexity
- **Architecture** — Open Standards · Vendor Lock-in · Security · EU AI Act / GDPR · Multi-Site

**8 smart context filters:**
- ⏱ Implementation Speed (Express → Complex)
- 🏢 Company Structure (SMB, Multi-Site, Multi-Plant, Multi-ERP, Global Corporation)
- 💼 Industry (Manufacturing, Finance, Healthcare, Tech, Energy, Public Sector…)
- 🧑‍💻 Team Profile (Data Eng, BI/SQL, ML/AI, Platform/Infra, Mixed)
- 💰 Monthly Budget (Starter → Enterprise)
- ☁️ Cloud Strategy (AWS-Native, Azure-Native, GCP-Native, Multi-Cloud, On-Prem/Hybrid)
- 🎯 Strategic Priority (Cost Reduction, AI/ML Leadership, Self-Service BI, Governance, Cloud Modernization, Real-Time)
- 📋 Compliance Focus (EU GDPR / AI Act, HIPAA, FedRAMP, SOC 2 / ISO 27001)

---

## How scoring works

```
Final Score = Base Score + Context Modifiers

Base Score  = Σ(weight × criterion_score) / Σ(weight × 5) × 100
Context     = Σ(filter modifiers) — each filter adds/subtracts points
              based on how well the platform fits your context
```

- **Criteria weights** are adjustable via the sidebar sliders (0–5)
- **Quick presets** cover common profiles: Data Engineer, BI/SQL, ML/AI, Platform Eng, Cost-First, Open Source, Microsoft-first, Enterprise
- **Best-in-row** highlighting shows which platform leads each criterion
- **Insight chips** surface relevant platform combinations based on your filter selections

---

## Criteria Scoring Reference (0–5 scale)

| Score | Meaning |
|-------|---------|
| 5 | Industry-leading / best-in-class |
| 4 | Strong / above average |
| 3 | Good / competitive |
| 2 | Limited / below average |
| 1 | Weak / requires significant workarounds |
| 0 | Not supported |

---

## Tech Stack

Pure **HTML + CSS + JavaScript** — no frameworks, no build step, no dependencies.

- CSS custom properties for theming and dark mode
- CSS Flexbox for the comparison grid
- Vanilla JS data-driven rendering (`render()` rebuilds DOM from data on every state change)
- Debounced render (80ms) prevents excessive redraws during slider drag
- Single-file architecture — each tool works offline, no server required

---

## License

MIT — free to use, adapt, and share.

---

*Data and scores are indicative as of 2026. Platform capabilities evolve rapidly — always verify against current vendor documentation before making procurement decisions.*
