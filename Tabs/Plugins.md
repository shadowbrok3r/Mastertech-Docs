---
tags:
  - mastertech
  - tab
  - shared
  - advanced
---

# Plugins

The Plugins tab is a **WASM (WebAssembly) plugin manager** for Mastertech. It lets you enable, disable, and manage plugins that extend Mastertech's functionality — adding new tools, automations, or integrations beyond the built-in features.

> Desktop tab only (native). On the web, this tab shows a placeholder message.  
> See [[0. Table of Contents]] or [[2. Views and Layout]] for all tabs.

---

## What Are Plugins?

Plugins are small programs compiled to WebAssembly (`.wasm`) that run inside Mastertech. Because they're sandboxed WASM modules, they can be safely loaded and unloaded without affecting the rest of the app.

Plugins can:
- Add new UI elements or tool panels
- Automate tasks
- Connect to external services
- Extend the Scripts library

---

## MCP Integration

The Plugins tab includes an **MCP (Model Context Protocol)** section that shows available MCP tools. MCP tools are a standardized way for AI models to interact with external services and data sources. Plugins can expose MCP tool endpoints that the [[AI]] tab or [[Admin Console]] AI can call.

The MCP section is collapsible and shows:
- Registered MCP tools and their descriptions
- Enable/disable toggles per tool

---

## Managing Plugins

| Action | How |
| ------ | --- |
| **Enable** a plugin | Toggle it on in the list |
| **Disable** a plugin | Toggle it off |
| **View details** | Click the plugin name for description and version |

---

## Related Tabs

- [[AI]] — AI features can use plugins via MCP tool calls
- [[Admin Console]] — Plugin deployment to remote machines via WebSocket
- [[Websockets]] — Remote plugin loading via the `Cmd` protocol

---

*Part of: [[0. Table of Contents]]*
