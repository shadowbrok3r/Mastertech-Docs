---
tags:
  - mastertech
  - tab
  - shared
---

# My Tools

My Tools is a **personal virtual filesystem** built into Mastertech. It gives each user their own private storage space for tools, scripts, files, and resources — accessible from anywhere you log into Mastertech.

> Shared tab — available in both `Mastertech.exe` and at [master-tech.app](https://master-tech.app). See [[0. Table of Contents]].

---

## What It Is

My Tools acts like a personal file manager inside Mastertech. Unlike the [[File Browser]] (which browses the local machine's physical filesystem), My Tools is a virtual space that persists to your account — you can access the same files whether you're on your tech machine, a customer's machine, or the web interface.

---

## Use Cases

- **Store your own scripts** — Keep personal automation scripts you use regularly
- **Saved templates** — Store pre-written recommendation templates for common service scenarios
- **Reference files** — Keep driver notes, part numbers, or other reference documents handy
- **Tool downloads** — Store frequently used installer files or utilities

---

## Integration

My Tools is built on the `displays::virtual_filesystem` module — it's a server-side virtual filesystem backed by SurrealDB, meaning your files are stored in the Mastertech database and sync across devices.

---

## Related Tabs

- [[File Browser]] — Physical filesystem browser for the local machine
- [[Scripts]] → User Scripts — Scripts stored here can be added to the Scripts library
- [[Admin Console]] → [[Script Editor]] — For shared team scripts vs. personal tools

---

*Part of: [[0. Table of Contents]]*
