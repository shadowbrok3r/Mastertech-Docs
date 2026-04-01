---
tags:
  - mastertech
  - tab
  - shared
---

# Create Prestashop Order

The Create Prestashop Order tab is a **multi-step order creation form** that lets you build a new Prestashop order directly from Mastertech — without logging into the Prestashop back-office. It's useful for creating service orders for walk-in customers or for situations where a new order needs to be created manually.

> Shared tab — available in both `Mastertech.exe` and at [master-tech.app](https://master-tech.app). See [[0. Table of Contents]].

---

## Workflow Steps

The form walks you through three sequential steps:

### Step 1 — Select or Create Customer

**Select existing customer:**
- Search for an existing Prestashop customer by name, email, or phone
- Select them from the results to use their existing account

**Create new customer:**
- If the customer isn't in Prestashop yet, fill out the new customer form
- Fields: name, email, phone, address

### Step 2 — Create Order

Once a customer is selected/created:
- Choose order type and products
- Search the **Odoo product catalog** for parts, services, or systems to add to the order
- Set quantities and pricing

### Step 3 — Service Details

Fill in service-specific details for the order:
- Service description
- Technician assignment
- Notes and special instructions
- Any additional service line items

---

## Odoo Product Search

During the order creation step, you can search the **Odoo product catalog** to find and add products to the order. This integrates Mastertech with the company's inventory/product management system.

---

## When to Use This

- Walk-in customer who doesn't have a Prestashop account yet
- Creating a service order for a repair that wasn't checked in through the normal flow
- Quickly building an order without logging into Prestashop separately
- Any situation where you need to create a Prestashop order from a tablet or remote location

---

## Related Tabs

- [[3. TUR Sheet]] — For existing check-ins from Prestashop or Everest
- [[Task Audit]] — The order created here will appear in the audit trail
- [[Store Tasks]] — Tasks associated with the new order show up here
- [[Inventory]] — Check available parts before creating the order

---

*Part of: [[0. Table of Contents]]*
