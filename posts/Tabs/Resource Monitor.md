---
tags:
  - mastertech
  - tab
  - shared
---

# Resource Monitor

The Resource Monitor tab shows **live system performance metrics** for the machine Mastertech is running on. It continuously graphs CPU, RAM, GPU, network, disk activity, temperatures, and provides a real-time process table.

> Available in both the desktop app and on the web. See [[0. Table of Contents]] or [[2. Views and Layout]] for all tabs.

---

## Metrics Displayed

### CPU
- **Usage %** over time — plotted as a live line chart
- Per-core breakdown where supported
- CPU name and clock shown in the header

### RAM
- **Used / Total** in GB
- Usage percentage over time
- Live updating bar chart

### GPU
- **GPU usage %** (if a compatible GPU is present via NVML)
- VRAM usage
- GPU name

### Network
- **Upload / Download** bandwidth in real time
- Per-adapter breakdown
- Live line chart showing traffic over time

### Disks
- **Read / Write** throughput per drive
- Currently active drives shown as metric plots

### Temperatures
- CPU and GPU temperatures (where readable)
- Displayed in °C

### Processes

A live **process table** showing:

| Column | Notes |
| ------ | ----- |
| Name | Process name |
| PID | Process ID |
| CPU % | Current CPU usage |
| RAM | Memory usage |
| Status | Running/sleeping |

Processes can be sorted by column.

---

## Chart Types

The Resource Monitor uses several chart styles depending on the metric:

| Type | Used for |
| ---- | -------- |
| **Line chart** | CPU, RAM, GPU, network over time |
| **Bar chart** | Disk read/write |
| **Metric plot** | Temperature gauges |

---

## How It Works

- Metrics are polled on a background thread at regular intervals using the `sysinfo` crate (and `nvml-wrapper` for GPU data).
- Charts display a rolling window of history — older data scrolls off the left edge as time progresses.
- Data collection starts when the tab is first opened.

---

## Use Cases

- **Before submitting a TUR** — check if the machine has obvious performance issues (CPU pinned, RAM maxed) that should be noted in recommendations
- **Diagnosing slow machines** — identify runaway processes in the process table
- **Checking temps** — catch overheating before it causes a shutdown during tuneup

---

## Related Tabs

- [[System Information]] — Static hardware summary (specs, not live metrics)
- [[Scripts]] — Run tuneup scripts while monitoring performance
- [[3. TUR Sheet]] — Document performance findings in recommendations
- [[Admin Console]] → per-client resource monitor for **remote machines**

---

*Part of: [[0. Table of Contents]]*
