---
tags:
  - mastertech
  - desktop-only
  - tab
---

# Part Order

The Part Order tab provides a form for submitting special part orders tied to a customer ticket. It links directly to the current [[3. TUR Sheet|TUR Sheet]] data — if you've already pulled a ticket and filled in customer details, the Part Order tab will inherit that information automatically.

> Desktop tab only. See [[0. Table of Contents]] or [[2. Views and Layout]] for all tabs.

---

## Overview

When a customer's machine needs a part that isn't in stock, the Part Order tab lets you submit an order request while staying in Mastertech. The form pre-populates with the customer and ticket data from the active TUR session.

---

## How to Use

1. **Pull a ticket** in the [[3. TUR Sheet]] tab first — fill in the service number and customer details.
2. **Switch to Part Order** — the customer name, ticket/order number, and other relevant fields will carry over.
3. **Fill in part details** — part number, description, quantity, notes, etc.
4. **Submit the order.**

> ⚠️ You must be **logged in** to submit part orders. If you're not authenticated, the tab will prompt you to sign in.

---

## Integration with TUR Sheet

The Part Order tab is designed as a companion to the [[3. TUR Sheet]]. The `customer_name`, `service_number`, and ticket context are passed from the TUR sheet state directly into the part order form — so you don't have to re-enter the same information twice.

---

## Related Tabs

- [[3. TUR Sheet]] — Provides the customer and ticket context
- [[4. Task Boards]] — The task created by the TUR will track the part order status
- [[Inventory]] — Check current stock before ordering

---

*Part of: [[0. Table of Contents]]*
