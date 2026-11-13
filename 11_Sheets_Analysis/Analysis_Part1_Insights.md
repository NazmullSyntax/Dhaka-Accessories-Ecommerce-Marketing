# Google Sheets Analysis Part 1 — Insights (Simulated)

**Disclaimer:** All numbers are from the simulated dataset created on Day 17.

## Campaign Summary Table
| Campaign | Spend | Impressions | Clicks | Purchases | Revenue | CTR | CPC | CPM | CPA | ROAS |
|---|---|---|---|---|---|---|---|---|---|---|
| DA_1111_Sale_Dec2025 | 6,000 | 55,050 | 1,105 | 60 | 36,000 | 2.01% | 5.43 | 108.99 | 100 | 6.00 |
| DA_Engagement_Kundan_Nov2025 | 4,540 | 43,480 | 792 | 35 | 22,750 | 1.82% | 5.73 | 104.41 | 129.71 | 5.01 |
| DA_Engagement_ToteBag_Nov2025 | 3,010 | 31,550 | 499 | 14 | 10,500 | 1.58% | 6.03 | 95.40 | 215.00 | 3.49 |
| DA_Retarget_Kundan_Dec2025 | 1,500 | 9,250 | 237 | 16 | 10,400 | 2.56% | 6.33 | 162.16 | 93.75 | 6.93 |
| **Grand Total** | **15,050** | **139,330** | **2,633** | **125** | **79,650** | **1.89%** | **5.72** | **108.01** | **120.40** | **5.29** |

## Insight 1: Retargeting has the highest ROAS
**Observation:** Retarget campaign ROAS 6.93, highest of all 4 campaigns.
**Reasoning:** Warm audience already engaged with the page. Trust exists. Higher CPM (162) but much higher conversion.
**Action:** Increase retarget budget for 11.11. Expand warm audience window from 30 days to 60.

## Insight 2: ToteBag has the lowest CTR and highest CPA
**Observation:** CTR 1.58% (lowest), CPA 215 BDT (highest).
**Reasoning:** Audience `AUD_Cold_Tote_Students` is narrower (Men+Women 22–30, laptop interest). Creative `DA_Tote_Ad1_Product` may not be strong enough. CPM is lowest (95) but clicks do not follow through.
**Action:** Test new creative for Tote (review image + student angle). Broaden audience to include university + freelancing separately. Run A/B test on hook.

## Insight 3: 11.11 has highest spend and volume
**Observation:** Spend 6,000, purchases 60, ROAS 6.00.
**Reasoning:** Seasonal demand spike. Higher CPM (108.99) but also higher conversion. Countdown + urgency creatives drove intent.
**Action:** Replicate the countdown structure for Eid and Black Friday. Reserve 40% of monthly budget for seasonal peaks.

## Insight 4: Kundan is the strongest cold campaign
**Observation:** CTR 1.82%, CPA 129.71, ROAS 5.01.
**Reasoning:** Interest targeting (jewelry, wedding) matched the audience well. Product margin 61.5% means CPA 129 is comfortably profitable.
**Action:** Scale budget gradually (max 20% per day). Test lookalike audience after 50 purchases.

## Insight 5: CPM differs by audience type
**Observation:** Retarget CPM 162 (highest), Tote CPM 95 (lowest).
**Reasoning:** Retarget audiences are small → higher auction cost per impression. Tote audience is broad and cheap but does not convert.
**Action:** Do not judge campaign by CPM alone. Pair CPM with CTR and CPA. Cheap CPM with poor CTR is worse than high CPM with strong ROAS.

## Priority Actions This Week
1. Increase retarget budget by 30% (highest ROAS)
2. Test new creative for Tote campaign (lowest CTR)
3. Keep Kundan campaign as is, scale gradually
4. Plan Eid campaign using 11.11 structure
5. Monitor CPM — if it rises above 200, narrow audience or improve creative hook