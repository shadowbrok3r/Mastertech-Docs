---
tags:
  - mastertech
  - tab
  - shared
  - admin
  - advanced
---

# Query Editor

The Query Editor is a **raw SurrealDB query interface** for running ad-hoc queries against the Mastertech database. It's the developer/power-user tool for reading and writing data directly with SurrealQL.

> Shared tab — available in both `Mastertech.exe` and at [master-tech.app](https://master-tech.app).  
> **Admin only.** This tab is only accessible when logged in with admin credentials.

---

## Layout

### Bottom — Editor

A code editor for writing SurrealQL queries. Supports multi-line input with basic syntax editing.

### Center — Response

The query result is displayed as formatted JSON in the response panel. Results update after each query execution.

---

## Running Queries

1. Type a SurrealQL query in the editor panel
2. Press **Execute** (or the keyboard shortcut)
3. View the JSON response above

### Example Queries

```sql
-- Get all open tasks for a store
SELECT * FROM tasks WHERE store = "store_name" AND status != "complete";

-- Find a user by email
SELECT * FROM users WHERE email = "brett.knowlton@pclaptops.com";

-- Count tasks created today
SELECT count() FROM tasks WHERE created_at > time::now() - 1d;
```

---

## SurrealDB Resources

SurrealDB uses SurrealQL — a SQL-like query language with graph and document capabilities. Key concepts:

- Tables are like SQL tables but store JSON documents
- `SELECT * FROM table` — basic select
- `WHERE` clauses work like SQL
- `CREATE`, `UPDATE`, `DELETE` for writes
- `RELATE` for graph relationships

Refer to the [SurrealDB documentation](https://surrealdb.com/docs) for full SurrealQL reference.

---

## ⚠️ Caution

Queries run here execute **directly against the production database**. `UPDATE` and `DELETE` statements have immediate, irreversible effects. Always test with `SELECT` before running writes.

---

## Related Tabs

- [[Database Editor]] — Table-based UI for browsing records (safer for non-query users)
- [[Admin Console]] — Other admin tools
- [[Logs]] — Check logs if queries fail or behave unexpectedly

---

*Part of: [[0. Table of Contents]]*
