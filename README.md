# inso APB Config + Windows Optimizations
This configuration contains my own settings for **APB Reloaded**, inspired by Flaws' original config.  
It aims to optimize in-game performance and responsiveness. A script to optimize the APB executable for Windows is also provided if you wish to use it.

## `1` Installation
Drag and drop the folders into your APB Reloaded main directory and replace everything when prompted to.

For example, if you wish to install my graphics open the `Graphics` folder and drag and drop the `APBGame` folder into your own APB Reloaded main directory where your own `APBGame` folder is located but ***NOT inside `APBGame` itself!*** If Windows prompts you to replace files then you're doing it right. If not, check whether you are placing the files in the correct directory.

The only config that requires one additional step is localization because you need to add the `-language=1031` launch argument to your shortcut in case you haven't already done that.

## Launch Arguments
+ `-language=1031` - Sets the game to load with custom localization (required for localization).
+ `-nomovies` / `-nomoviesstartup` - Removes loading screens.
+ `-nosplash` - Removes the initial splash screen on boot (the GFAC logo cannot be removed).
+ `-nosteam` - Disables Steam integration, including Steam auto-login.

<details>
  <summary>Click here for an image example of launch arguments</summary>
  
![targetfield](https://i.imgur.com/o0vQdAr.png)

</details>

Example correct Target field path: <br>
`"C:\Program Files (x86)\Steam\steamapps\common\APB Reloaded\Binaries\APB.exe" -language=1031 -nomovies -nosplash`

> [!CAUTION]
> Make sure to add a space after the closing quotation mark and before each dash, as well as between each launch argument, as shown in the examples above.

## Additional Info

> [!IMPORTANT]
> Whenever a game update is released, open the default APB launcher, let it update, then close the launcher, reinstall your desired configs and launch the game from your desktop shortcut. Do **NOT** create a new APB shortcut every time there is an update — it is unnecessary. Creating a shortcut to `APB.exe` is a one-time step, you do **not** need to redo it for updates or patches.

> [!NOTE]
> To revert everything back to vanilla and start fresh, open the default APB launcher, click **Options → Repair** and let it finish. Once done, you may close the launcher and start over with modding your game.

# `2` Windows Optimization for APB Executable (Performance & Latency Optimization Toolkit)
This script applies system tweaks for **APB Reloaded** to improve performance, reduce input delay, and lower network latency.  
A simple graphical interface lets you choose which optimizations to apply. Everything is **safe**, **effective**, and **fully reversible**.

# Applying Optimizations
**Right-click** the `.ps1` file → **"Run with PowerShell"**.  
The script will automatically request administrator privileges. If you don't have permission to run PowerShell scripts, enable it first via:
```
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```
Once done, a graphical interface will open with checkboxes. Here is what each option does:

<details>
  <summary>Click here for an image example of the script (GUI interface)</summary>
  
![targetfield](https://i.imgur.com/tjbG35y.png)

</details>

| Option | What it does |
|---|---|
| **All-in-One** | Applies everything at once *(recommended)* |
| **CPU Priority** | Gives more resources to APB so it runs better |
| **Network Optimization** | Reduces ping and stabilizes the in-game connection |
| **GPU High Performance** | Sets your GPU to high performance mode for APB |
| **RunAsAdmin** | Launches APB as administrator to avoid certain issues |
| **Firewall** | Allows APB through the firewall to prevent network drops |
| **Defender Exclusion** | Prevents Windows Antivirus from slowing down the game in the background |
| **Remove all** | Removes everything and restores Windows to its previous state |

> [!IMPORTANT]
> If the game refuses to launch after applying the **RunAsAdmin** optimization, check **"Remove all optimizations"** and click Apply to revert everything.

> [!NOTE]
> To reset everything, simply check **"Remove all optimizations"** and click **Apply**.

---

<p align="center">
  <sub>©insopti — <a href="https://guns.lol/inso.vs">guns.lol/inso.vs</a></sub>
</p>
