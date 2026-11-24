# Software Requirements Specification (SRS) — FarmConnect

## 1. Purpose
FarmConnect is a proposed agricultural marketplace connecting farmers/FPOs with consumers, retailers and bulk buyers.

## 2. User roles
- Farmer: register, manage profile, publish products, update stock and review orders.
- Buyer: browse/search listings, view seller and product details, place orders and track status.
- Administrator: moderate users/listings and review platform activity.

## 3. Functional requirements
1. The system shall support farmer and buyer registration and login.
2. The system shall allow farmers to create, edit, deactivate and update product listings.
3. Each listing should include product name, category, unit, quantity, price, location and last-updated time.
4. Buyers shall be able to search and filter active listings.
5. Buyers shall be able to submit an order request.
6. Farmers shall be able to accept or reject an order.
7. The system shall maintain order status and timestamps.
8. The system may display market-price and demand-analysis information when valid data is available.
9. The system may support map-based delivery planning through a configured mapping provider.

## 4. Non-functional requirements
- Responsive and accessible interface, including mobile screens.
- Passwords must be securely hashed; secrets must not be stored in source code.
- Role-based authorization must protect farmer, buyer and admin functions.
- Validate all user input and enforce server-side stock checks.
- Keep pages lightweight for limited-connectivity environments.
- Provide clear error messages and timestamps for listings and orders.

## 5. Proposed technology stack
HTML, CSS, Bootstrap, JavaScript, Python, Django and SQLite for the prototype. A production deployment may require a more scalable database, backups, monitoring and secure hosting.

## 6. Assumptions and constraints
The proposal assumes users have access to a phone or computer and intermittent internet. Payment gateway, SMS, live logistics and external market-data integrations are not assumed to be implemented until configured and tested.

## 7. Acceptance criteria
Core acceptance requires successful role registration/login, product listing management, buyer search, order creation, seller decision and order-status updates with permission checks.
