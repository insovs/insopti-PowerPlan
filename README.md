<h1 align="left"><code style="color:#4A9EFF">insopti PowerPlan</code></h1>

This script imports and activates my custom power plan **insopti PowerPlan**, designed to maximize system responsiveness and minimize latency. It automatically downloads the `.pow` configuration file from GitHub, imports it into Windows, and activates it. Everything is **safe**, **optimized**, and **fully reversible**.

# `1` Installation & Launch
**Right-click** the `.ps1` file → **"Run with PowerShell"**.  
The script will automatically request administrator privileges.

> [!CAUTION]
> If you don't have permission to run PowerShell scripts, enable it first via:
> ```
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
> ```

Once launched, the script will prompt you to choose the profile that matches your CPU configuration.

# Plan Selection
| Option | Description |
|---|---|
| **`1` Static OC mode** | For users with a manually fixed CPU frequency and Precision Boost disabled |
| **`2` Dynamic boost mode** | For all other users with Precision Boost / Turbo enabled (default in BIOS) |

> [!IMPORTANT]
> If you're unsure which to choose, go with **Dynamic boost mode** (`2`). This is the default setting for the majority of configurations.

# `2` What the script does
| Optimization | What it does |
|---|---|
| **PowerPlan Import** | Downloads and imports the `insopti` power plan into Windows |
| **Auto Activation** | Activates the plan immediately after import |
| **CPU no-throttle** | Disables CPU frequency throttling and latency mitigation functions |
| **CPU Unparking** | Unlocks all CPU cores (like ParkControl) — no core is put to sleep by Windows |
| **USB Power Management** | Optimizes USB power management to reduce input delay |
| **Sleep state settings** | Configures sleep states for maximum responsiveness |

> [!NOTE]
> The script does not modify any permanent system files. Switching back to another power plan is enough to revert everything.

# Additional Info
> [!IMPORTANT]
> This plan is designed for **desktop use plugged into a wall outlet**. Using it on a laptop running on battery is not necessarily recommended, as it maximizes power consumption at all times.

# `3` Preview & Results
The screenshots below show the **insopti PowerPlan as it appears in Windows**, as well as the **target field configuration** to verify the plan has been correctly applied and is active on your system.

![preview](https://imgur.com/1JNmZxV.png)
<details>
  <summary>Click here to show the next steps</summary>
  
![targetfield](https://imgur.com/A3UhJOr.png)
![targetfield](https://imgur.com/cH3hBPZ.png)
</details>
<p align="center">
  <sub>©insopti — <a href="https://guns.lol/inso.vs">guns.lol/inso.vs</a> | For personal use only.</sub>
</p>
