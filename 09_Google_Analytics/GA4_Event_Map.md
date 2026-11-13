# GA4 Ecommerce Event Map — Dhaka Accessories (Simulated)

**Disclaimer:** Simulated GA4 tracking plan for portfolio purposes. No real website or customer data is involved.

## GA4 Property Overview
| Field | Value |
|---|---|
| Account | Dhaka Accessories |
| Property | Dhaka Accessories Web |
| Timezone | Bangladesh (GMT+06:00) |
| Currency | BDT |
| Data Stream | Dhaka Accessories Web (Web) |
| Measurement ID | G-XXXXXXXXXX (simulated) |
| Status | Inactive (no website connected) |

## Why GA4 and Meta Pixel Both
- Meta Pixel: ad optimization and retargeting
- GA4: business analysis, funnel, content performance
- Same funnel, different event names and purposes

## Event Name Mapping (Pixel vs GA4)
| Funnel Step | Meta Pixel Event | GA4 Event | Key Event? |
|---|---|---|---|
| Page view | PageView | page_view | No |
| Product view | ViewContent | view_item | No |
| Add to cart | AddToCart | add_to_cart | Yes (micro-conversion) |
| Checkout start | InitiateCheckout | begin_checkout | No |
| Purchase | Purchase | purchase | Yes (primary conversion) |

## GA4 Event Details

### view_item
| Parameter | Type | Example |
|---|---|---|
| currency | string | BDT |
| value | number | 650 |
| items[].item_id | string | DA-001 |
| items[].item_name | string | Kundan Choker Set |
| items[].price | number | 650 |
| items[].quantity | integer | 1 |

### add_to_cart
| Parameter | Type | Example |
|---|---|---|
| currency | string | BDT |
| value | number | 650 |
| items[].item_id | string | DA-001 |
| items[].item_name | string | Kundan Choker Set |
| items[].price | number | 650 |
| items[].quantity | integer | 1 |

### begin_checkout
| Parameter | Type | Example |
|---|---|---|
| currency | string | BDT |
| value | number | 650 |
| items[].item_id | string | DA-001 |
| items[].item_name | string | Kundan Choker Set |
| items[].price | number | 650 |
| items[].quantity | integer | 1 |

### purchase (CRITICAL: transaction_id required)
| Parameter | Type | Example |
|---|---|---|
| transaction_id | string | T_10001 |
| currency | string | BDT |
| value | number | 650 |
| items[].item_id | string | DA-001 |
| items[].item_name | string | Kundan Choker Set |
| items[].price | number | 650 |
| items[].quantity | integer | 1 |

## Key Events (Conversions) to Mark
| Event | Why |
|---|---|
| purchase | Primary revenue conversion |
| add_to_cart | Strong intent signal |

## What We Cannot Do Yet
- No live website → GA4 stays inactive
- No real customer data → all parameters simulated
- No GTM setup yet → GA4 code installation is planned, not executed

## Verification Plan (When Website Exists)
1. Install GA4 tag (via Google Tag Manager or gtag.js)
2. Open website, check Realtime report shows page_view
3. Use DebugView (Admin → DebugView) to see events live
4. Perform test actions: view product, add to cart, purchase
5. Confirm each event appears with correct parameters
6. Mark purchase as Key Event