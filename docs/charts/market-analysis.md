# FarmConnect — Illustrative Charts

The charts below use **sample demonstration values only** to show how the proposed dashboard could visualize information. They are not live AGMARKNET/e-NAM data and must not be presented as measured project results.

## Example weekly demand index

```mermaid
xychart-beta
  title "Illustrative weekly demand index"
  x-axis ["W1", "W2", "W3", "W4", "W5", "W6"]
  y-axis "Index (sample)" 0 --> 100
  bar [42, 50, 47, 63, 72, 68]
```

## Example indicative price comparison

```mermaid
xychart-beta
  title "Illustrative price comparison (₹/kg)"
  x-axis ["Market A", "Market B", "Market C", "Market D"]
  y-axis "₹ per kg (sample)" 0 --> 80
  bar [32, 36, 34, 39]
```

## Suggested live dashboard metrics
- Average listed price by crop, unit, location and date.
- Demand index calculated from search and order activity.
- Available quantity and listing freshness.
- Order acceptance, fulfilment and cancellation rates.

Before using real figures, record source, collection date, geography, crop variety, grade and unit. Do not compare unlike products or units.
