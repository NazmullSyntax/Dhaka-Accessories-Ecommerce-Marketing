# GA4 DebugView Verification Plan (Simulated)

## What is DebugView
DebugView shows events in real-time as they fire on your website. It is the primary tool to verify GA4 setup before trusting reports. 

## How to Access
1. Install GA4 DebugView Chrome extension, OR
2. Add `?debug_mode=true` to website URL, OR
3. Use Google Tag Manager Preview mode
4. In GA4: Admin → DebugView

## Verification Steps
| Step | Action | Expected Event in DebugView |
|---|---|---|
| 1 | Open home page | page_view |
| 2 | Click product DA-001 | view_item with items array |
| 3 | Click "Add to Cart" | add_to_cart with value 650, currency BDT |
| 4 | Go to checkout | begin_checkout |
| 5 | Complete test order | purchase with transaction_id, value, currency |

## Common GA4 Errors
| Error | Cause | Fix |
|---|---|---|
| No events at all | GA4 tag not installed | Install gtag.js or GTM tag |
| view_item missing items[] | items passed as string, not array | Pass native JS array |
| purchase counted twice | transaction_id missing or duplicate | Ensure unique transaction_id per order |
| currency mismatch | "BDT" vs "bdt" | Use uppercase ISO code consistently |
| Event name wrong case | `Purchase` instead of `purchase` | GA4 uses snake_case, all lowercase |

## Important Note
GA4 silently accepts events with wrong parameters but excludes them from ecommerce reports. Data appears lower than reality without any warning. DebugView is the only way to catch this.