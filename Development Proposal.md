# Mixed-Use Development Strategy  
### Capital Allocation & Public-Private Investment Recommendation  

This analysis evaluates three mixed-use development opportunities to determine the optimal capital allocation strategy across retail and residential assets.

## Sites Analyzed
- **Waterfront DC** — Urban Infill  
- **Landover Mall** — Redevelopment Opportunity  
- **South Riding, VA** — Greenfield Growth  

---

## Overview

The objective is to identify a development strategy that balances:

- Financial return  
- Risk exposure  
- Public-private partnership potential  
- Long-term asset value creation  

This analysis combines financial feasibility with sensitivity testing to inform a board-level investment decision.

---

## Financial Comparison

| Metric | Waterfront DC | Landover Mall | South Riding, VA |
|--------|-------------|---------------|------------------|
| **Total Cost** | $79.7M | $363.8M | $396.9M |
| **NOI** | $4.9M | $16.1M | $21.7M |
| **Residual Land Value (RLV)** | $18.0M | $26.5M | $141.6M |

plt.figure()
plt.bar(df["Site"], df["NOI"])
plt.title("Net Operating Income Comparison")
plt.ylabel("NOI ($)")
plt.xticks(rotation=20)
plt.show()
---
plt.figure()
plt.bar(df["Site"], df["Total Cost"])
plt.title("Total Development Cost Comparison")
plt.ylabel("Cost ($)")
plt.xticks(rotation=20)
plt.show()

---
plt.figure()
plt.bar(df["Site"], df["RLV"])
plt.title("Residual Land Value Comparison")
plt.ylabel("RLV ($)")
plt.xticks(rotation=20)
plt.show()

---
import numpy as np

rent_change = np.linspace(-0.2, 0.2, 10)  # -20% to +20%

noi_base = df["NOI"]

plt.figure()

for i, site in enumerate(df["Site"]):
    noi_sensitivity = noi_base[i] * (1 + rent_change)
    plt.plot(rent_change, noi_sensitivity, label=site)

plt.title("NOI Sensitivity to Rent Changes")
plt.xlabel("Rent Change (%)")
plt.ylabel("NOI ($)")
plt.legend()
plt.show()

---
cost_change = np.linspace(-0.2, 0.2, 10)

rlv_base = df["RLV"]

plt.figure()

for i, site in enumerate(df["Site"]):
    rlv_sensitivity = rlv_base[i] * (1 - cost_change)
    plt.plot(cost_change, rlv_sensitivity, label=site)

plt.title("RLV Sensitivity to Cost Changes")
plt.xlabel("Cost Change (%)")
plt.ylabel("Residual Land Value ($)")
plt.legend()
plt.show()

---

## Key Insights

### South Riding, VA — Flagship Investment
- Highest NOI and Residual Land Value  
- Strong residential-driven retail demand  
- Most scalable and financially resilient  

**Takeaway:** Primary return driver  

---

### Waterfront DC — Strategic Urban Investment
- Lowest total development cost  
- Stable, lower-risk returns  
- Strong alignment with transit-oriented development  

**Takeaway:** Portfolio stabilizer + urban impact  

---

### Landover Mall — Public-Private Redevelopment Opportunity
- High cost relative to value creation  
- Most sensitive to market fluctuations  
- Requires public subsidy to be viable  

**Takeaway:** Conditional investment only  

---

## Sensitivity Findings

### Rent Sensitivity
- **South Riding** shows strong upside with rent growth  
- **Landover Mall** is highly sensitive to rent declines  
- **Waterfront DC** remains stable but capped  

### Cost Sensitivity
- **South Riding** maintains feasibility under cost increases  
- **Landover Mall** becomes quickly infeasible  
- **Waterfront DC** has the lowest exposure  

---

## Capital Allocation Strategy

A diversified investment approach is recommended:

- **60–70% → South Riding, VA**  
  *Primary return engine*  

- **20–30% → Waterfront DC**  
  *Stability + urban positioning*  

- **10–20% → Landover Mall (Conditional)**  
  *Only with public-private partnership support*  

---

## Public-Private Investment Framing

| Site | Role | Public Sector Alignment |
|------|------|------------------------|
| **South Riding** | Growth driver | Infrastructure support |
| **Waterfront DC** | Urban catalyst | Strong planning alignment |
| **Landover Mall** | Equity-focused redevelopment | Requires incentives (TIF, grants) |

---

## Final Recommendation

Approve a phased mixed-use development strategy:

> **Lead with South Riding for returns, support with Waterfront for stability, and pursue Landover only through structured public-private partnership.**

This approach:
- Maximizes financial performance  
- Balances risk across asset types  
- Aligns with regional economic and planning goals  
