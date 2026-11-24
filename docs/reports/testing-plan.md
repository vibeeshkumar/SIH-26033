# Testing and Evaluation Plan — FarmConnect

## Functional test cases
| ID | Test | Expected result |
|---|---|---|
| TC-01 | Register with valid farmer details | Farmer account is created |
| TC-02 | Register with invalid/missing fields | Validation message is shown |
| TC-03 | Login with valid credentials | User reaches the correct role dashboard |
| TC-04 | Buyer attempts farmer-only listing edit | Access is denied |
| TC-05 | Farmer creates a valid product listing | Listing is saved and displayed |
| TC-06 | Farmer updates available quantity | New quantity and timestamp are saved |
| TC-07 | Buyer searches by product/location | Matching active listings are shown |
| TC-08 | Buyer submits order within available stock | Pending order is created |
| TC-09 | Buyer requests more than available stock | Request is rejected with clear message |
| TC-10 | Farmer accepts/rejects order | Order status is updated and visible to buyer |

## Non-functional checks
- Responsive layout on mobile, tablet and desktop.
- Basic accessibility: labels, keyboard navigation and readable contrast.
- Security: password hashing, CSRF protection, authorization and input validation.
- Performance: page-load and search response times under expected pilot load.
- Reliability: backup and restore test for the database.

## Evaluation metrics
Track active sellers, active listings, listing freshness, order acceptance, fulfilment rate, cancellations, time from order to dispatch and user feedback. Establish a baseline and reporting period before interpreting changes.

> This is a proposed test plan. Test results should be filled in only after the application has been executed and verified.
