---
tags:
  - mastertech
  - desktop-only
  - tab
---

# System Information

The System Information tab displays a read-only summary of the hardware in the machine Mastertech is currently running on. It's a quick reference for specs without needing to dig through Device Manager or msinfo32.

> Desktop tab only. See [[0. Table of Contents]] or [[2. Views and Layout]] for all tabs.

---

## What It Shows

The tab displays two main tables:

### Hardware Summary

| Field | Example |
| ----- | ------- |
| Hostname | `LAPTOP-ABC123` |
| CPU | `Intel Core i7-1165G7 @ 2.80GHz` |
| RAM | `16 GB DDR4` |
| GPU | `Intel Iris Xe Graphics` |
| Motherboard | `HP ProBook 450 G8` |
| Product Name | `HP ProBook 450 G8` |

### Drive Information

A table listing all physical drives and partitions with:

| Field | Notes |
| ----- | ----- |
| Drive letter / label | C:, D:, external labels |
| Total size | In GB |
| Used / free space | Reported from the OS |
| Drive type | SSD, HDD, NVMe, USB |
| Health (where available) | SMART status if readable |

---

## Where This Data Comes From

The data is gathered automatically when Mastertech launches. It reads:
- **Hardware fields** from WMI (Windows Management Instrumentation) queries via the `wmi` crate
- **Drive info** from the system disk enumeration

This is the same data that gets **attached to a TUR Sheet** when **Send System Info** is checked — so what you see here is exactly what the salesperson will receive.

---

## Tips

- This tab is **read-only** — there are no editable fields.
- Data is populated on app startup and does not refresh live. If you plug in a new drive, restart Mastertech to see it.
- For live metrics (CPU %, RAM usage, etc.), see [[Resource Monitor]].
- For deeper crash/dump analysis, see [[Minidump Analysis]].

---

## Related Tabs

- [[3. TUR Sheet]] — System info is attached to TUR submissions when "Send System Info" is checked
- [[Resource Monitor]] — Live performance metrics
- [[Minidump Analysis]] — Crash analysis using hardware context
- [[Scripts]] — Run hardware checks in the Informational category

---

*Part of: [[0. Table of Contents]]*
