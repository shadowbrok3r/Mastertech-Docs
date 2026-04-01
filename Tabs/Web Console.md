---
tags:
  - mastertech
  - tab
  - shared
  - admin
---

# Web Console

The Web Console is a **remote client manager** — it shows all Mastertech instances that are currently connected to MtechServer via WebSocket. From the Web Console you can interact with remote machines: browse their files, open a shell, run scripts, and more.

> Shared tab — available in both `Mastertech.exe` and at [master-tech.app](https://master-tech.app).  
> For the admin-enhanced version with script editing and enhanced AI, see [[Admin Console]].

---

## What It Shows

The Web Console displays a grid or list of all **connected client machines**. Each client card shows:
- **Client name** (set by the tech when they connected via [[Websockets]])
- **IP / location**
- **Connection status**
- Quick action buttons

---

## View Modes

### Grid View
Client cards shown in a grid layout — good for scanning many connections at once.

### List View
Clients shown as a detailed list — more information per row.

---

## Per-Client Actions

Click any connected client to open its **detail view**, which has two main modes:

### Shell
A command-line interface for executing commands on the remote machine. Run PowerShell commands, check system state, or script quick fixes without physically touching the machine.

### File Explorer
A remote file browser showing the client machine's filesystem. Browse, download, and upload files directly between the server and the remote machine.

---

## TUR Integration

From the Web Console you can open a **TUR modal** for a connected client — pre-filling the TUR Sheet with data from the remote machine so you can submit a TUR without being physically at that computer.

---

## Connection Manager

Manage WebSocket connections from the Web Console — view connection health, disconnect stale sessions, and see how long each machine has been connected.

---

## Related Tabs

- [[Websockets]] — The client-side tab that initiates the connection
- [[Admin Console]] — Admin-enhanced version with script editor and enhanced AI
- [[Scripts]] — Remote script deployment via the WebSocket connection
- [[3. TUR Sheet]] — TUR modal pre-fills from remote machine data

---

*Part of: [[0. Table of Contents]]*
