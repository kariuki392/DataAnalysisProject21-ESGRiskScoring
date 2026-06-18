# ESG Risk Scoring & Portfolio Assessment Framework

An institutional-grade, data-driven quantitative framework to audit, score, and evaluate Environmental, Social, and Governance (ESG) risk exposure across a multi-asset investment portfolio. 

This repository provides a complete, production-ready pipeline that standardizes non-financial operational metrics into uniform, actionable risk indices ($0 - 100$) for a synthetic portfolio of 30 companies across 5 core industrial sectors: Technology, Energy, Financials, Healthcare, and Manufacturing.

---

## 🚀 Business Case & Problem Statement
In modern asset management, quantitative investment strategies, and corporate sustainability consulting, ESG considerations have transitioned from secondary compliance metrics into critical alpha-generating and risk-mitigating indicators. 

Regulatory bodies globally are increasingly mandating transparent ESG disclosures. Institutional asset managers face severe exposure when holding equities with unmitigated operational liabilities:
* **Environmental:** High carbon intensity flags long-term exposure to tightening carbon tax regimes and transition risks.
* **Social:** Weak board diversity or poorly audited supply chain logistics introduce human rights violations, regulatory fines, and systemic structural vulnerabilities.
* **Governance:** Fragile internal corporate governance structures or frequent public controversy incidents result in sharp capital depreciation and erosion of investor trust.

### The Solution
This project implements a repeatable **ESG Risk Assessment Framework** that acts as an analytical proxy for live corporate risk scoring pipelines used by investment firms. It normalizes disparate operational vectors, applies specific industry weight matrices, maps risk tiers, and highlights critical capital laggards.

---

## 📊 Framework & Quantitative Architecture

### 1. Metric Scale Normalization
To resolve tracking discrepancies across highly non-uniform data types (e.g., comparing greenhouse gas volumes directly to governance scorecard decimals), the pipeline applies an explicit **Min-Max Scaling Engine**. 

All operational metrics are mapped onto a uniform scale where **100 represents peak sustainability compliance (Lowest Risk)** and **0 represents severe operational liability (Highest Risk)**:

* **Environmental (E_Score):** Derived via inverse Min-Max scaling on raw **Carbon Intensity** (Metric tons $CO_2e$ per \$M revenue). High-emission assets are mathematically penalized toward zero.
* **Social (S_Score):** Formed by a balanced, equally-weighted ($50/50$) index uniting **Board Diversity Percentages** and **Supply Chain Risk Scores** (1-100 scale inverted).
* **Governance (G_Score):** Established via base corporate **Governance Structure Scores**, subject to a deductive penalty framework subtracting **15 points per active severe controversy flag**, clipped at a hard floor of 0.

### 2. Composite Weighting Architecture
The composite quantitative assessment maps corporate equities to a strict weighting standard matching institutional allocation baselines:

$$\text{Total ESG Score} = (E_{\text{Score}} \times 0.40) + (S_{\text{Score}} \times 0.30) + (G_{\text{Score}} \times 0.30)$$

### 3. Risk Profile Tiers
Assets are continuously classified into actionable investment groups according to their weighted scores:
* **Leader (Low Risk):** $\text{Score} \ge 75$ — Robust institutional positioning, high sustainability resilience.
* **Average (Medium Risk):** $50 \le \text{Score} < 75$ — Standard compliance profile, moderate transition vulnerabilities.
* **Laggard (High Risk):** $\text{Score} < 50$ — Critical exposure; structural ESG liabilities requiring rapid capital reallocation or divestment.

---

## 📂 Project Structure & Components

```bash
esg_risk_scoring/
│
├── esg_analytics.ipynb          # Interactive Jupyter Notebook for data engineering & scoring
├── generate_dashboards.py       # Automated production script exporting high-res PNG visuals
├── esg_portfolio_scorecard.csv  # Standardized data output tracking all 30 company assets
└── dashboards/                  # High-resolution analytical graphics directory
    ├── esg_portfolio_heatmap_dashboard.png
    └── esg_sector_benchmarks_laggards.png
