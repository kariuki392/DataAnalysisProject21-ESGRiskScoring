# 📊 ESG Risk Scoring & Portfolio Assessment Framework
### Quantitative Asset Management & Corporate Sustainability Analytics

---

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python&logoColor=white" alt="Python 3.10">
  <img src="https://img.shields.io/badge/Pandas-2.0-indigo?style=flat-square&logo=pandas&logoColor=white" alt="Pandas 2.0">
  <img src="https://img.shields.io/badge/Framework-SFDR%20/%20EU%20Taxonomy-darkblue?style=flat-square" alt="Framework SFDR">
  <img src="https://img.shields.io/badge/Framework-TCFD%20Aligned-darkblue?style=flat-square" alt="Framework TCFD">
  <img src="https://img.shields.io/badge/Domain-Risk%20%26%20Compliance-crimson?style=flat-square" alt="Domain Risk & Compliance">
</p>

---

## 🚀 Business Case & Problem Statement
In contemporary asset management, quantitative investment strategies, and corporate sustainability consulting, **Environmental, Social, and Governance (ESG)** factors have transitioned from passive compliance checklists into critical alpha-generating and risk-mitigating indicators. 

Global regulatory frameworks are rapidly mandating granular non-financial disclosures. Institutional asset managers face immense tail-risk exposure when holding corporate equities with unmitigated operational liabilities:
* **🌱 Environmental:** High carbon intensity flags severe long-term exposure to tightening carbon tax regimes, regulatory caps, and structural transition risks.
* **🤝 Social:** Weak internal board diversity or poorly audited supply chain logistics introduce human rights liabilities, vendor disruptions, and heavy reputational damage.
* **⚖️ Governance:** Fragile corporate governance architectures or frequent public controversy incidents correlate with sharp capital depreciation and systemic erosion of investor trust.

### 💡 The Solution
This project implements a repeatable, institutional-grade **ESG Risk Assessment Framework** that acts as an analytical proxy for live corporate risk-scoring pipelines. The system normalizes disparate operational data vectors, applies industry-specific weight matrices, maps portfolios into structural risk categories, and systematically flags high-exposure corporate laggards.

---

## 📊 Framework & Quantitative Architecture

### 1. Metric Scale Normalization
To eliminate tracking discrepancies across highly non-uniform data dimensions (e.g., comparing raw greenhouse gas volumes directly against governance scoring decimals), the pipeline applies an explicit **Min-Max Scaling Engine**. 

All underlying operational metrics are mathematically mapped onto a uniform scale where **100 represents peak sustainability compliance (Lowest Risk)** and **0 represents severe operational liability (Highest Risk)**:

* **`E_Score` (Environmental):** Derived via inverse Min-Max scaling on raw **Carbon Intensity** (Metric tons $CO_2e$ per \$M revenue). Heavy-emission industrial assets are automatically penalized toward zero.
* **`S_Score` (Social):** Formed by a balanced, equally-weighted ($50/50$) index uniting corporate **Board Diversity Percentages** and inverted **Supply Chain Risk Scores** ($1-100$).
* **`G_Score` (Governance):** Established via base **Governance Structure Scores**, subject to a deductive penalty framework subtracting **15 points per active severe controversy flag**, clipped at a hard floor of 0.

### 2. Composite Weighting Architecture
The composite quantitative assessment maps corporate equities to a strict weighting standard matching institutional asset allocation baselines:

$$\text{Total ESG Score} = (E_{\text{Score}} \times 0.40) + (S_{\text{Score}} \times 0.30) + (G_{\text{Score}} \times 0.30)$$

### 3. Risk Profile Tiers
Assets are continuously classified into actionable investment tranches according to their final weighted scores:
* **🟩 Leader (Low Risk):** $\text{Score} \ge 75$ — Robust institutional positioning, high sustainability resilience.
* **🟨 Average (Medium Risk):** $50 \le \text{Score} < 75$ — Standard compliance profile, moderate transition vulnerabilities.
* **🟥 Laggard (High Risk):** $\text{Score} < 50$ — Critical exposure; structural ESG liabilities requiring rapid capital reallocation or divestment.

---

## 📂 Project Structure & Components

```bash
esg_risk_scoring/
│
├── 📓 esg_analytics.ipynb          # Interactive Jupyter Notebook for data engineering & scoring
├── 🐍 generate_dashboards.py       # Automated production script exporting high-res PNG visuals
├── 📊 esg_portfolio_scorecard.csv  # Standardized data output tracking all 30 company assets
└── 📂 dashboards/                  # High-resolution analytical graphics directory
    ├── 📉 esg_portfolio_heatmap_dashboard.png
    ├── 📊 esg_sector_benchmarks_laggards.png
    ├── 🎯 esg_risk_frontier_analysis.png
    ├── 🧬 esg_factor_correlations.png
    └── ⚖️ esg_governance_vulnerabilities.png