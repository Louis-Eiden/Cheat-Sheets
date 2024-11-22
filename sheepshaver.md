# SheepShaver Cheatsheet

---

## **UNDER CONSTRUCTION**

---

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Troubleshooting](#troubleshooting)
- [Additional Resources](#additional-resources)
- [Tutorials](#tutorials)

## Introduction

SheepShaver is a Macintosh emulator that runs on Linux, macOS, and Windows. It allows you to run classic Mac OS applications and games on your modern computer.

## Installation

download from source:

> git clone https://github.com/sheepshaver/sheepshaver.git

or the official installer from:

https://www.emaculation.com/forum/viewtopic.php?t=5325

extract the zip file and run the SheepShaverGUI.exe as admin.

## Usage

### Basic Controls

- **Start/Stop**: Click the "Start" button in the GUI to launch SheepShaver, "Quit" to exit
- **Full Screen**: Press Ctrl+Return to toggle between windowed and full-screen modes
- **Mouse Capture**: Click inside the window to capture mouse, Ctrl+Return to release
- **Keyboard**: Most keys work as expected; special Mac keys are mapped to PC equivalents

### File Transfer

1. Set up a shared folder in SheepShaver preferences
2. Access shared files through "Unix" drive on the Mac OS desktop
3. Drag and drop files between host and guest systems

## Configuration

### System Requirements

- ROM file from a real Mac (Mac OS ROM image)
- Mac OS installation media (7.5.2 through 9.0.4)
- Minimum 32MB RAM allocation (128MB recommended)
- Hard disk image file (minimum 500MB recommended)

### Basic Setup

1. Launch SheepShaverGUI
2. Set ROM path
3. Create or select hard disk image
4. Configure memory allocation
5. Set screen resolution
6. Choose shared folders
7. Save settings

### Network Configuration

- Built-in networking support
- TCP/IP networking available
- Ethernet emulation supported
- Internet access possible through host connection

## Troubleshooting

### Common Issues

1. **Black Screen on Startup**

   - Verify ROM file integrity
   - Check screen resolution settings
   - Ensure sufficient memory allocation

2. **Crashes During Boot**

   - Try different ROM versions
   - Verify OS installation
   - Check disk image integrity

3. **No Network Connection**
   - Verify network settings in preferences
   - Check host firewall settings
   - Ensure proper network driver installation

### Performance Tips

- Allocate appropriate RAM (not too much, not too little)
- Use appropriate screen resolution
- Disable unnecessary extensions
- Regular maintenance of virtual disk

## Additional Resources

### Official Resources

- [E-Maculation Forums](https://www.emaculation.com/forum/)
- [SheepShaver GitHub Repository](https://github.com/cebix/macemu)

### ROM Sources

- Legal ROM extraction tools
- Original Mac hardware required
- No direct ROM download links (copyright restrictions)

### Compatible Software

- Mac OS 7.5.2 through 9.0.4
- Most classic Mac applications
- Games and productivity software
- Educational software

## Tutorials

### Basic Setup Tutorial

1. Download and install SheepShaver
2. Obtain legal ROM file
3. Create disk image
4. Install Mac OS
5. Configure preferences
6. First boot and testing

### Advanced Configuration

- Custom keyboard mapping
- Multiple disk images
- Network configuration
- Printer setup
- Audio configuration

### Tips and Tricks

- Using disk image mounting tools
- Extension management
- Performance optimization
- Data backup strategies
- Troubleshooting techniques

### Install Mac OS 9.0.4

1. extract SheepShaver (ShaveShifter)

2. Copy the ISO and the ROM into the SheepShaver folder.

3. Rename the ROM to "MAC OS ROM" without extension.

4. start SheepShaverGUI as Admin.

5. create a new disk image with 1000MB. (2000MB is maximum)

6. Add the Mac OS 9.0.4 ISO file.

7. Disable CD-Rom Drives

8. Enable "My Computer" icon on your Mac desktop (external file system)

9. under Graphics/Sound tab set Window Refresh Rate to Dynamic and Set a bigger screen resolution.

10. Under Memory/Msc tab set Memory to at least 32MB but 512MB is highly recommended.

11. Click on the "Start" button to boot your Mac OS 9.0.4.

12. initialize the hard drive.

13. Start the Mac OS 9.0.4 Installer.

[How To on Youtube](https://www.youtube.com/watch?v=TY3pjSGg1y4&t=3s)

[SheepShaver from E-Maculation](https://www.emaculation.com/forum/viewtopic.php?t=5325)

[ROM from Redundant Robot](https://www.redundantrobot.com/)

[Mac OS 9 from WinWorld](https://winworldpc.com/product/mac-os-9/90)

[GTK Runtime Environment](https://sourceforge.net/projects/gtk-win/files/GTK+%20Runtime%20Environment/GTK+%202.24/)
