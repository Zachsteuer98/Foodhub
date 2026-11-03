# FoodHub order analysis

A portfolio case study of restaurant demand, customer ratings, order cost, and delivery performance using 1,898 FoodHub orders.

## Open the presentation

Open [`foodhub_dashboard.html`](foodhub_dashboard.html) in a modern browser. The standalone page includes the full dataset, interactive filters, and CSV export; it requires no server or package installation. Use **Print / Save PDF** to create a static copy.

## Analysis process

The presentation follows the analysis from the original project: profile the dataset and rating completeness; examine restaurant, cuisine, cost, rating, preparation-time, and delivery-time distributions; compare demand and service measures across categories; answer the business questions; then summarize findings and recommendations.

Charts include frequency bars, cost and time histograms and boxplots, cuisine-by-day and prep-by-delivery heatmaps, cuisine price comparisons, prep time by rating, and delivery-time comparisons by day and cuisine.

## Corrections and definitions

- The source contains 736 `Not given` ratings (not 735). These remain missing; they are not replaced with an average.
- Promotion eligibility uses submitted rating count and mean rating, not restaurant order count.
- Estimated commission is $6,166.30 using 25% on orders above $20 and 15% on orders above $5 through $20. It is commission only, not gross order value or profit.
- The over-60-minute measure combines food preparation and delivery. Delivery-time averages alone measure pickup to customer.

All findings are descriptive of this dataset. Small cuisine groups and missing customer ratings limit some comparisons.
