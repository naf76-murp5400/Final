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


<table border="1" cellpadding="8" cellspacing="0" width="100%">
<tr>
<th>Metric</th>
<th>Waterfront DC</th>
<th>Landover Mall</th>
<th>South Riding</th>
</tr>

<tr>
<td>Total Cost</td>
<td>$79.7M</td>
<td>$363.8M</td>
<td>$396.9M</td>
</tr>

<tr>
<td>NOI</td>
<td>$4.9M</td>
<td>$16.1M</td>
<td>$21.7M</td>
</tr>

<tr>
<td>RLV</td>
<td>$18.0M</td>
<td>$26.5M</td>
<td>$141.6M</td>
</tr>
</table>

<h2>NOI Comparison</h2>
<canvas id="noiChart"></canvas>

<h2>Total Cost Comparison</h2>
<canvas id="costChart"></canvas>

<h2>Residual Land Value</h2>
<canvas id="rlvChart"></canvas>

<h2>Development Strategy</h2>
<ul>
<li><b>South Riding:</b> Highest returns (Primary investment)</li>
<li><b>Waterfront DC:</b> Stable, lower-risk</li>
<li><b>Landover Mall:</b> Requires public-private partnership</li>
</ul>

<h2>Final Recommendation</h2>
<p>
Allocate majority capital to South Riding, support with Waterfront DC, 
and pursue Landover only with public incentives.
</p>

<script>
const labels = ["Waterfront DC", "Landover Mall", "South Riding"];

new Chart(document.getElementById("noiChart"), {
  type: "bar",
  data: {
    labels: labels,
    datasets: [{
      label: "NOI ($M)",
      data: [4.9, 16.1, 21.7]
    }]
  }
});

new Chart(document.getElementById("costChart"), {
  type: "bar",
  data: {
    labels: labels,
    datasets: [{
      label: "Total Cost ($M)",
      data: [79.7, 363.8, 396.9]
    }]
  }
});

new Chart(document.getElementById("rlvChart"), {
  type: "bar",
  data: {
    labels: labels,
    datasets: [{
      label: "RLV ($M)",
      data: [18.0, 26.5, 141.6]
    }]
  }
});
</script>

</body>
</html>
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
