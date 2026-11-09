# Eii Thy Store

**A Khmer/English gaming storefront with a checkout that keeps the selected package and player details together.**

[Visit the live store](https://eiithystore.com) · [Customer journey](docs/customer-journey.md) · [Project status](docs/project-status.md)

## What it does

Customers browse game packages, enter their player details, and review their cart. Eligible purchases show crypto payment instructions within checkout. The store owner verifies payment before manually fulfilling the order.

| Experience | Implemented behavior |
| --- | --- |
| Product selection | Game cards, package selection, and green completion indicators |
| Cart | Player details carry forward; unavailable packages are clearly excluded |
| Payment instructions | QR code, receiving network, exact amount, and expiry appear inline |
| Order tracking | Signed-in customers can view their order status |
| Fulfillment | Owner review and manual delivery; transaction submission is not payment confirmation |
| Languages | Khmer and English storefront navigation and shopping content |

## Design decisions

- Keep one primary add-to-cart action instead of repeated review panels and buttons.
- Show completion within the relevant section rather than a duplicate step bar.
- Keep real purchases distinct from preview-only packages and test-payment tools.
- Retain customer selections throughout checkout instead of asking for them again.

## Technologies

React · TypeScript · Vite/Vinext · Cloudflare Workers · D1 · Drizzle

## Current status

Actively developed. Supported crypto purchases use manual verification and fulfillment. Some catalog entries and payment methods remain previews. See the live store for current availability; this repository does not promise supplier stock or automatic delivery.

## Repository boundaries

This is a documentation-only portfolio showcase. Source code, payment configuration, customer records, voucher codes, credentials, and production artwork are not published here. The implementation is maintained separately in a private repository.

Game names belong to their respective owners. Eii Thy Store is independent and is not affiliated with game publishers.
