---
tags:
  - mastertech
  - desktop-only
  - tab
  - windows
---

# Scripts

The Scripts tab is a powerful Windows automation hub. It provides a categorized library of one-click scripts you can queue and run against the current machine — from full tuneup workflows to individual junkware removal tools.

> Desktop tab only (Windows). See [[0. Table of Contents]] or [[2. Views and Layout]] for all tabs.

---

## Layout

The Scripts tab has a three-column layout:

| Column | Purpose |
| ------ | ------- |
| **Left — Categories** | Browse script categories and select scripts to add to the queue |
| **Center — Queue** | Scripts queued to run, with status indicators |
| **Right — Logs** | Live output log from running scripts |

---

## Script Categories

### 🔧 Tuneup / QC

Standard tuneup and quality-check scripts run on customer machines:

| Script | What it does |
| ------ | ------------ |
| **Data Transfer** | Opens the data transfer workflow (see below) |
| **Activate CPS** | Activates CPS software |
| **Activate SEB** | Activates SecureAnywhere Backup |
| **Install Windows Updates** | Triggers Windows Update via PowerShell |
| **Disable Sleep / Hibernation** | Turns off sleep and hibernation |
| **Run SuperAntiSpyware Scan** | Launches an SAS scan |
| **Run Webroot Scan** | Launches a Webroot scan |
| **Run Junkware Category** | Queues all junkware removal scripts |
| **Run Tron** | Runs the Tron batch script |
| **Install LibreOffice** | Downloads and installs LibreOffice |
| **Disable proxy settings** | Clears Windows proxy configuration |
| **Disable Notifications** | Turns off Windows notification banners |
| **Change SuperAntiSpyware settings** | Applies recommended SAS scan settings |
| **Disable Startup Apps** | Disables common unnecessary startup programs |
| **Unpin Copilot** | Removes the Copilot button from the taskbar |
| **Align Taskbar to left** | Moves the taskbar start button to the left (Windows 11) |

### ℹ Informational

Quick checks that report on the current machine's state without making changes:

| Script | What it reports |
| ------ | --------------- |
| **Is SuperEasyBackup installed?** | Checks for SEB installation |
| **Is Webroot installed?** | Checks for Webroot installation |
| **Is SuperAntiSpyware installed?** | Checks for SAS installation |
| **Are there scheduled tasks for it?** | Lists scheduled tasks related to AV |
| **Is Windows Activated?** | Reports Windows activation status |
| **Is Hibernation/Sleep enabled?** | Reports power plan sleep settings |
| **Any Recent Blue Screens?** | Scans event log for recent BSODs |
| **When Was The Last Service Date?** | Reports last PC Laptops service date |
| **Windows Version** | Reports current Windows build |
| **Check Updates** | Reports pending Windows updates |
| **Run Prechecks** | Runs all informational checks at once |

### 🗑 Junkware Removal

Removes common bloatware and unwanted software:

- **OneLaunch**
- **WebNavigator Browser**
- **Wave Browser**
- **Clear Browser**
- **Shift Browser**
- **Avast Browser**
- **McAfee Safe**
- **Driver Support**
- **Winzip**

### 📜 User Scripts

Custom scripts created by users in the [[Script Editor]] (Admin feature). These appear per-user and can be shared across the team.

---

## Script Queue

Scripts are not run immediately when selected — they're added to the **Queue** first. This lets you build a batch of scripts to run in sequence.

- **Add** a script by clicking its name in the category list
- **Remove** individual scripts from the queue
- **Run Queue** executes all queued scripts in order
- Each script shows its status: **Pending** → **Running** → **Completed** / **Failed**

---

## Log Output

The right panel shows a **live log** of everything happening as scripts execute:

- Color-coded by severity: info (white), success (green), warning (yellow), error (red)
- **Auto-scroll** keeps the log at the bottom as new entries arrive (can be toggled)
- Useful for debugging script failures or confirming steps completed

---

## Data Transfer

Selecting **Data Transfer** from the queue opens a dedicated overlay for moving customer files:

1. Mastertech scans for common data locations (Desktop, Documents, Pictures, Downloads, etc.) on the machine
2. You select which folders/paths to include as **sources**
3. You select a **destination** (external drive, network path, etc.)
4. Robocopy runs in the background and reports progress to the log

Progress for active transfers is shown in a **progress bar** at the top of the interface.

---

## Related Tabs

- [[File Browser]] — Manual file copying; alternative to the Data Transfer script
- [[System Information]] — Hardware context for what you're tuning up
- [[3. TUR Sheet]] — The service number input in Scripts links to ticket data (keys, email)
- [[Admin Console]] → [[Script Editor]] — Create and manage custom user scripts
- [[Logs]] — Full application logs including script run history

---

*Part of: [[0. Table of Contents]]*
