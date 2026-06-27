# Data Platform Intelligence Hub — 2026

> Two interactive advisors to help enterprises select the right cloud data platform — from commercial leaders to open-source alternatives.

**Live site:** [nitedan.github.io/data-platform-comparison](https://nitedan.github.io/data-platform-comparison/)

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

## Tools

### 🧭 [Platform Advisor — Core](platform-advisor.html)
The focused advisor for most organizations. Compares the **top 4 commercial platforms + Apache Iceberg+S3** (open-source / lowest cost).

**23 criteria including:**
- Data Engineering · Data Warehousing · ML/AI · GenAI & LLMs
- **AI Tools Integration** · **AI Agent Orchestration** · **Autonomous Agentic AI** *(3-level AI maturity)*
- Real-Time Analytics · Streaming / CDC · SQL Performance · Scalability
- Ease of Use · Power BI Integration · Data Sharing · Multi-ERP Support
- Cost Efficiency · Implementation Speed · **Implementation Complexity** *(easy vs hard)*
- Open Standards · Vendor Lock-in · Security & Compliance
- **AI EU Policy / GDPR** *(EU AI Act alignment, data sovereignty)*
- Multi-Site / Multi-Plant

**Context filters (8 categories):**
- ⏱ Implementation Speed (Express → Complex)
- 🏢 Company Structure (SMB, Multi-Site, Multi-Plant, Multi-ERP, Global)
- 💼 Industry (Manufacturing, Finance, Healthcare, Tech, Energy, Public Sector…)
- 🧑‍💻 Team Profile (Data Eng, BI/SQL, ML/AI, Platform/Infra, Mixed)
- 💰 Monthly Budget (Starter → Enterprise)
- ☁️ Cloud Strategy (AWS-Native, Azure-Native, GCP-Native, Multi-Cloud, On-Prem/Hybrid)
- 🎯 Strategic Priority (Cost Reduction, AI/ML, Self-Service BI, Governance, Modernization, Real-Time)
- 📋 Compliance Focus (EU GDPR / AI Act, HIPAA, FedRAMP, SOC 2 / ISO 27001)

---

### 🏆 [Platform Advisor — Top 10](platform-advisor-top10.html)
The extended advisor for enterprise buyers evaluating the **full global market** — all 10 major platforms plus Apache Iceberg+S3.

Same 23 criteria and 8 filter categories as the Core advisor, expanded to cover legacy enterprise platforms (Teradata, IBM, Oracle) and hybrid cloud platforms (Azure Synapse, Cloudera).

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
