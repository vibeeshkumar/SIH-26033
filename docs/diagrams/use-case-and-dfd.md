# FarmConnect — Use Case and Data Flow Diagrams

## Use case diagram

```mermaid
flowchart LR
  Farmer([Farmer]) --> REG((Register / Login))
  Farmer --> LIST((Manage Product Listings))
  Farmer --> STOCK((Update Quantity & Price))
  Farmer --> ORDERS((Review Buyer Orders))
  Buyer([Buyer]) --> SEARCH((Search Products))
  Buyer --> VIEW((View Product Details))
  Buyer --> PLACE((Place Order))
  Buyer --> TRACK((Track Order Status))
  Admin([Administrator]) --> VERIFY((Manage Users / Listings))
  Admin --> REPORT((View Platform Reports))
  LIST --> SYS[FarmConnect Platform]
  SEARCH --> SYS
  PLACE --> SYS
  ORDERS --> SYS
```

## Level 0 data flow diagram

```mermaid
flowchart LR
  F[Farmer] -->|Profile, product, stock, price| P((FarmConnect))
  P -->|Listing status, order details| F
  B[Buyer] -->|Search, enquiry, order| P
  P -->|Product results, confirmation, status| B
  P <--> D[(Users, Products, Orders Database)]
  P <--> M[Market / Price Data]
  P <--> L[Mapping Service]
```

## Main data entities
- **User:** user ID, role, name, contact, location.
- **Product:** product ID, seller ID, name, category, unit, quantity, price, updated time.
- **Order:** order ID, buyer ID, seller ID, items, quantity, total, status, timestamps.
- **Delivery:** delivery ID, order ID, pickup and drop locations, partner, status.

> The diagrams describe the proposed workflow and logical data model, not a verified implementation schema.
