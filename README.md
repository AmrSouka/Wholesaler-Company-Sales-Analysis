# Wholesaler Company Sales Analysis

A Power BI dashboard analyzing sales performance for a wholesale/retail distribution business, covering revenue trends, commodity performance, brand classification, and customer age demographics.

![Dashboard Overview](docs/images/dashboard-overview.png)

## Overview

The **Sales Analysis** dashboard gives a single view into total sales, order volume, and household reach, with breakdowns by month, commodity, brand type, and customer age category — filterable by month, department, and store.

## Filters

| Filter | Options |
|---|---|
| Month | All / by month |
| Department | All / by department |
| Store ID | All / by store |

## Top KPI Cards

| Metric | Value |
|---|---|
| Total Sales | $3.26M |
| Total Quantity | 111.50M |
| Total Orders | 112,706 |
| Total Households | 2,446 |

## Total Sales by Month

Line chart of monthly sales trend, ranging from ~$350K–$400K January through July, a sharp dip to ~$100K around November, and a rebound to ~$400K by December.

## Total Sales by Commodity

Horizontal bar chart ranking commodities by total sales, top to bottom:

1. Coupon/Misc Items
2. Soft Drinks
3. Beef
4. Fluid Milk Products
5. Cheese
6. Frozen Meat/Meat Products
7. Baked Bread/Buns
8. Beers/Ales

## Total Sales by Brand Classification

Pie chart split between:

| Brand | Sales | % |
|---|---|---|
| National | $2.32M | 71.08% |
| Private | $0.94M | 28.92% |

## Total Sales and Total Orders by Age Category

Grouped bar chart (log-scale axis) comparing Total Sales vs. Total Orders across age categories: Unknown, 45-54, 35-44, 25-34, 65+, 55-64, 19-24 — with the Unknown segment leading in both sales and orders.

## Tech Stack

- **Power BI Desktop** — data modeling, DAX measures, and report layout
- Data source: wholesale sales transactions dataset (store, department, commodity, brand, and customer demographic data)

## Repository Structure

```
wholesaler-sales-analysis/
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── images/
│   │   └── dashboard-overview.png
│   └── CHANGELOG.md
└── pbix/
    └── (place your .pbix file here)
```

## Getting Started

1. Clone this repository.
2. Open the `.pbix` file (once added under `pbix/`) in Power BI Desktop.
3. Update data source connections under **Home > Transform data > Data source settings**.
4. Refresh the data model.

## Roadmap / Ideas

- [ ] Add store-level drill-through
- [ ] Add year-over-year comparison
- [ ] Add commodity-level profit margin analysis
- [ ] Document DAX measures in `docs/dax-reference.md`

## License

See [LICENSE](LICENSE).
