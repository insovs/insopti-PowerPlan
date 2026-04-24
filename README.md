<div align="center">

[![Discord](https://img.shields.io/badge/Support-Discord-5865F2?logo=discord&logoColor=white)](https://discord.com/invite/fayeECjdtb)
[![Preview](https://img.shields.io/badge/Video-Preview-FF0000?logo=youtube&logoColor=white)](https://youtu.be/JIATuKskBmk)

<img width="1983" height="793" alt="image" src="https://github.com/user-attachments/assets/7cb13fec-27de-4d26-922e-d7a90b5e8d07" />

</div>

# 🚀 Overview

Imports and activates a custom **PowerPlan** to maximize performance, system responsiveness and minimize latency.<br>
Automatically downloads the `.pow`, imports it into Windows, and activates it.<br>
Everything is **safe**, **optimized**, and **fully reversible**.

<details>
<summary><b>👁️ Show Preview Tool</b></summary>
<img width="761" height="370" alt="68747470733a2f2f696d6775722e636f6d2f314a4e6d5a78562e706e67" src="https://github.com/user-attachments/assets/3fe3762d-984e-4bac-9a40-30554d1c729a" />
<img width="766" height="383" alt="68747470733a2f2f696d6775722e636f6d2f413355684a4f722e706e67" src="https://github.com/user-attachments/assets/e122a170-b467-42e4-88bc-8f348634658b" />
<img width="758" height="713" alt="68747470733a2f2f696d6775722e636f6d2f6348336842505a2e706e67" src="https://github.com/user-attachments/assets/08a1fc34-9a8c-4276-a314-96982ca42550" />
</details>

---

## 📥 Usage / Instalation

Head to the **[Releases](https://github.com/insovs/insopti-PowerPlan/releases)** section and download `insopti-PowerPlan.ps1`, then **right-click** it → **Run with PowerShell**

The script will automatically request administrator privileges, then prompt you to select the profile suited to your CPU configuration.

> [!CAUTION]
> If PowerShell scripts are blocked on your system, enable execution first:
> ```powershell
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
> ```
> Or use **[EnablePowerShellScript](https://github.com/insovs/EnablePowerShellScript)** for a one-click solution.

---

## Plan selection

| Option | Description |
|---|---|
| **`1` Static OC mode** | For users with a manually fixed CPU frequency (OC) and Precision Boost disabled |
| **`2` Dynamic boost mode** | For all other users with Precision Boost / Turbo enabled (default in BIOS) |

> [!IMPORTANT]
> If you are unsure which to pick, go with **Dynamic boost mode** (`2`). It is the default setting for most configurations.

---

## What the script does

| Optimization | Description |
|---|---|
| **PowerPlan Import** | Downloads and imports the `insopti` power plan into Windows |
| **Auto Activation** | Activates the plan immediately after import |
| **CPU no-throttle** | Disables CPU frequency throttling and latency mitigation features |
| **CPU Unparking** | Unlocks all CPU cores, no core is put to sleep by Windows |
| **USB Power Management** | Optimizes USB power management to reduce input delay |
| **Sleep state settings** | Configures sleep states for maximum responsiveness |

---

## Uninstall / Reset

To revert to the default Windows power plan:

1. Open **Control Panel** → **Power Options**
2. Select a native Windows plan (Balanced, High performance, etc.)
3. Delete the `insopti` plan from the list if you wish to remove it completely

> [!NOTE]
> The script does not modify any permanent system files. Switching power plans is enough to revert everything. No benchmarks are provided as results vary depending on BIOS settings, hardware configuration, and overall system tuning — feel free to run your own and share your results.

---

> [!IMPORTANT]
> This plan is designed for **desktop use plugged into mains power**. Using it on a laptop running on battery is not recommended as it maximizes power consumption at all times.

---

<div align="center">
  <sub>©insopti — <a href="https://guns.lol/inso.vs">guns.lol/inso.vs</a> · For personal use only.</sub>
</div>
