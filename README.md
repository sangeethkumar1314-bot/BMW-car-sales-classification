# 🚗 BMW Car Sales Dashboard (Power BI)

An interactive Power BI dashboard that analyses BMW car sales by model, region, fuel type, transmission, colour and year. It is built on the **BMW Car Sales Classification** dataset from Kaggle.

![BMW Dashboard](dashboard.png)

---

## 📌 Project Overview

This project turns raw BMW sales records into a clear, interactive view that answers questions like:

- How many cars were sold, and how much revenue did they generate?
- Which BMW models and regions perform best?
- How are sales split across fuel types, transmissions and colours?
- How have sales changed from year to year?
- How do engine size and price relate for each fuel type?

---

## 🧰 What I Did

1. **Collected the data** from Kaggle (BMW Car Sales Classification).
2. **Cleaned and prepared it** in Power BI using Power Query.
3. **Built a star schema** with one fact table and six dimension tables.
4. **Wrote DAX measures** for sales, revenue, average price, ranking and YoY growth.
5. **Designed the dashboard** with 5 KPI cards and 8 interactive visuals.
6. **Analysed the results** and wrote recommendations.

---

## 📊 Dashboard Contents

### KPI Cards
| KPI | Description |
|---|---|
| **Total Cars Sold** | Total sales volume |
| **Average Price** | Average car price (USD) |
| **Total Revenue** | Total revenue generated |
| **Top Model** | Best-selling BMW model |
| **YoY Sales Growth %** | Year-over-year change in sales |

### Visuals
| Visual | Chart Type | Insight |
|---|---|---|
| Sales by Year | Line chart | Sales trend over time |
| Sales by Region | Donut chart | Regional contribution |
| Top 5 Models | Bar chart | Best-performing models |
| Sales by Fuel Type | Donut chart | Fuel type share |
| Sales by Transmission | 100% stacked column | Manual vs automatic |
| Revenue by Model | Pie chart | Revenue share per model |
| Engine Size vs Price | Scatter chart | Price vs engine size by fuel |
| Sales by Colour | Stacked area chart | Colour preferences |

---

## 🔍 Key Insights

*Fill in the blanks from your dashboard.*

- Total cars sold: **[ number ]**, total revenue: **[ amount ]**
- Average price: **[ amount ]**
- Best-selling model: **[ model ]**
- Top region: **[ region ]**, weakest region: **[ region ]**
- Most popular fuel type: **[ fuel ]** (**[ % ]** of sales)
- Transmission split: **[ Automatic % ]** vs **[ Manual % ]**
- Sales trend: **[ rising / falling / flat ]**, latest YoY growth **[ % ]**
- Most popular colour: **[ colour ]**

---

## ✅ Recommendations

### 📦 Model strategy
1. **Prioritise stock and marketing for top-selling models.** Focus on **[ top models ]**, which drive the largest share of sales. *(Top 5 Models chart)*
2. **Review low-performing models.** Check whether **[ lowest models ]** need price changes, better positioning or reduced production. *(Revenue by Model chart)*

### 🌍 Regional strategy
3. **Protect and grow the strongest region.** Keep investing in **[ top region ]** with dealership support and targeted campaigns. *(Sales by Region chart)*
4. **Build a growth plan for weaker regions.** Test local promotions, financing offers or a different model mix in **[ weak region ]**. *(Sales by Region chart)*

### ⛽ Fuel and pricing
5. **Match the product mix to fuel-type demand.** If **[ Electric / Hybrid ]** share is growing, increase availability. If it is small, run awareness and incentive campaigns. *(Fuel Type chart)*
6. **Check pricing against engine size.** Look for models priced out of line with their engine size and adjust pricing or packages. *(Engine Size vs Price chart)*

### ⚙️ Customer preference
7. **Stock by transmission preference.** Order more **[ Automatic / Manual ]** cars in line with the sales split. *(Transmission chart)*
8. **Plan colour availability.** Keep popular colours such as **[ colours ]** well stocked and limit slow-selling ones. *(Colour chart)*

### 📈 Monitoring
9. **Track YoY growth regularly.** Use the YoY KPI to spot slowdowns early and investigate the years or regions behind them. *(YoY card and Sales by Year chart)*

---

## ⚠️ Limitations

- The dataset comes from Kaggle and may be simulated, so validate results with real company data before major decisions.
- Cost and profit data are not included, so the analysis covers sales and revenue, not profitability.

---

## 🧱 Data Model (Star Schema)

- **Fact table:** `FactSales`
- **Dimension tables:** `DimModel`, `DimRegion`, `DimYear`, `DimFuel`, `DimTransmisson`, `DimColor`

## 🧮 DAX Measures

`Total cars Sold` · `Total Revenue` · `Average price` · `Model Rank` · `Top Model` · `YoY Sales Growth%`

---

## 🛠️ Tools Used

- Power BI Desktop
- Power Query
- DAX
- Star schema modelling

---

## 🚀 How to Use

1. Download or clone this repository.
2. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows).
3. Open `Dashboard_BMW.pbix` and explore the visuals.

---

## 👤 Author

**Your Name**
- GitHub: [@sangeethkumar1314-bot](https://github.com/sangeethkumar1314-bot)
