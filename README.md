<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>BMW Sales Analysis – Project README</title>
<style>
:root{--bg:#f6f8fb;--card:#fff;--text:#1c2430;--muted:#5b6675;--accent:#1c69d4;--line:#e1e6ee;--fill:#fff3c4;--fillt:#6b5200;color-scheme:light}
@media (prefers-color-scheme:dark){:root{--bg:#10151c;--card:#1a212b;--text:#e8edf4;--muted:#9aa6b5;--accent:#5aa2ff;--line:#2a3340;--fill:#4a3d10;--fillt:#ffe28a;color-scheme:dark}}
*{box-sizing:border-box}
body{margin:0;background:var(--bg);color:var(--text);font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;line-height:1.65}
header{background:linear-gradient(135deg,#0b2a55,#1c69d4);color:#fff;padding:52px 20px;text-align:center}
header h1{margin:0 0 8px;font-size:2rem}
header p{margin:0;opacity:.9}
main{max-width:920px;margin:0 auto;padding:24px 20px 60px}
section{background:var(--card);border:1px solid var(--line);border-radius:12px;padding:22px;margin-top:20px}
h2{margin-top:0;color:var(--accent);font-size:1.25rem}
h3{margin:18px 0 6px;font-size:1.05rem}
.fill{background:var(--fill);color:var(--fillt);padding:1px 6px;border-radius:4px;font-weight:600}
.rec{border-left:4px solid var(--accent);background:var(--bg);padding:10px 14px;border-radius:0 8px 8px 0;margin:12px 0}
.rec b{color:var(--accent)}
.rec small{display:block;color:var(--muted)}
code{background:var(--bg);padding:2px 6px;border-radius:6px;font-family:ui-monospace,Consolas,monospace}
ul,ol{padding-left:22px}
.tags span{display:inline-block;border:1px solid var(--line);border-radius:20px;padding:2px 12px;margin:3px 4px 3px 0;font-size:.85rem;color:var(--muted)}
footer{text-align:center;color:var(--muted);padding:20px}
</style>
</head>
<body>
<header>
  <h1>🚗 BMW Car Sales Analysis</h1>
  <p>Power BI dashboard · What I did and what the data recommends</p>
</header>

<main>

<section>
  <h2>1. Objective</h2>
  <p>To analyse BMW car sales and build an interactive Power BI dashboard that helps a business team understand <b>what sells, where it sells, and how sales are changing</b>, then turn those findings into clear recommendations.</p>
</section>

<section>
  <h2>2. What I Did</h2>
  <ol>
    <li><b>Collected the data</b> – downloaded the BMW Car Sales Classification dataset from Kaggle.</li>
    <li><b>Cleaned and prepared it</b> – loaded it into Power BI and used Power Query to check data types, remove errors and prepare columns.</li>
    <li><b>Built a star schema</b> – one fact table (<code>FactSales</code>) connected to dimension tables: <code>DimModel</code>, <code>DimRegion</code>, <code>DimYear</code>, <code>DimFuel</code>, <code>DimTransmisson</code>, <code>DimColor</code>.</li>
    <li><b>Wrote DAX measures</b> – <code>Total cars Sold</code>, <code>Total Revenue</code>, <code>Average price</code>, <code>Model Rank</code>, <code>Top Model</code>, <code>YoY Sales Growth%</code>.</li>
    <li><b>Designed the dashboard</b> – 5 KPI cards and 8 interactive visuals (line, donut, pie, bar, 100% stacked column, scatter and stacked area charts), all cross-filtering.</li>
    <li><b>Analysed the results</b> – read each visual to find patterns and wrote the recommendations below.</li>
  </ol>
  <div class="tags">
    <span>Power BI</span><span>Power Query</span><span>DAX</span><span>Data Modelling</span><span>Data Visualisation</span>
  </div>
</section>

<section>
  <h2>3. Key Findings</h2>
  <p><i>Fill the highlighted blanks from your dashboard.</i></p>
  <ul>
    <li>Total cars sold: <span class="fill">[ number ]</span> and total revenue: <span class="fill">[ amount ]</span>.</li>
    <li>Average price: <span class="fill">[ amount ]</span>.</li>
    <li>Best-selling model: <span class="fill">[ model ]</span>; top 5 models: <span class="fill">[ list ]</span>.</li>
    <li>Strongest region: <span class="fill">[ region ]</span>; weakest region: <span class="fill">[ region ]</span>.</li>
    <li>Most popular fuel type: <span class="fill">[ fuel ]</span> (<span class="fill">[ % ]</span> of sales).</li>
    <li>Transmission split: <span class="fill">[ Automatic % ]</span> vs <span class="fill">[ Manual % ]</span>.</li>
    <li>Sales trend: <span class="fill">[ rising / falling / flat ]</span>, latest YoY growth <span class="fill">[ % ]</span>.</li>
    <li>Most popular colour: <span class="fill">[ colour ]</span>.</li>
  </ul>
</section>

<section>
  <h2>4. Recommendations</h2>
  <p>Each recommendation is linked to a visual in the dashboard. Keep the ones your data supports.</p>

  <h3>📦 Product / Model strategy</h3>
  <div class="rec"><b>Prioritise stock and marketing for the top-selling models.</b>
    Focus inventory and promotion on <span class="fill">[ top models ]</span>, which drive the largest share of sales.
    <small>Based on: Top 5 Models bar chart</small></div>
  <div class="rec"><b>Review low-ranking models.</b>
    Check whether <span class="fill">[ lowest models ]</span> need price changes, better positioning or reduced production.
    <small>Based on: Model Rank and Revenue by Model pie chart</small></div>

  <h3>🌍 Regional strategy</h3>
  <div class="rec"><b>Protect and grow the strongest region.</b>
    Keep investing in <span class="fill">[ top region ]</span> with dealership support and targeted campaigns.
    <small>Based on: Sales by Region donut chart</small></div>
  <div class="rec"><b>Create a growth plan for weaker regions.</b>
    Test local promotions, financing offers or model mix changes in <span class="fill">[ weak region ]</span>.
    <small>Based on: Sales by Region donut chart</small></div>

  <h3>⛽ Fuel &amp; technology</h3>
  <div class="rec"><b>Align the product mix with fuel-type demand.</b>
    If <span class="fill">[ Electric / Hybrid ]</span> share is growing, increase availability; if it is small, run awareness and incentive campaigns.
    <small>Based on: Fuel Type donut chart and Engine Size vs Price scatter</small></div>
  <div class="rec"><b>Use the engine-size and price relationship for pricing.</b>
    Check for models priced out of line with their engine size and adjust pricing or packages.
    <small>Based on: Engine Size vs Price scatter chart</small></div>

  <h3>⚙️ Configuration &amp; customer preference</h3>
  <div class="rec"><b>Stock according to transmission preference.</b>
    Order more <span class="fill">[ Automatic / Manual ]</span> vehicles in line with the sales split.
    <small>Based on: Transmission 100% stacked column</small></div>
  <div class="rec"><b>Plan colour availability.</b>
    Keep popular colours like <span class="fill">[ colours ]</span> well stocked and limit slow colours.
    <small>Based on: Colour stacked area chart</small></div>

  <h3>📈 Growth &amp; monitoring</h3>
  <div class="rec"><b>Track YoY growth regularly.</b>
    Use the YoY Sales Growth % KPI to spot slowdowns early and investigate the years or regions behind them.
    <small>Based on: YoY KPI card and Sales by Year line chart</small></div>
</section>

<section>
  <h2>5. Limitations</h2>
  <ul>
    <li>The dataset is from Kaggle and may be simulated or simplified, so results should be validated with real company data before major decisions.</li>
    <li>Cost, profit margin and customer data are not included, so recommendations focus on sales and revenue, not profitability.</li>
  </ul>
</section>

<section>
  <h2>6. Future Improvements</h2>
  <ul>
    <li>Add profit margin and cost data.</li>
    <li>Add forecasting of future sales.</li>
    <li>Add slicers for Year, Region and Model.</li>
    <li>Publish the report to Power BI Service for sharing.</li>
  </ul>
</section>

<section>
  <h2>7. Author</h2>
  <p><b>Your Name</b> · <a href="https://github.com/your-username">GitHub</a> · <a href="https://linkedin.com/in/your-profile">LinkedIn</a></p>
</section>

</main>
<footer>⭐ If you found this project useful, feel free to star the repo!</footer>
</body>
</html>
