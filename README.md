[README (6).md](https://github.com/user-attachments/files/27368757/README.6.md)
# Hermès · The Atelier Ledger
### Luxury Chronology Analytics Series · Repo 1

![SQL](https://img.shields.io/badge/SQL-PostgreSQL-7F77DD?style=flat-square)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-D85A30?style=flat-square)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-Formulas-1D9E75?style=flat-square)
![Excel](https://img.shields.io/badge/Excel-Advanced-639922?style=flat-square)
![Era](https://img.shields.io/badge/Era-1837–1880-2C1A0E?style=flat-square)

---

## About the House

Hermès was founded in 1837 by Thierry Hermès as a harness and saddlery workshop in Paris's 9th arrondissement. Its earliest clients were European nobility, military officers, and the haute bourgeoisie — a clientele whose patronage was not transactional but relational. Each commission was bespoke, each piece a direct expression of the craftsman's skill and the client's standing.

What makes Hermès analytically compelling is not its modernity but its continuity. The business decisions that define the house today — controlled scarcity, uncompromising craft standards, resistance to volume growth — were already present in the workshop's earliest decades. The data in this project reconstructs that founding logic: who the clients were, who built the work, what it cost to make, and how revenue compounded across four distinct eras of the atelier's first forty-three years.

This is not a case study in disruption. It is a case study in discipline.

---

## The Analytical Lens

The central question this project asks is: what does the data of a bespoke luxury workshop reveal about the economics of prestige? A modern luxury analyst at Hermès today would recognize every tension in this dataset — client concentration risk, craftsman irreplaceability, the counterintuitive margin profile of smaller goods versus grand commissions, and the feast-and-famine revenue pattern that defines commission-driven business models. The 1837 atelier and the 2024 maison are separated by nearly two centuries. The analytical questions are identical.

---

## Project Structure

| Tool | Era Covered | Key Concepts Demonstrated |
|---|---|---|
| SQL | 1837–1880 | JOINs, CTEs, window functions, RANK(), LAG(), running totals |
| Power BI | 1837–1880 | Dual-axis line chart, scatter plot, stacked bar, DAX measures, era reference lines |
| Google Sheets | 1837–1880 | COUNTIFS, SUMIF, IFS with AND(), expanding range cumulative totals, conditional formatting |
| Excel | 1837–1880 | XLOOKUP, RANK, sparklines, structured tables, Executive Summary dashboard |

---

## Key Findings

- **Client concentration:** Comte de Paris alone accounted for 17.74% of total atelier revenue. The top four clients were all Royalty — collectively representing 50.28% of all revenue. Every Military and Bourgeoisie client fell below the atelier average of 1,550fr.

- **Craftsman irreplaceability:** Thierry Hermès fulfilled 8 of 30 commissions and generated 47.77% of total atelier revenue — nearly 4.3x the workshop average. His absence would have been existential to the business.

- **The margin paradox:** Smaller leather goods — satchels, portfolios, and bridles — consistently outperformed grand ceremonial pieces on margin percentage. The Carved Dispatch Satchel led at 91.28% despite a modest 430fr sale price. The Royal Presentation Saddle at 1,850fr yielded a comparatively lower 85.73%. Volume and complexity of materials, not sale price, determines margin in the Hermès atelier.

- **Compounding through volatility:** Annual revenue was volatile throughout — driven by single high-value royal commissions rather than consistent order volume. Yet cumulative revenue climbed steadily through every era, crossing 31,000fr by 1879. The bespoke luxury model: feast and famine by commission, compounding wealth by decade.

- **Productivity vs. output:** Gustave Morel commanded the highest revenue per labour day at 70fr, yet fulfilled only one commission. Henri Beaumont combined elite daily productivity with strong total output. Thierry Hermès led on volume and absolute revenue but not on per-day efficiency — the master craftsman's irreplaceability came from relationships and range, not speed.

---

## Era Framework

| Era | Years | Defining Characteristic |
|---|---|---|
| Founding Decade | 1837–1849 | Volatile early commissions — single royal orders swing entire years |
| Consolidation | 1850–1859 | Client base broadens — international nobility begins commissioning |
| Expansion | 1860–1869 | Peak revenue years — 1862 Coronation Harness at 2,850fr is the atelier's single highest commission |
| Maturity | 1870–1880 | Revenue moderates — workshop reputation established, clientele stable |

---

## Lexicon

| Term | Definition |
|---|---|
| **Sellier** | Saddler. The founding craft identity of Hermès — informs the house's quality language to this day |
| **Maroquinerie** | Leather goods division. The most margin-dense category in the modern house |
| **Atelier** | Workshop. In luxury, the atelier is not just a physical space but a statement of craft philosophy |
| **Bespoke** | Made to individual specification. The defining commercial model of the founding era |
| **Commission** | A client-initiated order for a specific piece. The revenue unit of a bespoke atelier |
| **Client tier** | The social classification of the atelier's clientele — Royalty, Nobility, Military, Bourgeoisie |
| **Revenue per labour day** | Total revenue generated divided by total days worked — a craftsman productivity metric |
| **Gross margin %** | (Sale price − material cost) / sale price × 100. The primary product profitability metric |

---

## Tools & Concepts

**SQL**
`INNER JOIN` · `LEFT JOIN` · `GROUP BY` · `HAVING` · `COUNT` · `SUM` · `AVG` · `ROUND` · `CTE` · chained CTEs · `RANK()` · `LAG()` · `SUM() OVER()` · `ROWS BETWEEN UNBOUNDED PRECEDING AND CURRENT ROW` · `CASE WHEN` · three-table JOIN · junction table pattern · NULL handling

**Power BI**
Clustered bar chart · Scatter plot · Stacked bar chart · Dual-axis line chart · DAX measures · X-axis constant line · Dynamic average line · Era reference lines · Tier color system · Analytical text annotations · Interactive slicer · Bubble sizing by field

**Google Sheets**
`SUMIF` · `COUNTIFS` · `IFS` with `AND()` · `ROUND` · `SUM($C$3:C3)` expanding range · `IF(ROW()=2,"",C1)` lag pattern · `">"&E2` dynamic operator concatenation · Conditional formatting with custom formulas · Color scale heat map · Tier band formatting · Era band formatting

**Excel**
`XLOOKUP` · `RANK` · `IFS` · `COUNTIFS` · `MAX` nested in `XLOOKUP` · Sparklines · Structured tables · Named ranges · Executive Summary dashboard · Cross-tab formula references · Freeze panes · Number formatting

---

## About This Series

This repository is part of the **Luxury Chronology Analytics Series** — a portfolio project tracing the history of reputable luxury and major apparel brands from founding to present, told through data. Each brand receives its own repository. Each repository moves through SQL, Power BI, Google Sheets, and Excel. The analytical questions are grounded in real luxury retail metrics. The work is designed to read as if produced inside an actual luxury house analytics team.

**Series order:** Hermès (1837) → Louis Vuitton (1854) → Burberry (1856) → Prada (1896) → Chanel (1910) → and beyond.

---

*Luxury Chronology Analytics Series · Analyst: Mikal Brisbon · 2026*
