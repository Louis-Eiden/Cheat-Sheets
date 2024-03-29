# Windows Cheat Sheet

A Cheat Sheet for Windows 10

## Table of Contents

- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Run Commands](#run-commands)
- [Folder Shortcuts](#folder-shortcuts)
- [CMD Commands](cmd.md)
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
  - [Open WSL Linux Shell from File Explore](#open-wsl-linux-shell-from-file-explorer)
  - [Windows 10 God Mode](#windows-10-god-mode)
  - [Windows 10 Secret Start Menu](#windows-10-secret-start-menu)
  - [Windows 10 Secret Screen Recorder](#windows-10-secret-screen-recorder)
  - [Show Windows Keys](#show-windows-keys)
  - [Speed up Windows 10](#speed-up-windows-10)
  - [Create a Windows 10 Bootable USB](#create-a-windows-10-bootable-usb)
  - [Create a Linux Bootable USB](#create-a-linux-bootable-usb)
- [Fixes](#fixes)
  - [Fix blurry apps](#fix-blurry-apps)
  - [Restart Graphics Driver](#restart-graphics-driver)
  - [Fix Windows Update](#fix-windows-update)
  - [Scan and repair system files](#scan-and-repair-system-files)
  - [Reset Windows Update Components](#reset-windows-update-components)
  - [System Restore](#system-restore)
  - [Manual System Restore](#manual-system-restore)

#

## **<u id="keyboard-shortcuts" >Keyboard Shortcuts</u>** [source&nearr;](https://support.microsoft.com/en-us/windows/keyboard-shortcuts-in-windows-dcc61a57-8ff0-cffe-9796-cb9706c75eec)

| Shortcut                                        | Description                                                                |
| ----------------------------------------------- | -------------------------------------------------------------------------- |
| `Windows Key`                                   | Open Start Menu                                                            |
| `Windows Key + A`                               | Open Action Center                                                         |
| `Windows Key + B`                               | Highlight the notification area                                            |
| `Windows Key + C`                               | Open Cortana in listening mode                                             |
| **<u>`Windows Key + D`**                        | Display and hide the desktop                                               |
| **<u>`Windows Key + E`**                        | Open File Explorer                                                         |
| `Windows Key + F`                               | Open Feedback Hub                                                          |
| **<u>`Windows Key + G`**                        | Open Game bar when a game is open                                          |
| `Windows Key + H`                               | Open the Share charm                                                       |
| `Windows Key + I`                               | Open Settings                                                              |
| `Windows Key + J`                               | Set focus to a Windows tip                                                 |
| **<u>`Windows Key + K`**                        | Open the Connect quick action                                              |
| `Windows Key + L`                               | Lock your PC or switch accounts                                            |
| `Windows Key + M`                               | Minimize all windows                                                       |
| `Windows Key + Shift + M`                       | Restore minimized windows on the desktop                                   |
| `Windows Key + O`                               | Lock device orientation                                                    |
| `Windows Key + P`                               | Choose a presentation display mode                                         |
| `Windows Key + Q`                               | Open Cortana in typing mode                                                |
| **<u>`Windows Key + R`**                        | Open Run dialog box                                                        |
| `Windows Key + S`                               | Open search                                                                |
| **<u>`Windows Key + T`**                        | Cycle through apps on the taskbar                                          |
| `Windows Key + U`                               | Open Ease of Access Center                                                 |
| **<u>`Windows Key + V`**                        | Show Clipboard History                                                     |
| **<u>`Windows Key + X`**                        | Open the Quick Link menu                                                   |
| `Windows Key + Z`                               | Show the commands available in an app                                      |
| **<u>`Windows Key + 1-9`**                      | Open the app pinned to the taskbar in the position indicated by the number |
| `Windows Key + ,`                               | Temporarily peek at the desktop                                            |
| `Windows Key + .`                               | Snap a window to a quadrant of the screen                                  |
| `Windows Key + Spacebar`                        | Switch input language and keyboard layout                                  |
| **<u>`Windows Key + Tab`**                      | Open Task view                                                             |
| `Windows Key + Esc`                             | Close Task view                                                            |
| **<u>`Windows Key + Left/Right arrow`**         | Snap app windows Left/Right                                                |
| **<u>`Windows Key + Up/Down arrow`**            | Maximize/Minimize app windows                                              |
| **<u>`Windows Key + Shift + Up arrow`**         | Stretch the desktop window to the top and bottom of the screen             |
| **<u>`Windows Key + Shift + Down arrow`**       | Restore/minimize active desktop windows vertically, maintaining width      |
| **<u>`Windows Key + Shift + Left/Right arrow`** | With multiple monitors, move the active window to other monitor            |
| **<u>`Windows Key + Ctrl + Left/Right arrow`**  | Switch between virtual desktops                                            |
| `Windows Key + Ctrl + D`                        | Add a virtual desktop                                                      |
| `Windows Key + Ctrl + F4`                       | Close current virtual desktop                                              |
| `Windows Key + Ctrl + F`                        | Search for PCs (if you're on a network)                                    |

#

## **<u id="run-commands" >Run Commands</u>**

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

## **<u id="folder-shortcuts">Folder Shortcuts</u>**

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

#

## **<u id="powershell-commands">PowerShell Commands</u>** [source&nearr;](https://ss64.com/ps/)

| Command                                                | Description                            |
| ------------------------------------------------------ | -------------------------------------- |
| `Get-Command`                                          | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Management`  | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Utility`     | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Security`    | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Diagnostics` | Get the commands for a specific module |
| `Get-Command -Module Microsoft.PowerShell.Host`        | Get the commands for a specific module |

#

## **<u id="windows-terminal">Windows Terminal</u>** [source&nearr;](https://docs.microsoft.com/en-us/windows/terminal/)

Windows Terminal is a new, modern, feature-rich, productive terminal application for command-line users. It includes many of the features most frequently requested by the Windows command-line community including support for tabs, rich text, globalization, configurability, theming & styling, and more.

#

## **<u id="tools">Tools</u>**

### **<u id="chocolatey">Chocolatey</u>** [source&nearr;](https://chocolatey.org/)

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

### **<u id="windows-subsystem-for-linux">Windows Subsystem for Linux</u>** [source&nearr;](https://docs.microsoft.com/en-us/windows/wsl/install-win10)

The Windows Subsystem for Linux lets developers run a GNU/Linux environment.
Including most command-line tools, utilities, and applications directly on Windows, unmodified, without the overhead of a traditional virtual machine or dualboot setup.

### <u id="installing-wsl2">Installing WSL2</u>

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

### <u id="useful-wsl2-commands">Useful WSL2 Commands</u>

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

### <u id="powertoys">PowerToys</u>

PowerToys is a set of utilities for power users to tune and streamline their Windows experience for greater productivity. Inspired by the Windows 95 era PowerToys project, this reboot provides power users with ways to squeeze more efficiency out of the Windows 10 shell and customize it for individual workflows. A great overview of the Windows 95 PowerToys can be found here.

#

### <u id="x-mouse-controls">X-Mouse Controls</u> [source&nearr;](https://www.highrez.co.uk/downloads/XMouseButtonControl.htm)

Use this application to cause windows to change focus as the mouse moves over them. This is a great way to make the mouse behave how you want it to in Windows 10.

#

### <u id="zoomit">ZoomIt</u> [source&nearr;](https://docs.microsoft.com/en-us/sysinternals/downloads/zoomit)

ZoomIt is a screen zoom and annotation tool for technical presentations that include application demonstrations. ZoomIt runs unobtrusively in the tray and activates with customizable hotkeys to zoom in on an area of the screen, move around while zoomed, and draw on the zoomed image. I wrote ZoomIt to fit my specific needs and use it in all my presentations.

#

### <u id="windows-sysinternals">Windows Sysinternals</u> [source&nearr;](https://docs.microsoft.com/en-us/sysinternals/)

The Sysinternals Troubleshooting Utilities have been rolled up into a single suite of tools. This file contains the individual troubleshooting tools and help files. It does not contain non-troubleshooting tools like the BSOD Screen Saver or NotMyFault.

#

## **<u id="tricks-and-tips">Tricks and Tips</u>**

### <u id="open-command-prompt-from-file-explorer">Open Command Prompt from File Explorer</u>

1. `Shift + Right-click` on a folder
2. Choose Open command window here in the context menu.

### <u id="open-powershell-from-file-explorer">Open PowerShell from File Explorer</u>

1. `Shift + Right-click` on a folder
2. Choose Open PowerShell window here in the context menu.

### <u id="open-wsl-linux-shell-from-file-explorer">Open WSL Linux Shell from File Explorer</u>

1. `Shift + Right-click` on a folder
2. Choose Open Linux shell here in the context menu.

#

### **<u id="windows-10-god-mode">Windows 10 God Mode</u>** [source&nearr;](https://www.howtogeek.com/436615/windows-10-god-mode/)

God Mode is a handy way to access multiple Windows commands in one single window. It’s not really a mode so much as a hidden control panel that contains everything, including some commands that are hidden from the regular Control Panel.

To enable God Mode, create a new folder anywhere on your root drive and name it:

```
GodMode.{ED7BA470-8E54-465E-825C-99712043E01C}
```

The folder icon will change to a Control Panel-style icon, and you can open it to see a list of all the commands that are available in God Mode.

#

### **<u id="windows-10-secret-start-menu">Windows 10 Secret Start Menu</u>** [source&nearr;](https://www.howtogeek.com/436615/windows-10-god-mode/)

Windows 10 has a hidden menu for quick access to important features. To access it, right-click the Start button or press Windows+X on your keyboard.

#

### **<u id="windows-10-secret-screen-recorder">Windows 10 Secret Screen Recorder</u>** [source&nearr;](https://www.howtogeek.com/436615/windows-10-god-mode/)

Windows 10 has a secret, built-in tool intended to help record your screen during Xbox gaming sessions. But Game Bar can also be used with non-gaming apps.

To enable Game Bar:

1. Go to Settings > Gaming > Game Bar. Turn on “Record game clips, screenshots, and broadcast using Game Bar.”
2. Press Windows+G to open Game Bar.
3. Check the “Yes, this is a game” checkbox to load the Game Bar. This option won’t be available if Game Bar isn’t enabled for your game.
4. Click the Start Recording button (or `Win+Alt+R`) to start capturing video.
5. Click it again to stop recording. Alternatively, you can press `Win+Alt+R` again to stop it.

#

### **<u id="show-windows-keys">Show Windows Keys</u>**

```powershell
Get-ItemProperty -Path 'HKLM:\SOFTWARE\Microsoft\Windows NT\CurrentVersion\DigitalProductId' | Select-Object -Property PSChildName, DigitalProductId
```

#

### **<u id="speed-up-windows-10">Speed up Windows 10</u>** [source&nearr;](https://www.howtogeek.com/435649/how-to-speed-up-windows-10/)

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

#

### **<u id="create-a-windows-bootable-usb">Create a Windows Bootable USB</u>**

1. Download the [Windows Media Creation Tool](https://www.microsoft.com/en-us/software-download/)
2. Run the tool and select Create installation media for another PC
3. Select the language, architecture, and edition of Windows, you need to install
4. Select USB flash drive
5. Select the USB drive you want to use
6. Wait for the tool to download the Windows 10 installation files and create the bootable USB

#

### **<u id="create-a-linux-bootable-usb">Create a Linux Bootable USB</u>**

1. Download the [Rufus](https://rufus.ie/) tool
2. Run the tool and select the USB drive you want to use
3. Select the ISO image you want to use
4. Select the partition scheme and target system type
5. Select the file system and cluster size
6. Select the volume label
7. Check the Quick Format option
8. Check the Create a bootable disk using option
9. Select the ISO image option
10. Click the Start button
11. Click the OK button

#

### **<u id="create-a-bootable-usb-manually-using-cmd">Create a bootable USB Manually using CMD</u>**

1. Open Command Prompt as Administrator
2. Run `diskpart`
3. Run `list disk`
4. Run `select disk #` (replace # with the number of the USB drive)
5. Run `clean`
6. Run `create partition primary`
7. Run `select partition 1`
8. Run `active`
9. Run `format fs=ntfs quick`
10. Run `assign`
11. Run `exit`
12. Run `bootsect /nt60 #` (replace # with the drive letter of the USB drive)
13. Copy the contents of the ISO image to the USB drive

#

## **<u id="fixes">Fixes</u>**

### <u id="fix-blurry-apps">Fix blurry apps</u> [source&nearr;](https://www.howtogeek.com/435674/how-to-fix-blurry-apps-on-windows-10-with-an-external-monitor/)

Windows 10 is supposed to automatically scale its interface so that it looks crisp and smooth on high-resolution displays. Unfortunately, many Windows 10 users are facing an issue where their fonts look blurry and hard to read.

1. Right-click on the app’s shortcut on the desktop or in the start menu and open Properties.
2. Go to the Compatibility tab and under Settings section, check the ‘Disable display scaling on high DPI settings’ option.
3. Click Apply and then OK to save the changes.

### <u id="restart-graphics-driver">Restart Graphics Driver</u>

`Win+Ctrl+Shift+b`

#

### <u id="fix-windows-update">Fix Windows Update</u> [source&nearr;](https://www.howtogeek.com/247380/how-to-fix-windows-update-when-it-gets-stuck/)

If Windows Update freezes or gets stuck, there are several steps to try.

1. Run the Windows Update Troubleshooter
2. Restart the Windows Update Service
3. Restart the Background Intelligent Transfer Service
4. Disable Your Anti-virus Software
5. Use the Media Creation Tool
6. Perform a System Restore

#

### <u id="scan-and-repair-system-files">Scan and repair system files</u>

1. Open Command Prompt as Administrator
2. Run `CHKDSK /F /R`
3. Run `sfc /scannow`
4. Run `dism /online /cleanup-image /restorehealth`

#

### <u id="reset-windows-update-components">Reset Windows Update Components</u>

1. Open Command Prompt as Administrator
2. Type the following commands and press Enter after each one:
   - `net stop bits`
   - `net stop wuauserv`
   - `net stop appidsvc`
   - `net stop cryptsvc`

#

### <u id="system-restore">System Restore</u> [source&nearr;](https://www.howtogeek.com/237230/how-to-enable-system-restore-and-repair-system-problems-on-windows-10/)

System Restore is a Windows feature that can help fix certain types of crashes and other computer problems. Here’s how it works, how to set it up, and how to use it when things go awry.

1. Open the Start menu and type “restore”. Click on “Create a restore point”.
2. Click on the “System Restore” button. ...
3. Click “Next” on the dialog box that tells you about the restore process. ...
4. Select the restore point you want to use from those in the list. ...
5. Click “Next” and then “Finish” to confirm your restore point.

#

### <u id="manual-system-restore">Manual System Restore</u>

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
