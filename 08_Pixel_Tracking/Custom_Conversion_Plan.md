# Custom Conversion Plan (Simulated)

## What is a Custom Conversion
A Custom Conversion is a narrower rule on top of a standard event. For example, instead of tracking all Purchases, track only Purchases above a certain value. 

## Planned Custom Conversions
| Name | Based on Standard Event | Rule | Use |
|---|---|---|---|
| CC_Purchase_Above_500 | Purchase | value > 500 BDT | Optimize for high-value orders |
| CC_AddToCart_Kundan | AddToCart | content_ids contains "DA-001" | Product-specific retargeting |
| CC_Purchase_Bundle | Purchase | num_items > 1 | Bundle offer optimization |

## When to Use
- After 50+ standard events collected
- When you want to optimize for a specific product or order value
- When broad Purchase optimization is not profitable enough

## Note
Custom conversions are built in Events Manager → Custom Conversions. 
We cannot create them yet because Pixel has no data. This is the plan.