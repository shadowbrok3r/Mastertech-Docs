---
tags:
  - mastertech
  - desktop-only
  - tab
  - advanced
---

# Websockets

The Websockets tab is a direct WebSocket client console built into Mastertech. It lets the desktop app connect to a running MtechServer WebSocket endpoint — enabling remote command execution, file transfers, and real-time communication with a remote machine.

> Desktop tab only. For the server-side admin view of connected clients, see [[Web Console]] and [[Admin Console]].

---

## Overview

When Mastertech is running on a **customer's machine** (or any remote machine), it can connect back to MtechServer and become a **managed client**. The Websockets tab is the interface for that connection on the local machine.

Once connected, the local machine becomes visible in [[Admin Console]] and [[Web Console]] on the server side — enabling admins and techs to:
- Execute remote commands
- Browse the remote filesystem
- Transfer files
- Monitor resources
- Run scripts remotely

---

## Layout

### Top Bar
- **Client Name** — Set a display name for this connection (how it appears in the admin view)
- **Connect / Disconnect** button — Establishes or drops the WebSocket connection

### Center — Message History

A chat-style panel showing the history of WebSocket messages exchanged. This includes:
- Commands sent to this client
- Responses and outputs
- File transfer events
- Binary protocol messages (`Cmd` enum payloads)

### Input

Send raw messages or commands to the server from this field.

---

## Supported Commands

The Websockets console communicates via a binary `Cmd` protocol that supports:

| Command type | What it does |
| ------------ | ------------ |
| **Filesystem** | Browse, read, write files on this machine |
| **Shell** | Execute shell commands |
| **File transfer** | Send/receive files to/from the server |
| **Plugins** | Load and run WASM plugins |
| **MCP proxy** | Forward MCP tool calls to this machine |
| **Frame capture** | Capture screen frames |
| **Processes** | List and manage running processes |
| **Event log** | Read Windows event log |
| **Services** | List/start/stop Windows services |
| **Scheduled tasks** | View scheduled tasks |
| **Registry** | Read/write registry keys |
| **Startup apps** | View/manage startup programs |
| **Remote scripts** | Run scripts pushed from the server |

---

## Detachable Window

The Websockets console can be **detached into its own floating window**:
- Right-click the **Websockets** tab → *Detach Websocket Console*
- Reattach: *Attach Websocket Console*

This keeps the WebSocket console visible while you work in other tabs.

---

## Related Tabs

- [[Web Console]] — Server-side view of all connected clients (including this machine)
- [[Admin Console]] — Admin control center for managing connected machines
- [[File Browser]] — Local file access; Websockets enables remote file access
- [[Scripts]] — Scripts can be run remotely via Websockets from the admin side

---

*Part of: [[0. Table of Contents]]*
