---
name: overdue-triage
description: Rank Refco's overdue invoices — oldest and largest first; customers with a logged payment promise wait until their promised date.
category: collections
user-invocable: true
metadata:
  version: "1.0"
  changelog:
    - "1.0: Refco's order for chasing overdue invoices"
---

# Overdue triage

1. List every open invoice past its due date.
2. Skip any invoice with a logged payment promise whose date has not passed.
3. Rank the rest by days overdue, then by amount.
4. Return the list with invoice, customer, amount and days overdue — one line each.
