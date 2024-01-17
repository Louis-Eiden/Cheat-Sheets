# Windows Cheat Sheet

A Cheat Sheet for Windows 10

## Table of Contents

- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Run Commands](#run-commands)
- [Folder Shortcuts](#folder-shortcuts)
- [CMD Commands](#cmd-commands)
- [PowerShell Commands](#powershell-commands)
- [Windows Terminal](#windows-terminal)
- [Tools](#tools)
  - [Chocolatey](#chocolatey)
  - [Windows Subsystem for Linux](#windows-subsystem-for-linux)
  - [PowerToys](#powertoys)
  - [X-Mouse Controls](#x-mouse-controls)
  - [ZoomIt](#zoomit)
  - [Windows Sysinternals](#windows-sysinternals)
- [Tricks and Tips](#tricks-and-tips)
  - [Open Command Prompt from File Explorer](#open-command-prompt-from-file-explorer)
  - [Open PowerShell from File Explorer](#open-powershell-from-file-explorer)
  - [Open WSL Linux Shell from File Explore](#open-wsl-linux-shell-from-file-explore)
  - [Windows 10 God Mode](#windows-10-god-mode)
  - [Windows 10 Secret Start Menu](#windows-10-secret-start-menu)
  - [Windows 10 Secret Screen Recorder](#windows-10-secret-screen-recorder)
  - [show windows keys](#show-windows-keys)
  - [Speed up Windows 10](#speed-up-windows-10)
- [Fixes](#fixes)
  - [Fix blurry apps](#fix-blurry-apps)
  - [Restart Graphics Driver](#restart-graphics-driver)
  - [Fix Windows Update](#fix-windows-update)
  - [Scan and repair system files](#scan-and-repair-system-files)
  - [Reset Windows Update Components](#reset-windows-update-components)
  - [System Restore](#system-restore)
  - [Manual System Restore](#manual-system-restore)

#

## Keyboard Shortcuts

| Shortcut                                      | Description                                                                |
| --------------------------------------------- | -------------------------------------------------------------------------- |
| `Windows Key`                                 | Open Start Menu                                                            |
| `Windows Key + A`                             | Open Action Center                                                         |
| Windows Key + B                               | Highlight the notification area                                            |
| Windows Key + C                               | Open Cortana in listening mode                                             |
| **<u>Windows Key + D**                        | Display and hide the desktop                                               |
| **<u>Windows Key + E**                        | Open File Explorer                                                         |
| Windows Key + F                               | Open Feedback Hub                                                          |
| **<u>Windows Key + G**                        | Open Game bar when a game is open                                          |
| Windows Key + H                               | Open the Share charm                                                       |
| Windows Key + I                               | Open Settings                                                              |
| Windows Key + J                               | Set focus to a Windows tip                                                 |
| **<u>Windows Key + K**                        | Open the Connect quick action                                              |
| Windows Key + L                               | Lock your PC or switch accounts                                            |
| Windows Key + M                               | Minimize all windows                                                       |
| Windows Key + Shift + M                       | Restore minimized windows on the desktop                                   |
| Windows Key + O                               | Lock device orientation                                                    |
| Windows Key + P                               | Choose a presentation display mode                                         |
| Windows Key + Q                               | Open Cortana in typing mode                                                |
| **<u>Windows Key + R**                        | Open Run dialog box                                                        |
| Windows Key + S                               | Open search                                                                |
| **<u>Windows Key + T**                        | Cycle through apps on the taskbar                                          |
| Windows Key + U                               | Open Ease of Access Center                                                 |
| **<u>Windows Key + V**                        | Show Clipboard History                                                     |
| **<u>Windows Key + X**                        | Open the Quick Link menu                                                   |
| Windows Key + Z                               | Show the commands available in an app                                      |
| **<u>Windows Key + 1-9**                      | Open the app pinned to the taskbar in the position indicated by the number |
| Windows Key + ,                               | Temporarily peek at the desktop                                            |
| Windows Key + .                               | Snap a window to a quadrant of the screen                                  |
| Windows Key + Spacebar                        | Switch input language and keyboard layout                                  |
| **<u>Windows Key + Tab**                      | Open Task view                                                             |
| Windows Key + Esc                             | Close Task view                                                            |
| **<u>Windows Key + Left/Right arrow**         | Snap app windows Left/Right                                                |
| **<u>Windows Key + Up/Down arrow**            | Maximize/Minimize app windows                                              |
| **<u>Windows Key + Shift + Up arrow**         | Stretch the desktop window to the top and bottom of the screen             |
| **<u>Windows Key + Shift + Down arrow**       | Restore/minimize active desktop windows vertically, maintaining width      |
| **<u>Windows Key + Shift + Left/Right arrow** | With multiple monitors, move the active window to other monitor            |
| **<u>Windows Key + Ctrl + Left/Right arrow**  | Switch between virtual desktops                                            |
| Windows Key + Ctrl + D                        | Add a virtual desktop                                                      |
| Windows Key + Ctrl + F4                       | Close current virtual desktop                                              |
| Windows Key + Ctrl + F                        | Search for PCs (if you're on a network)                                    |

#

## Run Commands [source&nearr;]()

#### Run a command - Windows Key + R

#### Run a command as Administrator - Windows Key + R, then press Ctrl + Shift + Enter

| Command        | Description                 |
| -------------- | --------------------------- |
| `cmd`          | Open Command Prompt         |
| `powershell`   | Open Windows PowerShell     |
| `taskmgr`      | Open Settings               |
| `control`      | Open Control Panel          |
| `msconfig`     | Open System Configuration   |
| `devmgmt.msc`  | Open Device Manager         |
| `diskmgmt.msc` | Open Disk Management        |
| `eventvwr.msc` | Open Event Viewer           |
| `appwiz.cpl`   | Open Programs and Features  |
| `sysdm.cpl`    | Open System Properties      |
| `msinfo32`     | Open System Information     |
| `regedit`      | Open Registry Editor        |
| `resmon`       | Open Resource Monitor       |
| `perfmon`      | Open Performance Monitor    |
| `lusrmgr.msc`  | Open Local Users and Groups |
| `secpol.msc`   | Open Local Security Policy  |
| `gpedit.msc`   | Open Group Policy Editor    |
| `compmgmt.msc` | Open Computer Management    |
| `ncpa.cpl`     | Open Network Connections    |
| `powershell`   | Open Windows PowerShell     |
| `documents`    | Open Documents folder       |
| `downloads`    | Open Downloads folder       |

#

## Folder Shortcuts

#### - Open via Run dialog box - Windows Key + R, then type shortcut name

#### - Open via File Explorer - Ctrl + l, then type shortcut name

#### - Open via Command Prompt - cd shortcut name

| Shortcut                  | Description                      |
| ------------------------- | -------------------------------- |
| `%windir%`                | Go to Windows folder             |
| `%userprofile%`           | Go to User folder                |
| `%systemroot%\system32`   | Go to System32 folder            |
| `%programfiles%`          | Go to Program Files folder       |
| `%programfiles(x86)%`     | Go to Program Files (x86) folder |
| `%appdata%`               | Go to AppData folder             |
| `%localappdata%`          | Go to LocalAppData folder        |
| `%temp%`                  | Go to Temp folder                |
| `%tmp%`                   | Go to Temp folder                |
| `%public%`                | Go to Public folder              |
| `%userprofile%\desktop`   | Go to Desktop folder             |
| `%userprofile%\documents` | Go to Documents folder           |

## CMD Commands [source&nearr;](https://ss64.com/nt/)

#### - Open via Run dialog box - Windows Key + R, then type cmd

#### - Open via File Explorer - Ctrl + l, then type cmd

#### - Open via File Explorer - Shift + Right-click on a folder, then choose Open command window here

#### - Drag and drop a folder into the command window to type the path

| Command       | Description                                      |
| ------------- | ------------------------------------------------ |
| `F7`          | Display command history                          |
| `F1`          | Copy previous command                            |
| `\| clip`     | Copy command output to clipboard                 |
| `>`           | Redirect command output to file                  |
| `&&`          | Run multiple commands on one line if previous ok |
| `&`           | Run multiple commands on one line                |
| `^`           | Escape character                                 |
| `\|\|`        | Run command if previous command fails            |
| `/?`          | Help                                             |
| `cls`         | Clear Screen                                     |
| `cd`          | Change Directory                                 |
| `cd ..`       | Change Directory to parent folder                |
| `cd \`        | Change Directory to root folder                  |
| `cd /d`       | Change Directory to a specific drive             |
| `md`          | Make Directory                                   |
| `rd`          | Remove Directory                                 |
| `del`         | Delete file                                      |
| `del /f`      | Force delete file                                |
| `del /q`      | Quiet mode, do not ask if ok to delete on global |
| `dir`         | List files and folders                           |
| `dir /a`      | List all files and folders                       |
| `copy`        | Copy file                                        |
| `move`        | Move file                                        |
| `ren`         | Rename file                                      |
| `type`        | Display file contents                            |
| `echo`        | Display message                                  |
| `start`       | Start program                                    |
| `tasklist`    | List running processes                           |
| `taskkill`    | Kill process                                     |
| `shutdown`    | Shutdown computer                                |
| `shutdown /r` | Restart computer                                 |

## PowerShell Commands [source&nearr;](https://ss64.com/ps/)

| Command                                                | Description                            |
| ------------------------------------------------------ | -------------------------------------- |
| `Get-Command`                                          | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Management`  | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Utility`     | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Security`    | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Diagnostics` | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Host`        | Get the commands for a specific module |

### Windows Terminal [source&nearr;](https://docs.microsoft.com/en-us/windows/terminal/)

Windows Terminal is a new, modern, feature-rich, productive terminal application for command-line users. It includes many of the features most frequently requested by the Windows command-line community including support for tabs, rich text, globalization, configurability, theming & styling, and more.

#

## Tools

### **<u>Chocolatey</u>** [source&nearr;](https://chocolatey.org/)

Chocolatey is a package manager for Windows. It was designed to be a decentralized framework for quickly installing applications and tools that you need. It is built on the NuGet infrastructure currently using PowerShell as its focus for delivering packages from the distros to your door, err computer.
[packages](https://community.chocolatey.org/packages)

| Command                          | Description                     |
| -------------------------------- | ------------------------------- |
| `choco install <package name>`   | Install a package               |
| `choco search <package name>`    | Search for a package            |
| `choco list -l`                  | List installed packages         |
| `choco upgrade <package name>`   | Upgrade a package               |
| `choco upgrade all`              | Upgrade all packages            |
| `choco upgrade chocolatey`       | Upgrade Chocolatey              |
| `choco uninstall <package name>` | Uninstall a package             |
| `choco uninstall all`            | Uninstall all packages          |
| `choco info <package name>`      | Get information about a package |

#

### **<u>Windows Subsystem for Linux</u>** [source&nearr;](https://docs.microsoft.com/en-us/windows/wsl/install-win10)

The Windows Subsystem for Linux lets developers run a GNU/Linux environment.
Including most command-line tools, utilities, and applications directly on Windows, unmodified, without the overhead of a traditional virtual machine or dualboot setup.

### <u>Installing WSL2</u>

- Pre-requisities

  - WSL 2 is only available in Windows 11 or Windows 10, Version 1903, Build 18362 or later
  - Type msinfo32 from the PowerTools search bar and confirm Hyper-V is supported and enabled
  - Or just run the following from PowerShell (as Administrator):

    ```Bash
    dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
    ```

- Install WSL from Command Prompt (as Administrator)

  ```Bash
  - wsl.exe --install # use if this is your first install
  - wsl --set-default-version 2 # to verify, type "wsl -l -v" in Powershell or Windows Command Prompt
  ```

- Install a Linux distro from the Microsoft Store
- Access distro from the Windows Terminal

- Official documentation [here](https://docs.microsoft.com/en-us/windows/wsl/install)

### <u>Useful WSL2 Commands</u>

- From Powershell/Command Prompt
  | Command | Description |
  | ------- | ----------- |
  | `wsl status` | Check WSL status |
  | `wsl --update` | Update WSL package from Windows Store and kernel version |
  | `wsl --list --verbose` | List installed distros |
  | `wsl --set-default-version 2` | Set WSL version to 2 |
  | `wsl --shutdown` | Shutdown all running WSL distros |
  | `lsb_release -a` | Check Linux distro version |

#

### PowerToys [source&nearr;]()

PowerToys is a set of utilities for power users to tune and streamline their Windows experience for greater productivity. Inspired by the Windows 95 era PowerToys project, this reboot provides power users with ways to squeeze more efficiency out of the Windows 10 shell and customize it for individual workflows. A great overview of the Windows 95 PowerToys can be found here.

#

### X-Mouse Controls [source&nearr;](https://www.highrez.co.uk/downloads/XMouseButtonControl.htm)

Use this application to cause windows to change focus as the mouse moves over them. This is a great way to make the mouse behave how you want it to in Windows 10.

#

### ZoomIt [source&nearr;](https://docs.microsoft.com/en-us/sysinternals/downloads/zoomit)

ZoomIt is a screen zoom and annotation tool for technical presentations that include application demonstrations. ZoomIt runs unobtrusively in the tray and activates with customizable hotkeys to zoom in on an area of the screen, move around while zoomed, and draw on the zoomed image. I wrote ZoomIt to fit my specific needs and use it in all my presentations.

#

### Windows Sysinternals [source&nearr;](https://docs.microsoft.com/en-us/sysinternals/)

The Sysinternals Troubleshooting Utilities have been rolled up into a single suite of tools. This file contains the individual troubleshooting tools and help files. It does not contain non-troubleshooting tools like the BSOD Screen Saver or NotMyFault.

#

# Tricks and Tips

## Open Command Prompt from File Explorer

1. Shift + Right-click on a folder
2. Choose Open command window here in the context menu.

## Open PowerShell from File Explorer

1. Shift + Right-click on a folder
2. Choose Open PowerShell window here in the context menu.

## Open WSL Linux Shell from File Explore

1. Shift + Right-click on a folder
2. Choose Open Linux shell here in the context menu.

#

## Windows 10 God Mode [source&nearr;](https://www.howtogeek.com/436615/windows-10-god-mode/)

God Mode is a handy way to access multiple Windows commands in one single window. It’s not really a mode so much as a hidden control panel that contains everything, including some commands that are hidden from the regular Control Panel.

To enable God Mode, create a new folder anywhere on your root drive and name it:

```
GodMode.{ED7BA470-8E54-465E-825C-99712043E01C}
```

The folder icon will change to a Control Panel-style icon, and you can open it to see a list of all the commands that are available in God Mode.

#

## Windows 10 Secret Start Menu [source&nearr;](https://www.howtogeek.com/436615/windows-10-god-mode/)

Windows 10 has a hidden menu for quick access to important features. To access it, right-click the Start button or press Windows+X on your keyboard.

#

## Windows 10 Secret Screen Recorder [source&nearr;](https://www.howtogeek.com/436615/windows-10-god-mode/)

Windows 10 has a secret, built-in tool intended to help record your screen during Xbox gaming sessions. But Game Bar can also be used with non-gaming apps.

To enable Game Bar:

1. Go to Settings > Gaming > Game Bar. Turn on “Record game clips, screenshots, and broadcast using Game Bar.”
2. Press Windows+G to open Game Bar.
3. Check the “Yes, this is a game” checkbox to load the Game Bar. This option won’t be available if Game Bar isn’t enabled for your game.
4. Click the Start Recording button (or Win+Alt+R) to start capturing video.
5. Click it again to stop recording. Alternatively, you can press Win+Alt+R again to stop it.

## show windows keys

```powershell
Get-ItemProperty -Path 'HKLM:\SOFTWARE\Microsoft\Windows NT\CurrentVersion\DigitalProductId' | Select-Object -Property PSChildName, DigitalProductId
```

## Speed up Windows 10 [source&nearr;](https://www.howtogeek.com/435649/how-to-speed-up-windows-10/)

1. Disable Startup Programs
   - Task Manager > Startup
2. Disable Transparency Effects
   - Settings > Personalization > Colors > Transparency Effects
3. Disable Special Effects
   - Settings > System > About > Advanced System Settings > Performance > Settings
4. Disable Search Indexing
   - Control Panel > Indexing Options > Modify
5. Disable USB Selective Suspend
   - Control Panel > Power Options > Change Plan Settings > Change Advanced Power Settings > USB Settings > USB Selective Suspend Setting
6. Disable Windows Tips
   - Settings > System > Notifications & Actions > Get Tips, Tricks, and Suggestions as You Use Windows
7. Disable Shadows, Animations, and Visual Effects
   - Settings > System > About > Advanced System Settings > Performance > Settings > Visual Effects
8. Disable News and Interests on the Taskbar
   - Right-click on the Taskbar > News and Interests > Turn Off
9. Disable Windows Defender !CAUTION!
   - Settings > Update & Security > Windows Security > Virus & Threat Protection > Manage Settings > Real-Time Protection
10. Disable Windows Search
    - Services > Windows Search > Startup Type > Disabled
11. Clean up Temporary Files and System Files
    - Settings > System > Storage > Temporary Files > Remove Files
12. Update Drivers
    - Device Manager > Right-click on a device > Update Driver
13. Optimise Page File
    - Control Panel > System > Advanced System Settings > Performance > Settings > Advanced > Virtual Memory > Change
14. Use a high performance power plan
    - Control Panel > Hardware and Sound > Power Options > High Performance

# Fixes

## Fix blurry apps [source&nearr;](https://www.howtogeek.com/435674/how-to-fix-blurry-apps-on-windows-10-with-an-external-monitor/)

Windows 10 is supposed to automatically scale its interface so that it looks crisp and smooth on high-resolution displays. Unfortunately, many Windows 10 users are facing an issue where their fonts look blurry and hard to read.

1. Right-click on the app’s shortcut on the desktop or in the start menu and open Properties.
2. Go to the Compatibility tab and under Settings section, check the ‘Disable display scaling on high DPI settings’ option.
3. Click Apply and then OK to save the changes.

## Restart Graphics Driver [source&nearr;]()

`Win+Ctrl+Shift+b`

#

## Fix Windows Update [source&nearr;](https://www.howtogeek.com/247380/how-to-fix-windows-update-when-it-gets-stuck/)

If Windows Update freezes or gets stuck, there are several steps to try.

1. Run the Windows Update Troubleshooter
2. Restart the Windows Update Service
3. Restart the Background Intelligent Transfer Service
4. Disable Your Anti-virus Software
5. Use the Media Creation Tool
6. Perform a System Restore

#

### Scan and repair system files

1. Open Command Prompt as Administrator
2. Run `CHKDSK /F /R`
3. Run `sfc /scannow`
4. Run `dism /online /cleanup-image /restorehealth`

#

### Reset Windows Update Components

1. Open Command Prompt as Administrator
2. Type the following commands and press Enter after each one:
   - `net stop bits`
   - `net stop wuauserv`
   - `net stop appidsvc`
   - `net stop cryptsvc`

#

## System Restore [source&nearr;](https://www.howtogeek.com/237230/how-to-enable-system-restore-and-repair-system-problems-on-windows-10/)

System Restore is a Windows feature that can help fix certain types of crashes and other computer problems. Here’s how it works, how to set it up, and how to use it when things go awry.

1. Open the Start menu and type “restore”. Click on “Create a restore point”.
2. Click on the “System Restore” button. ...
3. Click “Next” on the dialog box that tells you about the restore process. ...
4. Select the restore point you want to use from those in the list. ...
5. Click “Next” and then “Finish” to confirm your restore point.

#

## Manual System Restore

If System Restore doesn’t work for you, you can try to do a manual system restore.

1. Boot into Live USB
2. Go to C:\Windows\System32\config
3. Rename the following files to .old:
   - DEFAULT
   - SAM
   - SECURITY
   - SOFTWARE
   - SYSTEM
4. Go to C:\Windows\System32\config\RegBack or repair
5. Copy the latest version of the following files to C:\Windows\System32\config:
   - DEFAULT
   - SAM
   - SECURITY
   - SOFTWARE
   - SYSTEM
6. Reboot
