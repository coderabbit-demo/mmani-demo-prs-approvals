---
id: order-invariants
name: Order Invariants
paths:
  - "services/**"
  - "packages/contracts/**"
mode: error
report: platform
---
Fail when the PR can produce any of the following, and name the file and line:

- an order line with quantity < 1 or a negative unit price
- a discount stored as an order line
- discountCents greater than subtotalCents, or a negative netCents
- a weakened CHECK constraint
- a discount redemption that is not atomic (not in one transaction with the order update)

Otherwise pass.
