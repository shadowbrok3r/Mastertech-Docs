---
tags:
  - mastertech
  - desktop-only
  - tab
  - windows
  - advanced
---

# Minidump Analysis

The Minidump Analysis tab is a Windows crash dump analyzer built directly into Mastertech. It lets you load `.dmp` files from the machine and get a symbolicated stack trace — the same kind of analysis you'd normally need WinDbg or an online symbolication service to produce.

> Desktop tab only — Windows only. See [[0. Table of Contents]] or [[2. Views and Layout]] for all tabs.

---

## What Is a Minidump?

When Windows crashes (Blue Screen of Death / BSOD), it typically writes a crash dump file to disk at:

```
C:\Windows\Minidump\
```

These `.dmp` files contain a snapshot of what was happening at the time of the crash — including the call stack, loaded modules, and processor state. Analyzing them tells you *why* the machine crashed.

---

## Sub-tabs

The Minidump Analysis tab has four internal views selectable from a tab bar:

### Settings

Configure the analysis options:
- **Symbol path** — Path to `.pdb` symbol files or a symbol server URL (e.g., Microsoft's public symbol server)
- **Minidump file** — Select or browse to the `.dmp` file you want to analyze

### Raw Dump

Displays the **raw byte streams** from the dump file — useful for lower-level inspection of the dump structure before symbolication.

### Processed

The main output view: the **symbolicated stack trace**. After loading a dump and clicking to process, this shows:
- The exception that caused the crash
- The full call stack with module names and (where symbols are available) function names and line numbers
- The faulting driver or module

This is the most useful view for diagnosing BSODs and reporting to the customer.

### Logs

Shows the processing log output — progress of symbol resolution, errors loading symbol files, and any warnings from the dump processor.

---

## How to Use

1. Open the **Settings** sub-tab
2. Browse to the `.dmp` file (usually from `C:\Windows\Minidump\`)
3. Optionally set a symbol server path (Microsoft's public server: `https://msdl.microsoft.com/download/symbols`)
4. Click **Analyze** / **Process**
5. Switch to the **Processed** sub-tab to read the results
6. Check **Logs** if there are any errors

---

## Common Findings

| Pattern | Likely cause |
| ------- | ------------ |
| `ntfs.sys` in the stack | File system / drive corruption |
| Third-party AV driver | AV software causing a crash |
| `nvlddmkm.sys` | NVIDIA driver crash |
| `memory_management` | RAM issue (run MemTest) |
| `page_fault_in_nonpaged_area` | Bad RAM or failing driver |

Use the crash findings to inform the [[3. TUR Sheet|TUR Sheet]] recommendations — BSOD history is a major selling point for upgrades.

---

## Related Tabs

- [[System Information]] — Hardware specs for context when interpreting dumps
- [[Scripts]] → *Any Recent Blue Screens?* — Quick check for BSOD history in event log
- [[3. TUR Sheet]] — Document crash findings in recommendations
- [[Resource Monitor]] — Check if the machine is currently showing warning signs

---

*Part of: [[0. Table of Contents]]*
