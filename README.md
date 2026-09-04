# Myntra Wishlist Confidence Check MVP

A product-management graduation project prototype for improving **Wishlist → Purchase conversion** on Myntra without using discounts or other monetary incentives.

## Product idea

**Myntra Confidence Check** is a decision-support layer shown when a shopper revisits a wishlisted fashion product. Instead of adding another promotion, it brings the most useful purchase-confidence signals together at the decision point:

- Fit and size evidence
- Buyer-photo / real-world appearance signals
- Material and quality signals
- A simple purchase-confidence score
- A lightweight fit-context selector
- Clear evidence explaining why confidence is high or low

The goal is to reduce uncertainty that causes high-intent shoppers to save an item, research it, and leave without buying.

## MVP flow

1. Open the Myntra-style home screen.
2. Browse **Men, Women, Kids, Home, or Beauty**.
3. Search for products or browse category products.
4. Open **Wishlist** to see saved products.
5. Select a wishlist product.
6. Review the **Confidence Check**.
7. Choose fit context such as usual size, size up/down, or unsure.
8. Review evidence around fit, buyer photos, and quality.
9. Add the product to **Bag**.
10. Continue to checkout (represented as an MVP interaction).

## Included categories

The prototype includes at least three products in each of these categories:

- Men
- Women
- Kids
- Home
- Beauty

The sample catalog uses real product names and publicly accessible product imagery collected during the discovery/prototyping phase.

## Key product hypothesis

> High-intent apparel wishlist users delay purchase because the product page does not provide enough confidence that the specific item will fit and look right on their body.

The MVP intentionally tests this hypothesis without introducing price cuts, coupons, cashback, or other monetary incentives.

## Research context

The discovery work used public feedback sources such as app-store reviews and online community discussions. The initial public corpus highlighted **fit/size confidence** as a strong opportunity area, alongside quality, trust, returns/exchange, value, styling/occasion, and other decision barriers.

The public corpus is a discovery input, **not a representative estimate of Myntra's user population**. The final opportunity should be validated through user interviews and product testing.

## Success metrics

### Primary business metric
**Wishlist → Purchase Conversion (30-day):** percentage of users who add at least one item to Wishlist and purchase at least one wishlisted item within 30 days of the wishlist add event.

### Leading indicators
- Confidence Check open rate among eligible wishlist revisits
- Evidence interaction rate
- Fit-context selection rate
- Add-to-Bag rate after Confidence Check
- Wishlist revisit → product-detail progression

### Guardrails
- Return rate
- Exchange rate
- Cancellation rate
- Customer-support contacts related to product mismatch
- Page latency / error rate

## Technical implementation

This is a lightweight static front-end MVP built as a single `index.html` file with HTML, CSS, and JavaScript.

It is intentionally a prototype rather than a production Myntra integration. A real production implementation would require official product/catalog, account, wishlist, cart, review, and analytics integrations and appropriate backend services.

## Repository structure

```text
myntra-confidence-check/
├── index.html   # Interactive MVP
└── README.md    # Project documentation
```

## Running locally

Because the MVP is static, it can be opened directly in a browser. For a local development server, use any static-file server, for example:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000` in a browser.

## Deployment

The repository is structured for static hosting such as **GitHub Pages**. Enable GitHub Pages for the repository's `main` branch and root folder, then use the repository's generated `github.io` address.

## Important prototype note

The interface is designed to demonstrate how the feature could work inside Myntra. It does **not** connect to a user's real Myntra account, real wishlist, real cart, checkout, or private recommendation/review systems. Product data and imagery in the prototype are sample/publicly accessible references used for demonstration.

## Project goal

The MVP is designed to answer one product question:

**Can decision-ready evidence reduce uncertainty enough to move a high-intent wishlisted item from “saved for later” to “Add to Bag,” without relying on monetary incentives?**
