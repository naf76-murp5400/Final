<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Mixed-Use Development Strategy</title>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f8f9fb;
      color: #1f2937;
    }
    header {
      background: #111827;
      color: white;
      padding: 40px;
      text-align: center;
    }
    section {
      padding: 40px;
      max-width: 1000px;
      margin: auto;
    }
    h2 {
      border-bottom: 2px solid #e5e7eb;
      padding-bottom: 10px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }
    .card {
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.05);
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 20px;
      background: white;
    }
    th, td {
      padding: 12px;
      border-bottom: 1px solid #e5e7eb;
      text-align: center;
    }
    th {
      background: #f3f4f6;
    }
    canvas {
      margin-top: 30px;
    }
    .highlight {
      background: #ecfdf5;
      padding: 15px;
      border-left: 5px solid #10b981;
      margin-top: 20px;
    }
  </style>
</head>
<body>

<header>
  <h1>Mixed-Use Development Strategy</h1>
  <p>Capital Allocation & Public-Private Investment Recommendation</p>
</header>

<section>
  <h2>Overview</h2>
  <p>
    This analysis evaluates three mixed-use development opportunities—Waterfront DC, 
    Landover Mall, and South Riding, VA—to determine the optimal capital allocation strategy 
    balancing return, risk, and public impact.
  </p>
</section>

<section>
  <h2>Financial Comparison</h2>

  <table>
    <tr>
      <th>Metric</th>
      <th>Waterfront DC</th>
      <th>Landover Mall</th>
      <th>South Riding, VA</th>
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
      <td>Residual Land Value</td>
      <td>$18.0M</td>
      <td>$26.5M</td>
      <td>$141.6M</td>
    </tr>
  </table>

  <canvas id="noiChart"></canvas>
  <canvas id="costChart"></canvas>
  <canvas id="rlvChart"></canvas>

</section>

<section>
  <h2>Development Strategy</h2>

  <div class="grid">

    <div class="card">
      <h3>South Riding, VA</h3>
      <p><strong>Flagship Investment</strong></p>
      <p>Highest NOI and land value. Strong residential demand supports retail.</p>
    </div>

    <div class="card">
      <h3>Waterfront DC</h3>
      <p><strong>Strategic Urban Play</strong></p>
      <p>Lower cost, stable returns, strong alignment with smart growth.</p>
    </div>

    <div class="card">
      <h3>Landover Mall</h3>
      <p><strong>Redevelopment Opportunity</strong></p>
      <p>High cost and risk, but strong candidate for public-private partnership.</p>
    </div>

  </div>
</section>

<section>
  <h2>Capital Allocation</h2>

  <div class="highlight">
    <strong>Recommended Strategy:</strong>
    <ul>
      <li>60–70% → South Riding (Primary Return Driver)</li>
      <li>20–30% → Waterfront DC (Stability + Urban Impact)</li>
      <li>10–20% → Landover Mall (Only with Public Incentives)</li>
    </ul>
  </div>

</section>

<section>
  <h2>Final Recommendation</h2>
  <p>
    Approve a phased mixed-use development strategy led by South Riding, supported by 
    Waterfront DC, and conditionally including Landover Mall through public-private partnership.
  </p>
</section>

<script>
  const labels = ["Waterfront DC", "Landover Mall", "South Riding"];

  new Chart(document.getElementById("noiChart"), {
    type: "bar",
    data: {
      labels: labels,
      datasets: [{
        label: "NOI (Millions)",
        data: [4.9, 16.1, 21.7]
      }]
    }
  });

  new Chart(document.getElementById("costChart"), {
    type: "bar",
    data: {
      labels: labels,
      datasets: [{
        label: "Total Cost (Millions)",
        data: [79.7, 363.8, 396.9]
      }]
    }
  });

  new Chart(document.getElementById("rlvChart"), {
    type: "bar",
    data: {
      labels: labels,
      datasets: [{
        label: "Residual Land Value (Millions)",
        data: [18.0, 26.5, 141.6]
      }]
    }
  });
</script>

</body>
</html>
