# insopti PowerPlan Windows
Imports and activates a **PowerPlan**, designed to maximize performance, system responsiveness and minimize latency.

It automatically downloads the `.pow`, imports it into Windows, and activates it. Everything is **safe**, **optimized**, and **fully reversible**.  


> [!NOTE]
> Not sure what it does? Check the **[video preview](https://youtu.be/JIATuKskBmk)** to see it in action. the whole process takes under 10 seconds.

![preview](https://imgur.com/1JNmZxV.png)
<details>
  <summary>Click here to show the next steps</summary>
  
![targetfield](https://imgur.com/A3UhJOr.png)
![targetfield](https://imgur.com/cH3hBPZ.png)
</details>

## Installation & Launch
Head to the **[Releases](https://github.com/insovs/insopti-PowerPlan/releases)** section and download `insopti-PowerPlan.ps1`, then **right-click** it → **"Run with PowerShell"**.  
The script will automatically request administrator privileges.

> [!CAUTION]
> If you are not allowed to run PowerShell scripts, enable it first:
> ```
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
> ```
or refer to [EnablePowerShellScript](https://github.com/insovs/EnablePowerShellScript).  
Once launched, the script will prompt you to select the profile suited to your CPU configuration.

## Plan selection

| Option | Description |
|---|---|
| **`1` Static OC mode** | For users with a manually fixed CPU frequency (OC) and Precision Boost disabled |
| **`2` Dynamic boost mode** | For all other users with Precision Boost / Turbo enabled (default in BIOS) |

> [!IMPORTANT]
> If you are unsure which to pick, go with **Dynamic boost mode** (`2`). It is the default setting for most configurations.

## What the script does

| Optimization | What it does |
|---|---|
| **PowerPlan Import** | Downloads and imports the `insopti` power plan into Windows |
| **Auto Activation** | Activates the plan immediately after import |
| **CPU no-throttle** | Disables CPU frequency throttling and latency mitigation features |
| **CPU Unparking** | Unlocks all CPU cores, no core is put to sleep by Windows |
| **USB Power Management** | Optimizes USB power management to reduce input delay |
| **Sleep state settings** | Configures sleep states for maximum responsiveness |

## Additional info

> [!IMPORTANT]
> This plan is designed for **desktop use plugged into mains power**.
>   Using it on a laptop running on battery is not recommended as it maximizes power consumption at all times.

## Uninstall / Reset

To revert to the default Windows power plan:

1. Open **Control Panel** → **Power Options**.
2. Select a native Windows plan (Normal, Balanced, High performance, etc.).
3. Delete the `insopti` plan from the list if you wish to remove it completely.

> [!NOTE]
> No benchmarks are provided, as results vary depending on multiple factors like BIOS settings, hardware configuration, and overall system tuning. On my end, most optimizations were already applied at the BIOS level prior to using this plan, so the difference may be minimal if your system is already well configured, or significant if it is not. That said, feel free to run your own benchmarks and share your results — feedback is always welcome !

> The script does not modify any permanent system files. Switching power plans is enough to revert everything.

---

<p align="center">
  <sub>©insopti — <a href="https://guns.lol/inso.vs">guns.lol/inso.vs</a> | For personal use only.</sub>
</p>
