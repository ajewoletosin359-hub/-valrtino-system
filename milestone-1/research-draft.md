# VALRTINO Milestone 1 — research draft (markets and suppliers)

Working draft for the Milestone 1 PDF. Researched 2026-10-07 from public sources. All figures are estimates until the system's own tests prove them.

## Store as seen publicly (www.valrtino.com)

- Men's and women's fashion: dresses, jeans, tops, hoodies, shoes, watches, jewelry, lingerie, accessories.
- Prices about $59.95 to $480.95; checkout in USD or EUR.
- Page shows region "AU", "free tracked shipping Australia-wide", 14-day returns.
- Not confirmed: whether the Australia wording is the store's real setup or shown by visitor location. Confirm from Shopify order data once access is given.

## Market comparison

| Market | Online fashion market 2025 (ECDB) | Meta CPM (2026 benchmarks) | Apparel return rate | CJ shipping from China |
|---|---|---|---|---|
| United States | $239.8bn | about $23.00 | about 31% | 7-12 days; some stock in US warehouses |
| United Kingdom | $53.4bn | about $10.30 | about 24% | 7-12 days |
| Canada | $16.6bn | about $13.40 | about 30% | 15-25 days |
| Australia | $10.0bn | about $18.50 | about 31% | 8-16 days |
| Singapore | $1.9bn | about $12.00 | not found | 6-12 days |
| Ireland | $1.2bn | about $7.40-12.00 | not found | not found (other EU routes 7-14 days) |
| South Africa | $1.1bn, growing 15-20% | about $2.50 | not found | not found |
| New Zealand | $0.9bn | about $11.20 | about 27% | not found |

Gaps to fill or label "not available": return rates for Singapore, Ireland, South Africa; shipping times for New Zealand, Ireland, South Africa; competition measure per market; supplier availability per market.

Tax points to flag for his accountant (not verified here): UK VAT registration for overseas sellers on consignments up to GBP 135; Australian GST registration above AUD 75,000 turnover; EU VAT/IOSS for Ireland.

Preliminary recommendation (to confirm against his Shopify sales data):
1. Start with Australia if the store's current setup and orders are there: store already configured, mid-size market, 8-16 day shipping. Weakness: second-highest ad cost and high returns.
2. Add the United Kingdom second: cheapest ads among the large markets, lowest return rate found, 7-12 day shipping, five times Australia's market size. Check UK VAT first.
3. United States later: largest market, but the most expensive ads and the most competition.
4. Hold Canada (slow shipping), and New Zealand, Ireland, Singapore, South Africa (small markets; South Africa's low ad cost comes with lower spending power against $60-480 prices).

## Supplier / fulfillment comparison

| | CJ Dropshipping | AliExpress via DSers | Zendrop |
|---|---|---|---|
| Recurring fee | None; pay product + shipping per order | DSers has a free plan; paid plans exist | $49-79/mo, or usage-based $29-79/mo on Shopify |
| Shopify integration | Free official app | Official AliExpress partner app | Official app |
| Public API for our agents | Yes, API 2.0: products, variants, stock, order create/list/detail, freight calculation, tracking, webhooks, disputes | Order API needs AliExpress approval and is restricted; DSers itself works through its app | No public API; offers an MCP server for AI assistants (unproven for this use) |
| Stock and price monitoring | Supported by API | Inside DSers app; limited for a custom system | Inside app only |
| Order submission and tracking | Supported by API | Inside DSers app | Inside app; US warehouse 5-8 days |
| Duplicate-order prevention | Built on our side using the Shopify order ID; confirm CJ order-number field in its docs | Our side cannot control it inside the app | Our side cannot control it inside the app |
| Quality and returns | Varies by listing; needs sample orders | Varies by seller | Varies; curated US catalogue |

Recommendation: CJ Dropshipping. It is the only one of the three with a documented public API covering every agreed function, and it has no subscription fee.

Not yet verified: CJ API rate limits ("Interface Call Restrictions" page), whether createOrder accepts a merchant order number, CJ return policy terms, real product quality (sample orders, at his cost).

## Sources

- https://ecdb.com/resources/sample-data/market/us/fashion (and /gb/, /ca/, /au/, /nz/, /ie/, /sg/, /za/)
- https://www.adamigo.ai/blog/meta-ads-cpm-cpc-benchmarks-by-country-2026
- https://stackmatix.com/blog/facebook-ads-cpm-by-country-2026
- https://www.superads.ai/facebook-ads-costs/cpm-cost-per-mille/south-africa
- https://ecdb.com/blog/e-commerce-return-rate-by-category/5252
- https://eightx.co/blog/australia-ecommerce-return-rate-benchmark (and Canada, New Zealand, UK pages)
- https://developers.cjdropshipping.com/en/api/api2/
- https://apps.shopify.com/cucheng
- https://parcelsapp.com/en/carriers/cjpacket
- https://support.zendrop.com/en/articles/12511531-zendrop-plans-and-pricing-standard-and-usage-based
- https://support.zendrop.com/en/articles/14461568-zendrop-mcp-server
- https://zuplo.com/learning-center/aliexpress-api-guide.md
- https://www.growave.io/best-shopify-apps/shopify-aliexpress-dropshipping
