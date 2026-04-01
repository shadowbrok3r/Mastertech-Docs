---
tags:
  - mastertech
  - tab
  - shared
  - admin
  - advanced
---

# Database Editor

The Database Editor provides a **table-based view of the Mastertech SurrealDB database**. It lets authorized users browse and edit database records directly — useful for fixing data issues, inspecting the database state, and making manual corrections.

> Shared tab — available in both `Mastertech.exe` and at [master-tech.app](https://master-tech.app).  
> **Requires elevated privileges.** Handle with care — changes are permanent.

---

## Layout

### Left — Table Picker
A list of available database tables. Click a table name to load its contents in the main view.

Available tables include:
- `users` — Mastertech user accounts
- `tasks` — All tasks (TUR submissions, follow-ups, etc.)
- *(and other internal tables)*

### Center — Data View

The selected table's records displayed in rows. Each row shows the document fields for that record. Rows can be clicked to open a detail/edit view.

---

## Per-Table Viewers

Each table has a specialized row viewer that presents the data in a structured way appropriate to that table type rather than raw JSON. For example:
- **Users table** — shows name, email, store, initials, role
- **Tasks table** — shows customer info, tech/sales, status, timestamps

---

## When to Use This

- **Fixing data entry mistakes** — Correct a typo in a task or user record
- **Data inspection** — Verify what's actually stored vs. what the UI shows
- **Support requests** — Help a user with an account issue by looking up their record
- **Development** — Inspect database state during testing

---

## ⚠️ Caution

Changes made in the Database Editor are **directly written to the production database**. There is no undo. Double-check before saving any edits.

For running arbitrary queries instead of browsing tables, see [[Query Editor]].

---

## Related Tabs

- [[Query Editor]] — Run raw SurrealDB queries *(admin only)*
- [[Admin Console]] — Higher-level admin tools
- [[Store Tasks]] — The UI layer on top of the tasks table

---

*Part of: [[0. Table of Contents]]*
