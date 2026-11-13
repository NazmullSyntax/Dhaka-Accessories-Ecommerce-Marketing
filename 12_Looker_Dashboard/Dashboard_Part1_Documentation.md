# Looker Studio Dashboard Part 1 (Simulated)

**Disclaimer:** This dashboard uses simulated campaign data from Day 17. It does not represent real business performance.

## Dashboard Link
[Your Looker Studio share link]

## Data Source
- Google Sheets: `Dhaka_Accessories_Campaign_Data`
- Worksheet: `Campaign_Data`
- Connection: Google Sheets connector
- First row as headers: Yes

## Components Built

### Scorecards (4)
| Metric | Formula | Value |
|---|---|---|
| Total Spend | SUM(Spend BDT) | 15,050 BDT |
| Total Revenue | SUM(Revenue BDT) | 79,650 BDT |
| Overall ROAS | SUM(Revenue) / SUM(Spend) | 5.29 |
| Overall CPA | SUM(Spend) / SUM(Purchases) | 120.40 BDT |

### Bar Charts (2)
| Chart | Dimension | Metric | Sort |
|---|---|---|---|
| ROAS by Campaign | Campaign | ROAS | Descending |
| CPA by Campaign | Campaign | CPA | Ascending |

### Controls (2)
| Control | Field | Purpose |
|---|---|---|
| Date Range | Date | Filter by date |
| Dropdown | Campaign | Filter by campaign |

## Calculated Fields
| Field | Formula |
|---|---|
| ROAS | `SUM(\`Revenue (BDT)\`) / SUM(\`Spend (BDT)\`)` |
| CPA | `SUM(\`Spend (BDT)\`) / SUM(Purchases)` |

## Design
- Font: Poppins
- Colors: Maroon #7B2D26, Green #2E7D32, Grey #555555
- Layout: Scorecards top, charts middle, controls below title
- Disclaimer at bottom

## Why This Layout
Scorecards give an instant KPI snapshot. Bar charts allow campaign comparison at a glance. Controls make the dashboard interactive so a viewer can filter by date or campaign without editing the report [citation:1][citation:14].

## What to Build Next (Day 21)
- Time-series line chart (daily spend vs revenue)
- Funnel visualization (Impressions → Clicks → ATC → Purchases)
- Table with campaign details