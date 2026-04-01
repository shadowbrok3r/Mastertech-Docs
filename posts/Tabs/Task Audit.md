---
tags:
  - mastertech
  - tab
  - shared
---

# Task Audit

The Task Audit tab provides a **detailed audit table** for service orders linked to Prestashop. It shows a deeper, order-centric view of task history — useful for managers and techs who need to trace the full timeline of a customer's service from check-in through completion.

> Shared tab — available in both `Mastertech.exe` and at [master-tech.app](https://master-tech.app). See [[0. Table of Contents]].

---

## What It Shows

The Task Audit table is organized around **Prestashop orders** and the tasks linked to them. Each row represents a service order and shows:

- **Order number** (Prestashop)
- **Customer name**
- **Service description**
- **Technician / Salesperson**
- **Status** — where it is in the workflow
- **Timestamps** — created, updated, completed

---

## Filter Views

The Task Audit can be filtered by service category using the `TaskAudit` filter selector:

| Filter | What it shows |
| ------ | ------------- |
| **All Services** | Every order in the audit trail |
| **In Repair** | Orders currently in the repair phase |
| **Shelved** | Orders on hold or waiting for parts |
| *(other categories)* | Configured per store/workflow |

---

## Use Cases

- **Managers** auditing tech throughput and task completion rates
- **Verifying** that a TUR was submitted for every check-in
- **Cross-referencing** Prestashop orders with Mastertech task records
- **Looking up** why a specific order doesn't have a TUR task attached

---

## Related Tabs

- [[Store Tasks]] — Live view of all open tasks (not audit-focused)
- [[Completed Tasks]] — Closed task archive
- [[Sales Tracker]] — Aggregated sales data from the same order data
- [[3. TUR Sheet]] — The source of the TUR tasks that show up here

---

*Part of: [[0. Table of Contents]]*
