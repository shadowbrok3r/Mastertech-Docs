---
tags:
  - mastertech
  - desktop-only
  - tab
---

# File Browser

The File Browser is a fully integrated file explorer built into Mastertech. It gives you access to the local machine's filesystem without needing to alt-tab to Windows Explorer — keeping everything in one window while you work.

> Desktop tab only. See [[0. Table of Contents]] or [[2. Views and Layout]] for all tabs.

---

## Layout

The File Browser is divided into three main areas:

### Top — Path Bar
Displays the current directory path. You can manually type a path and navigate to it directly.

### Center — File List
A scrollable tree of files and folders in the current directory. Folders can be **expanded** to show their contents without navigating away. Files show their name, size, and type.

### Bottom — Drives & Status
Shows available **drives** (local and removable) for quick access. Also displays:
- The currently selected **filename**
- A **progress bar** for active copy operations

---

## Key Features

### Navigation
- Click a folder to open it, or expand it inline with the tree toggle.
- Use the path bar to jump directly to any path.
- Drive buttons at the bottom let you switch to any mounted drive instantly.

### File Operations
| Action | How |
| ------ | --- |
| Copy | Select files, then use **Shift+Ctrl+C** or the copy button |
| Paste | Navigate to destination, use **Shift+Ctrl+V** or paste button |
| Rename | Right-click a file → Rename |
| New Folder | Right-click in directory → New Folder |
| Delete | Right-click a file → Delete |

### Partial Folder Copy
One of the most useful features compared to standard Windows Explorer: you can copy **some but not all** files from a folder. Select exactly what you want and copy — this is a fast alternative to Robocopy for selective transfers.

### Progress Tracking
Active file copy operations show a **progress bar** at the bottom of the window so you can see how far along large transfers are without any additional tools.

---

## Detachable Window

The File Browser can be **detached into its own floating window** so it remains visible while you work in other tabs:

- Right-click the **File Browser** tab → *Detach File Browser*
- To reattach: right-click the same tab context menu → *Attach File Browser*

This is especially handy when copying files while also filling out a [[3. TUR Sheet|TUR Sheet]].

---

## Default Layout

The File Browser is docked to the **left side** of the screen by default when Mastertech first opens. You can move it anywhere using the [[2. Views and Layout|docking system]].

---

## Related Tabs

- [[Scripts]] — Run automated file operations like Robocopy from the Scripts tab
- [[3. TUR Sheet]] — Fill out TUR while copying files side-by-side
- [[Websockets]] — Remote file access via the WebSocket console
- [[Web Console]] — Remote file explorer for connected machines

---

*Part of: [[4. Task Boards|Desktop Workflow]] | [[0. Table of Contents]]*
