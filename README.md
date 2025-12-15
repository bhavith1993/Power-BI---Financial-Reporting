# Financial Statements & Revenue Analytics Dashboard (Power BI)

A personal Power BI project that stitches together **Sales**, **Invoices / A/R aging**, and **Financial Statements (P&L, Balance Sheet, Cash Flow)** into a single interactive report with a navigation hub.

> **Note:** This is a personal project. The data shown in screenshots is for demonstration only.

---

## What’s inside

### Report pages
- **Navigation**: icon-based landing page to jump to each section.
- **Revenue Insights**: sales trend, rolling average, top customers/cities, monthly waterfall, profit & margin KPIs.
- **Aged Trial Balance**: invoice aging buckets (1–30 / 31–60 / 61–90 / 90+), outstanding invoice count/value, detailed invoice listing.
- **Income Statement**: selected year vs previous year, variance and % variance visuals, normalized breakdown.
- **Balance Sheet**: assets/liabilities/equity layout + common ratios and composition waterfalls.
- **Cash Flow Statement**: operations/investing/financing sections with yearly comparisons and cash-in/out summaries.
- **Financial Details**: deeper drill matrix with toggles (Actuals / vs Last Year / % to Revenue) and quarterly/annual rollups.

---

## Data model (high level)

The model is built around a few core dimensions and multiple fact-style tables:

**Dimensions**
- `Dates`
- `Customers`
- `Products`
- `Regions`

**Facts / statement tables**
- `Sales` (order-level / line-level sales metrics)
- `Invoices` (A/R invoice values and due dates)
- `Income Statement` (P&L items by month/year)
- `Balance Sheet Data`
- `Cash Flow Data`

There are also supporting mapping/template tables used to drive statement layouts (e.g., cash flow template and category tables).

---

## How to run locally

1. Download the PBIX (or clone the repo if you publish it on GitHub).
2. Open the `.pbix` in **Power BI Desktop**.
3. If you’re using external data sources, update them in:
   - **Transform data → Data source settings**
4. Click **Refresh**.

---

## Screenshots

> Tip: Put images in an `assets/` folder for cleaner paths.  
> If you keep images in the repo root, change the paths below (remove `assets/`).

### Navigation
![Navigation](assets/Navigation.png)

### Revenue Insights
![Revenue Insights](assets/Revenue%20Insights.png)

### Aged Trial Balance
![Aged Trial Balance](assets/Aged%20Trial%20Balance.png)

### Income Statement
![Income Statement](assets/Income%20Statement.png)

### Balance Sheet
![Balance Sheet](assets/Balance%20Sheet.png)

### Cash Flow Statement
![Cash Flow Statement](assets/Cash-flow%20Statement.png)

### Financial Details
![Financial Details](assets/Financial%20Details.png)

### Model Diagram
![Model Diagram](assets/Model%20Diagram.png)

---

## Repo structure (suggested)

```text
.
├── Financial_Report.pbix
├── README.md
└── assets/
    ├── Navigation.png
    ├── Revenue Insights.png
    ├── Aged Trial Balance.png
    ├── Income Statement.png
    ├── Balance Sheet.png
    ├── Cash-flow Statement.png
    ├── Financial Details.png
    └── Model Diagram.png
```

---

## Notes (keep this honest)
- If you share the PBIX publicly, assume anyone can inspect measures, model, and any cached data.
- If you want maximum safety, share a **PBIT** instead and include a small sample dataset (CSV) or a data generator script.

---

## Contact
If you’re reviewing this and want the PBIX/PBIT or a quick walkthrough, reach out via my portfolio / LinkedIn.
