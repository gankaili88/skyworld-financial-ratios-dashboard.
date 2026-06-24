# SkyWorld Development Berhad — 4-Year Financial Ratios Dashboard

A Power BI dashboard analysing four years of financials for SkyWorld Development Berhad 
(Bursa Malaysia: 5325), a listed Malaysian property developer, built with an audit and 
analytical-review lens grounded in ISA 520.

## Quick view

![Overview](screenshots/01_overview.png)
![Profitability](screenshots/02_profitability.png)
![Liquidity & Gearing](screenshots/03_liquidity_gearing.png)
![Risk Flags](screenshots/04_risk_flags.png)

## The audit / finance problem

Analytical procedures under ISA 520 require auditors to identify ratios and 
movements that diverge from expectations. This dashboard operationalises that 
review for a property developer, where industry-specific factors (long DIO, 
MFRS 15 percentage-of-completion revenue, contract assets, progress billings) 
make standard ratio analysis misleading without context.

## What I built

- **Source:** 3 audited Annual Reports (FY2023–FY2025 published; FY2022 from prior year comparatives). ~25 line items per year.
- **Tools:** Excel (data preparation), Power BI Desktop (data model + visualisations), DAX (30+ measures).
- **Output:** 5-page dashboard (Overview, Profitability & Returns, Liquidity & Gearing, Risk Flags, Sources & Limitations).
- **Audit feature:** Risk Flags page applies ±20% YoY thresholds across all major ratios, mirroring the analytical review thresholds in ISA 520.

## Key findings

- Revenue collapsed from RM 841m (FY23 peak) to RM 445m (FY25) — a 47% drop over two years.
- Gross margin held / improved (31.6% → 37.1%) — pricing discipline maintained through the slowdown.
- DSO doubled (104 → 202 days) and DIO doubled (155 → 297 days); Cash Conversion Cycle expanded from ~103 days to 248 days. → signals potential inventory impairment risk (MFRS 102) and elevated ECL on receivables (MFRS 9).
- Interest coverage halved (14.9x → 6.8x). Still safe in absolute terms, but the two-year decline warrants going-concern monitoring (ISA 570).
- Net gearing improved (0.36 → 0.11) despite declining earnings — disciplined deleveraging.
- DuPont decomposition: ROE compressed from 27.9% to 6.4%, driven by simultaneous declines in net margin, asset turnover, and equity multiplier.

## What I learned and limitations

- This is a portfolio piece, not an audit opinion. A real audit would require segment-level data, bank covenant terms, project-level NRV testing, and management inquiries.
- Working capital days computed on average balances; FY2022 shows blank because no FY2021 prior balance was incorporated.
- DAX measures verified against an Excel ratio model (also in this repo).
- A YoY % can be misleading when the prior-year base is small (see Net Gearing flag) — auditors interpret the level, not just the percentage move.

## How to view

- **Quickest:** open `SkyWorld_Dashboard.pdf` for a static view of all 5 pages.
- **Interactive:** open `SkyWorld_Dashboard.pbix` in Power BI Desktop (free download); ensure `skyworld_ratios_populated.xlsx` is in the same folder so the data source resolves.

## About

Built by Gan Kai Li as part of a self-directed audit analytics portfolio. ICAEW 
Professional Level candidate, incoming Big Four audit associate.

[LinkedIn](https://www.linkedin.com/in/gan-kai-li-a8a782317/) · [GitHub](https://github.com/gankaili88)
