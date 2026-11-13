# Meta Pixel Event Map — Dhaka Accessories (Simulated)

**Disclaimer:** Simulated tracking plan for portfolio purposes. No real website or customer data is involved.

## Pixel Overview
| Field | Value |
|---|---|
| Pixel name | Dhaka Accessories Pixel |
| Pixel ID | [your-pixel-id] |
| Status | Inactive (no website connected) |
| Purpose | Track funnel events for ad optimization |

## Base Code
Installed in `<head>` of every page. Automatically fires PageView on every load.

```html
<!-- Meta Pixel Code -->
<script>
  !function(f,b,e,v,n,t,s)
  {if(f.fbq)return;n=f.fbq=function(){n.callMethod?
  n.callMethod.apply(n,arguments):n.queue.push(arguments)};
  if(!f._fbq)f._fbq=n;n.push=n;n.loaded=!0;n.version='2.0';
  n.queue=[];t=b.createElement(e);t.async=!0;
  t.src=v;s=b.getElementsByTagName(e)[0];
  s.parentNode.insertBefore(t,s)}(window, document,'script',
  'https://connect.facebook.net/en_US/fbevents.js');
  fbq('init', 'YOUR_PIXEL_ID');
  fbq('track', 'PageView');
</script>
<noscript>
  <img height="1" width="1" style="display:none"
       src="https://www.facebook.com/tr?id=YOUR_PIXEL_ID&ev=PageView&noscript=1"/>
</noscript>
<!-- End Meta Pixel Code -->

 fbq('track', 'ViewContent', {
  content_ids: ['DA-001'],
  content_name: 'Kundan Choker Set',
  content_type: 'product',
  value: 650.00,
  currency: 'BDT'
});
fbq('track', 'AddToCart', {
  content_ids: ['DA-001'],
  content_name: 'Kundan Choker Set',
  content_type: 'product',
  value: 650.00,
  currency: 'BDT'
});

fbq('track', 'InitiateCheckout', {
  content_ids: ['DA-001'],
  num_items: 1,
  value: 650.00,
  currency: 'BDT'
});

fbq('track', 'Purchase', {
  content_ids: ['DA-001'],
  content_name: 'Kundan Choker Set',
  content_type: 'product',
  value: 650.00,
  currency: 'BDT',
  num_items: 1
});


### করণীয়:
1. `08_Pixel_Tracking` folder-এ **New File** → `Pixel_Verification_Plan.md`

```markdown
# Pixel Verification Plan (Simulated)

## Tools
- **Meta Pixel Helper** (Chrome extension) — free, shows Pixel events live on page
- **Events Manager → Test Events** — Meta-র internal verification tool 

## Verification Steps
| Step | Action | Expected Result |
|---|---|---|
| 1 | Install Pixel Helper extension | Icon appears in Chrome toolbar |
| 2 | Open website home page | Pixel Helper shows PageView |
| 3 | Go to product page | Pixel Helper shows ViewContent with content_ids |
| 4 | Click Add to Cart | Pixel Helper shows AddToCart |
| 5 | Go to checkout | Pixel Helper shows InitiateCheckout |
| 6 | Complete purchase | Pixel Helper shows Purchase with value and currency |
| 7 | Check Events Manager → Test Events | All events appear with timestamps |

## Common Errors to Check
| Error | Cause | Fix |
|---|---|---|
| Event shows as "custom" | Wrong case (viewcontent vs ViewContent) | Fix case exactly  |
| Purchase has no value | value parameter missing | Add value and currency [citation:14] |
| PageView fires twice | Base code duplicated | Check `<head>` for duplicate code |
| No events at all | Pixel ID wrong or code in wrong place | Verify Pixel ID, place in `<head>`  |

## Note
We have no live website yet. This plan is ready for when the website exists.