# Sales & Order Performance Dashboard

A single-page dashboard I built to practice turning raw e-commerce data into something a non-technical person could actually read. Uses the Olist Brazilian e-commerce dataset (~100K orders, 2016–2018).

## What it does

The dashboard has four controls at the top: metric (sales / orders / AOV), time range, granularity (month / quarter / year), and a state filter. Everything below reacts to those controls.

Charts included:
- Sales over time (toggle between area, bar, line)
- Orders by state (polar area)
- Orders per quarter
- Top N categories by sales (switch between horizontal bar and bubble)
- São Paulo's share of orders over time
- Payment type breakdown
- Order status breakdown
- Category profile for top 5 states (radar)
- Orders by day-of-week × hour (heatmap)

## Running locally

```bash
git clone https://github.com/kevinmeng1022/sales-performance-dashboard.git
cd sales-performance-dashboard
open index.html
```

## Data

[Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) on Kaggle.

## Notes

- The heatmap uses raw canvas drawing instead of a Chart.js plugin, since Chart.js doesn't ship a native matrix chart.
- State filter is wired to all charts except the "Orders by State" map, which would be redundant.

## Contact

Kevin Meng · [LinkedIn](https://linkedin.com/in/mengkevin)
