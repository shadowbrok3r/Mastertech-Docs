---
tags:
  - mastertech
  - tab
  - shared
  - admin
  - advanced
---

# Admin Console

The Admin Console is the **admin-only control center** for Mastertech. It extends the [[Web Console]] with additional power-user tools: remote machine management, a script editor, enhanced AI capabilities, and deep per-client inspection.

> Shared tab — available in both `Mastertech.exe` and at [master-tech.app](https://master-tech.app).  
> **Requires admin privileges.** Regular users will not see this tab.

---

## Pages

The Admin Console has three main pages, switchable from the top navigation bar:

### All Clients

The primary view — shows all connected client machines (same as [[Web Console]]) but with extended admin controls:

- **Sort and filter** connected machines by name, status, or connection time
- **Undock** clients into separate viewports
- **Extended per-client interface** (see below)

### Script Editor

A code editor for creating and managing **user scripts** — custom scripts that appear in the [[Scripts]] tab's *User Scripts* category for all users.

- Write scripts with syntax highlighting
- Deploy scripts to the Scripts library
- AI-assisted generation (see below)
- Scripts are stored server-side and sync to all users

### AI Playground

An enhanced AI chat interface for admins with additional capabilities beyond the standard [[AI]] tab:
- Script generation with direct deployment to the script library
- Broader context about the connected machines
- Advanced prompting tools

---

## Per-Client Interface

Clicking any connected client in the All Clients view opens a detailed control panel for that machine. It includes multiple sub-tabs:

| Sub-tab | What it shows / does |
| ------- | -------------------- |
| **Resource Monitor** | Live CPU/RAM/GPU/network metrics for the remote machine |
| **Command Shell** | Execute PowerShell or CMD commands on the remote machine |
| **Terminal Viewer** | Live terminal output stream from the remote machine |
| **Remote Explorer** | Full remote filesystem browser — navigate, download, upload files |
| **Event Log** | Windows event log viewer for the remote machine |
| **Services** | List, start, and stop Windows services |
| **Task Scheduler** | View and manage scheduled tasks |
| **Registry** | Browse and edit the Windows registry |
| **Startup Apps** | View and manage startup programs |
| **Remote Scripts** | Run scripts from the server's script library on this machine |
| **EGUI Viewer** *(feature-gated)* | Remote egui UI rendering (advanced) |

---

## Remote Scripts

From the per-client interface → Remote Scripts sub-tab, admins can:
1. Select any script from the library (including custom user scripts)
2. Push it to run on the remote machine
3. See live output in the terminal viewer

This is the server-side counterpart to the [[Scripts]] tab that techs use locally.

---

## Use Cases

- **Remote troubleshooting** — Fix issues on a connected machine without being physically present
- **Bulk script deployment** — Push a tuneup script to multiple machines
- **Event log review** — Check for BSODs or errors on a remote machine
- **Service management** — Restart a stuck service on a remote machine
- **Script library management** — Create and publish new scripts for the team

---

## Related Tabs

- [[Web Console]] — Non-admin version of the client manager
- [[Websockets]] — Client-side connection tab
- [[Scripts]] — The user-facing script runner (scripts created here appear there)
- [[AI]] — Standard AI tab (Admin Console has enhanced version)
- [[Script Editor]] — The Admin Console's script editor page (internal)

---

*Part of: [[0. Table of Contents]]*
