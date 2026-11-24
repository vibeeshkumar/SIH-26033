# FarmConnect — System Architecture

```mermaid
flowchart TD
  F[Farmer] --> UI[Web UI<br/>HTML · CSS · Bootstrap · JavaScript]
  B[Buyer / Retailer / Wholesaler] --> UI
  UI --> DJ[Django Application]
  DJ --> AUTH[Registration & Authentication]
  DJ --> PROD[Product & Inventory Management]
  DJ --> ORD[Order Management]
  DJ --> ANALYTICS[Market Analysis / Demand Forecasting]
  DJ --> MAP[Mapping & Delivery Planning]
  AUTH --> DB[(SQLite Database)]
  PROD --> DB
  ORD --> DB
  ANALYTICS --> DATA[Price / Demand Data Sources]
  MAP --> MAPAPI[Mapping Service API]
```

## Component responsibilities
- **Web UI:** responsive pages for farmers and buyers.
- **Django:** authentication, validation, business rules and application endpoints.
- **SQLite:** prototype storage for accounts, products, orders and order status.
- **Analytics:** planned analysis of historical prices and demand; predictions require validated data.
- **Mapping:** planned location and route support through an external mapping provider.

> This is the proposed architecture. External data and mapping integrations must be configured before they are operational.
