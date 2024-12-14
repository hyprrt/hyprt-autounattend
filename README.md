# hyprt-autounattend
My custom autounattend file with tweaks for Windows 11 for a more pleasant experience overall.

# What tweaks?
## OOBE and Windows installer tweaks:
- Bypass Windows 11 requirements (TPM, Secure Boot, etc.)
- Allow Windows 11 to be installed without a network connection (runs OOBE\BYPASSNRO automatically)
- Uses a generic product key, and skips EULA and goes straight to partition setup in the installer.
- Defaults to local account creation during OOBE.
- Prevents automatic device encryption on a fresh install.
- Disables all express settings by default in OOBE.
- Removes all Windows 11 tiles by default after a fresh install.

## Windows 11 tweaks:
- Removes preset icons from the taskbar. (MS Edge, MS Store, Explorer, etc.)
- Icon only search in taskbar by default. (Can be changed of course, it just looks cleaner to me that way.)
- Always show file extensions in Explorer.
- Disables widgets entirely.
- Uses classic context menu.
- Left-aligned taskbar.
- Sets startup page of Windows 11 to "This PC" from "Home".
- Disables Bing in search.
- Disables fast startup.
- Allows execution of PowerShell scripts by default.
- Disables last access time stamp updates in NTFS.
- Prevents Windows Update from doing automatic reboots.
- Disables app suggestions/Content delivery manager.
- Disables Edge's first run experience. (Might show "This browser is managed by your organization" but it's pretty harmless and should be ignored.)
- Disables "Enhance Pointer Precision" mouse setting.

## Removed Windows 11 apps:
- All the apps with a ✅ are removed.
![brave_Llgc3QIQFR](https://github.com/user-attachments/assets/2c70a23e-b21e-4f10-9381-0a4650eeb8c1)

# Windows Defender:
- Use autounattend-no-defender.xml if you also want Defender gone after a fresh Windows install.
- Otherwise stick to the regular autounattend if you want to continue using Windows Defender.

# How do I use it?:
- Couldn't find anything better than [memstechtips's guide on the same.](https://github.com/memstechtips/UnattendedWinstall?tab=readme-ov-file#old-methods)

# What is autounattend-hyprt.xml?
- It's same as the regular autounattend with the only difference being that it sets the computer name to "devs11" after a fresh install. It is really only for my personal use.

# Who is this intended for?
- It's intended for intermediate-advanced users and it enables quite for risky stuff like automatically enabling PowerShell scripts, etc.
- It's intended for people who know what they are doing and are aware of the modifications this autounattend script can do.
- It's intended for people who are willing to go out of their comfort zone to make an overall more pleasant Windows experience for them.<br><br>

**IT IS NOT A HEAVY MODIFICATION TO WINDOWS! It's exactly identical to a fresh Windows 11 install. Comparing it to AtlasOS, ReviOS, Ghost Spectre or memstechtips' UnattendedWinstall doesn't do it justice. It's a bunch of small modifications and registry tweaks to Windows. Each and every thing can be restored to default after the installation and it does not break anything at all.** <br><br>

**Use at your own risk. I am not responsible for any damage caused.** <br>
**I will look out for updates and changes to Windows and try to update it, if it causes anything to break, please make an issue about it.** <br><br>

**I was able to achieve this using [schneegans.de's autounattend.xml generator](https://schneegans.de/windows/unattend-generator/). I just saved some of your time by making a boilerplate or a generic config for you to use by compiling settings and configs that most would have done anyway. If it works for you, great, otherwise feel free to import it on the website and make your modifications.** <br><br>

This project was greatly inspired by memstechtips' UnattendedWinstall script. I would highly recommend you check it out too [UnattendedWinstall](https://github.com/memstechtips/UnattendedWinstall). It has more heavier modications to Windows and a lot of changes to it. If you want something with only a small amount of changes on a stock Windows 11 install, I would still recommend you use my xml since his script is for advanced users.
