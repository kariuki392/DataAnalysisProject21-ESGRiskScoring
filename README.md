# 📊 Advanced Institutional ESG Risk Scoring & Predictive Analytics Framework
### Quantitative Asset Management & Multi-Factor Portfolio Risk Engineering

---

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python&logoColor=white" alt="Python 3.10">
  <img src="https://img.shields.io/badge/Pandas-2.0-indigo?style=flat-square&logo=pandas&logoColor=white" alt="Pandas 2.0">
  <img src="https://img.shields.io/badge/Statsmodels-0.14-orange?style=flat-square" alt="Statsmodels 0.14">
  <img src="https://img.shields.io/badge/Framework-SFDR%20/%20EU%20Taxonomy-darkblue?style=flat-square" alt="Framework SFDR">
  <img src="https://img.shields.io/badge/Domain-Quantitative%20Finance-crimson?style=flat-square" alt="Domain Quantitative Finance">
</p>

---

## 🚀 Business Case & Problem Statement
In contemporary asset management, fixed static weight systems are considered an analytical blind spot. Environmental risk metrics like carbon intensity pose an immediate, existential threat to an Energy generator via carbon taxation frameworks, yet they represent a negligible operational liability to a Financial services firm. Conversely, internal data privacy metrics and corporate governance structures are of paramount importance to institutional banks and software enterprises.

### 💡 The Solution
This framework implements an **Advanced Dynamic Industry Materiality Matrix Engine** that adjusts risk-exposure weightings dynamically according to sector classification. Furthermore, the pipeline integrates statistical anomaly auditing via multi-variable **Z-score profiling** and executes an empirical **Ordinary Least Squares (OLS) regression framework** to isolate factor elasticity. This transitions the pipeline from a simple visual reporting utility into a predictive risk engine suitable for stress-testing multi-asset portfolios.

This repository is structured for analysts and portfolio teams who want a clear, practical way to explore ESG risk across sectors.

---

## 📊 Advanced Framework & Quantitative Architecture

### 1. Dynamic Industry Materiality Matrix
To accurately model operational liabilities, the framework deprecates uniform scaling in favor of variable institutional weighting matrices tailored to real market risk baselines:

| Sector | Environmental ($E$) Weight | Social ($S$) Weight | Governance ($G$) Weight | Primary Risk Focus |
| :--- | :---: | :---: | :---: | :--- |
| **Energy** | `0.60` | `0.20` | `0.20` | Carbon Transition Liabilities |
| **Manufacturing** | `0.50` | `0.25` | `0.25` | Supply Chain Logistical Redundancy |
| **Technology** | `0.20` | `0.40` | `0.40` | Intellectual Property & Human Capital |
| **Healthcare** | `0.20` | `0.40` | `0.40` | Regulatory Compliance & Clinical Oversight |
| **Financials** | `0.10` | `0.40` | `0.50` | Fiduciary Integrity & Systemic Auditing |

The final score is computed row-by-row matching sectoral rules:
$$\text{Total ESG Score} = (E_{\text{Score}} \times W_{E, \text{Sector}}) + (S_{\text{Score}} \times W_{S, \text{Sector}}) + (G_{\text{Score}} \times W_{G, \text{Sector}})$$

### 2. Statistical Outlier Detection via Z-Scores
Rather than utilizing fixed sorting boundaries, the system uses formal statistical thresholds to locate true portfolio anomalies. Standardized $Z$-scores are computed over raw parameters:

$$Z = \frac{X - \mu}{\sigma}$$

Assets exhibiting an operational profile skewing beyond **$1.5$ standard deviations ($Z > 1.5$)** relative to the cross-portfolio baseline mean are flagged as critical volatility risks.

### 3. Multi-Variable Factor Elasticity Modeling (OLS Regression)
To mathematically validate the structural influence of each non-financial operational indicator on the composite assessment index, the pipeline fits an Ordinary Least Squares (OLS) regression model:

$$Y_{\text{Total ESG Score}} = \beta_0 + \beta_1(X_{\text{Carbon Intensity}}) + \beta_2(X_{\text{Board Diversity}}) + \beta_3(X_{\text{Supply Chain Risk}}) + \beta_4(X_{\text{Controversy Flags}}) + \epsilon$$

This yields explicit $R^2$ performance capture metrics, parameter weights ($\beta_n$), and $p$-value statistical significances.

---



## 🛠️ Implementation & Technical Setup
### 📦 1. Environment Setup & Prerequisites
Use an isolated virtual environment (venv) inside this project directory to avoid system permission issues. Then install the core analytics stack:

```bash
pip install numpy pandas matplotlib seaborn statsmodels ipykernel debugpy
```

## 📈 Visual Insights & Analytics Dashboards
The automated engine compiles and outputs 5 structural reporting assets:

### 📉 1. Portfolio Risk Profiles & Pillar Benchmarks (`esg_portfolio_heatmap_dashboard.png`)
- Sector ESG performance heatmap showing materiality-weighted scores.
- Risk class distribution for portfolio segment balance.

### 📊 2. Sector Benchmark Variance & Target Exposures (`esg_sector_benchmarks_laggards.png`)
- Cross-sector score boxplots for benchmark comparison.
- Target laggard identification for low-scoring assets (`Score < 50`).

### 🎯 3. Risk Frontier Analysis (`esg_risk_frontier_analysis.png`)
- Efficiency frontier view of environmental intensity versus logistics risk.
- Governance strength shown with dynamic marker sizing.

### 🧬 4. Factor Interdependency Matrix (`esg_factor_correlations.png`)
- Pearson correlation heatmap across non-financial risk drivers.
- Highlights interaction patterns between ESG factors.

### ⚖️ 5. Governance Auditing Metrics (`esg_governance_vulnerabilities.png`)
- Controversy count and governance vulnerability analysis.
- Elasticity trends for high-visibility risk events.

## ⚠️ 6. Methodology Limitations & Boundary Conditions

While this framework provides a highly rigorous, statistically backed quantitative assessment pipeline, deploying algorithmic models to evaluate real-world ESG exposure presents distinct integration limits that must be noted:

### 1. The Synthetic Data Uniformity Illusion
* **Limitation:** This pipeline processes a complete, perfectly structured matrix of variables with zero missing values. 
* **Real-World Context:** True corporate sustainability auditing suffers from severe data fragmentation. Smaller/mid-cap firms lack dedicated sustainability reporting resources, resulting in sparse data fields, uneven disclosure frequencies, and heavily lagging reporting timelines.

### 2. Provider Discrepancy & Alpha Attrition
* **Limitation:** The Min-Max scaling layer inside this model assumes an explicit, objective linear relationship between operational parameters and absolute risk scores.
* **Real-World Context:** Unlike standardized credit ratings (where S&P and Moody's correlate at ~99%), major ESG ratings agencies (MSCI vs. Sustainalytics) display structural score correlations of only ~50-60%. This divergence stems from varying internal data scraping methodologies, proprietary linguistic sentiment weights, and differing default tracking baselines.

### 3. Structural Survivorship & Greenwashing Arbitrage
* **Limitation:** The framework measures current controversy incident frequencies as a hard point-deduction floor.
* **Real-World Context:** Highly capitalized companies often employ sophisticated public relations architectures to deliberately obfuscate supply chain or governance oversights, artificially dampening the sensitivity of external risk modifier flags.
## 📈 Summary & Asset Allocation Recommendations
## Quantitative Executive Summary
⚡ **Operational Sector Drag:** The Energy Sector faces structural performance suppression due to inherent carbon intensity tracking profiles. To achieve a composite "Leader" ranking, these assets require top-quartile governance and social score mitigations.

💥 **Volatility Acceleration:** Corporate controversy triggers are the single most aggressive drivers of rapid downside risk, immediately wiping out marginal operational optimization gains.

🧩 **Structuring Governance Synergies:** Empirical multi-factor testing confirms that strong governance score thresholds track alongside improved logistical supply chain metrics, indicating structural corporate alignment.

### Asset Allocation Directives
- **Reallocate high-exposure laggards:** Divest or underweight the designated Top 7 low-scoring assets (`Score < 50`) to hedge structural exposure.
- **Deploy carbon-efficiency overlays:** Increase asset allocation to Technology and Healthcare as structural compliance cushions.
- **Institute shareholder proxy interventions:** For average market performers (`50 ≤ Score < 75`), use active governance engagement to strengthen board diversity and oversight.

## 📂 Project Structure & Components

```bash
esg_risk_scoring/
│
├── 📓 esg_analytics.ipynb          # Interactive Jupyter Notebook holding full statistical stack
├── 🐍 generate_dashboards.py       # Automated graphic visualization reporting engine script
├── 📊 esg_portfolio_scorecard.csv  # Standardized data output tracking all 30 company assets
└── 📂 dashboards/                  # Visual reporting directories holding exported assets
    ├── 📉 esg_portfolio_heatmap_dashboard.png
    ├── 📊 esg_sector_benchmarks_laggards.png
    ├── 🎯 esg_risk_frontier_analysis.png
    ├── 🧬 esg_factor_correlations.png
    └── ⚖️ esg_governance_vulnerabilities.png