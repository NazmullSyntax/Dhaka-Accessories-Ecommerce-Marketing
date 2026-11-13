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