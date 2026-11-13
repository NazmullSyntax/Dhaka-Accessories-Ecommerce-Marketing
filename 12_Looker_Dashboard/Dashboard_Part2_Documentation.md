# Looker Studio Dashboard Part 2 (Simulated)

**Disclaimer:** All data is simulated (Day 17). This dashboard does not represent real business performance.

## Dashboard Link
[Your updated share link]

## Components Added (Part 2)

### Time Series Chart
| Field | Value |
|---|---|
| Dimension | Date |
| Metric 1 | Spend (BDT) — SUM |
| Metric 2 | Revenue (BDT) — SUM |
| Chart type | Line |
| Title | Spend vs Revenue (Daily) |

### Funnel Chart
| Stage | Metric |
|---|---|
| 1 | Impressions |
| 2 | Clicks |
| 3 | Purchases |
| Title | Conversion Funnel |

Note: 5-stage funnel was simplified to 3 stages because Looker Studio's funnel chart performs better with 3 metrics.

### Campaign Table
| Dimension | Campaign |
|---|---|
| Metrics | Spend, Clicks, Purchases, Revenue, ROAS, CPA |
| Sort | ROAS descending |
| Heatmap | Yes (ROAS) |
| Title | Campaign Performance Detail |

## Interactivity
- Campaign dropdown filter applies to all charts
- Date range control applies to all charts
- Tested: selecting "Kundan" updates all scorecards, charts, and table

## Full Dashboard Layout
1. Title + disclaimer
2. Filters (Date, Campaign)
3. 4 Scorecards (Spend, Revenue, ROAS, CPA)
4. Time-series (Spend vs Revenue)
5. Funnel + Campaign table
6. Bar charts (ROAS, CPA)

## Design System
- Font: Poppins (heading 20, body 11)
- Colors: Maroon #7B2D26, Green #2E7D32, Gold #C9A227, Grey #555555
- Background: White
- Borders: Light grey, radius 8

## Funnel Insight (for report)
- Impressions → Clicks: 1.89% (creative/hook)
- Clicks → ATC: 12.2% (product page/offer)
- ATC → Checkout: 56.3% (normal)
- Checkout → Purchase: 69.4% (strong)

## What the Dashboard Answers
| Question | Where to look |
|---|---|
| How much did we spend? | Spend scorecard |
| Did we make money? | Revenue + ROAS scorecards |
| Which campaign performs best? | ROAS bar chart + table |
| Where is the funnel leaking? | Funnel chart |
| How did we perform over time? | Time-series chart |
| Can I see only Kundan? | Campaign filter |