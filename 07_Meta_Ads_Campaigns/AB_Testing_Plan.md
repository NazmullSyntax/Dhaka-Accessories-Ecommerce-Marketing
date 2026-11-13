# A/B Testing Plan — Dhaka Accessories (Simulated)

**Disclaimer:** Simulated test plan for portfolio purposes. No real money is spent.

## Why We Test
To replace guesses with data. Every test isolates one variable so we know exactly what caused the difference.

## Test 1: Creative Test (Image vs Review)

| Field | Control (A) | Variant (B) |
|---|---|---|
| Creative | Ad1_Product_Kundan.png (product image) | Ad3_Retargeting.png (customer review) |
| Audience | Same: AUD_Cold_Kundan_Women25-34 | Same |
| Copy | Same caption | Same caption |
| Budget | 1,000 BDT | 1,000 BDT |
| Duration | 7 days | 7 days |
| Metric | CPA (cost per message/order) | CPA |

**Hypothesis:** The customer review image will have lower CPA because social proof reduces hesitation.

**What we change:** Only the image. Everything else identical.

## Test 2: Audience Test (Interest vs Broad)

| Field | Control (A) | Variant (B) |
|---|---|---|
| Audience | Women 25–34, Dhaka, interests: jewelry, wedding | Women 25–34, Dhaka only (no interests) |
| Creative | Same: Ad1_Product_Kundan.png | Same |
| Copy | Same | Same |
| Budget | 1,000 BDT | 1,000 BDT |
| Duration | 7 days | 7 days |
| Metric | CPA | CPA |

**Hypothesis:** Interest targeting will have lower CPA for a new page with no data.

**What we change:** Only the audience. Everything else identical.

## Test 3: Copy Test (Hook A vs Hook B)

| Field | Control (A) | Variant (B) |
|---|---|---|
| Hook | "বিয়ের সিজনে গয়না নিয়ে চিন্তা?" | "৬৫০ টাকায় premium look — বিশ্বাস হচ্ছে না?" |
| Creative | Same: Ad1_Product_Kundan.png | Same |
| Audience | Same: AUD_Cold_Kundan_Women25-34 | Same |
| Budget | 1,000 BDT | 1,000 BDT |
| Duration | 7 days | 7 days |
| Metric | CTR + CPA | CTR + CPA |

**Hypothesis:** The number hook ("৬৫০ টাকা") will get higher CTR because it is specific and attention-grabbing.

**What we change:** Only the first line of the caption. Body and CTA identical.

## Test Rules
- Never change more than one variable at a time.
- Run for at least 7 days. Do not check daily and do not pause mid-test.
- Budget per variant: 1,000 BDT (small-scale test for learning).
- Expect directional results, not statistical certainty, due to small sample.
- After test ends, read results in Meta Experiments, then apply the winning element to the live campaign.

## What We Will Do With Results
- If Test 1 review image wins → use review-style creative for retargeting ads
- If Test 2 interest wins → keep interest targeting; if broad wins → expand audience for 11.11
- If Test 3 number hook wins → use number hooks in all future captions

## Limitations
- Small budget means small sample size
- Results are directional, not statistically conclusive
- Bangladesh market has less data than US/EU markets
- All data is simulated