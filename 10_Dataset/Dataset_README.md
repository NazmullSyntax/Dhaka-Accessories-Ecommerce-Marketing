# Campaign Dataset — Dhaka Accessories (Simulated)

**IMPORTANT DISCLAIMER:** This dataset is 100% simulated for learning and portfolio purposes. It does NOT represent real Meta Ads performance, real customer data, or any real company's business. No real money was spent.

## What This Dataset Is
A 30-day simulated campaign dataset across 4 campaigns, with funnel metrics, calculated KPIs, and realistic variance.

## File
`campaign_data_30days.csv` — 41 rows (1 header + 40 data rows)

## Columns (13 base + 6 calculated = 19)
### Base columns
| Column | Type | Description |
|---|---|---|
| Date | Date | Campaign date (15-Nov to 15-Dec) |
| Campaign | Text | Campaign name |
| Ad Set | Text | Ad set name (audience) |
| Ad | Text | Ad creative name |
| Objective | Text | Engagement (all campaigns) |
| Spend (BDT) | Number | Daily ad spend |
| Impressions | Number | Ad impressions |
| Reach | Number | Unique people reached |
| Clicks | Number | Link clicks |
| Add to Cart | Number | AddToCart events |
| Checkout | Number | InitiateCheckout events |
| Purchases | Number | Purchase events |
| Revenue (BDT) | Number | Order revenue |

### Calculated columns
| Column | Formula | Interpretation |
|---|---|---|
| CTR (%) | Clicks ÷ Impressions × 100 | Click-through rate |
| CPC (BDT) | Spend ÷ Clicks | Cost per click |
| CPM (BDT) | Spend ÷ Impressions × 1000 | Cost per 1000 impressions |
| CPA (BDT) | Spend ÷ Purchases | Cost per acquisition |
| ROAS | Revenue ÷ Spend | Return on ad spend |
| Conv Rate (%) | Purchases ÷ Clicks × 100 | Click-to-purchase rate |

## Campaign Summary
| Campaign | Rows | Spend | Purchases | Revenue | ROAS |
|---|---|---|---|---|---|
| Kundan | 15 | 4,540 | 35 | 22,750 | 5.01 |
| Tote | 10 | 3,010 | 14 | 10,500 | 3.49 |
| Retarget | 5 | 1,500 | 16 | 10,400 | 6.93 |
| 11.11 | 10 | 6,000 | 60 | 36,000 | 6.00 |
| **Total** | **40** | **15,050** | **125** | **79,650** | **5.29** |

## How Data Was Generated
- Spend, impressions, clicks, funnel events follow Bangladesh e-commerce benchmarks (CPC ৳3–25, CPM ৳60–220)
- Variance added day by day (weekend higher, weekday lower)
- Revenue = Purchases × product AOV (Kundan 650, Tote 750, mixed 600)
- All values chosen manually to create realistic patterns for analysis practice

## What This Dataset Is NOT
- Not real Meta Ads Manager data
- Not real customer data
- Not a claim of business performance
- Not financially actionable

## Intended Use
- Learning CTR, CPC, CPM, CPA, ROAS calculation
- Practicing Google Sheets analysis
- Building Looker Studio dashboard
- Writing performance reports (Day 22–23)


Date	Campaign	Ad Set	Ad	Objective	Spend	Impressions	Reach	Clicks	ATC	Checkout	Purchases	Revenue
06-Dec	DA_1111_Sale_Dec2025	AUD_Cold_1111_Broad	DA_1111_Teaser	Engagement	550	5200	3800	95	12	7	4	2400
07-Dec	DA_1111_Sale_Dec2025	AUD_Cold_1111_Broad	DA_1111_Teaser	Engagement	580	5500	4000	105	14	8	5	3000
08-Dec	DA_1111_Sale_Dec2025	AUD_Cold_1111_Broad	DA_1111_Teaser	Engagement	600	5800	4200	115	15	9	6	3600
09-Dec	DA_1111_Sale_Dec2025	AUD_Cold_1111_Broad	DA_1111_Teaser	Engagement	620	6000	4400	125	17	10	7	4200
10-Dec	DA_1111_Sale_Dec2025	AUD_Cold_1111_Broad	DA_1111_Teaser	Engagement	650	6300	4600	135	19	11	8	4800
11-Dec	DA_1111_Sale_Dec2025	AUD_Cold_1111_Broad	DA_1111_Live	Engagement	700	6800	5000	155	22	13	9	5400
12-Dec	DA_1111_Sale_Dec2025	AUD_Cold_1111_Broad	DA_1111_LastDay	Engagement	650	6400	4700	140	20	12	8	4800
13-Dec	DA_1111_Sale_Dec2025	AUD_Cold_1111_Broad	DA_1111_LastDay	Engagement	600	6000	4400	120	16	10	6	3600
14-Dec	DA_1111_Sale_Dec2025	AUD_Warm_1111	DA_1111_Recap	Engagement	550	5000	3600	90	11	6	4	2400
15-Dec	DA_1111_Sale_Dec2025	AUD_Warm_1111	DA_1111_Recap	Engagement	500	4800