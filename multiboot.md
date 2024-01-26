# MultiBoot USB

---
## **UNDER CONSTRUCTION**
---

# my live systems list:

Windows to go

## for password recovery:

Offline NT Password & Registry Editor
PCLoginNow
Kon-Boot

## for Penetration Testing:

Kali Linux

## for benchmarking:

Phoronix Test Suite
stresslinux https://www.stresslinux.org/sl/
memtest86

## for Virus Removal:

AVG Rescue CD
BitDefender Rescue CD
Kaspersky Rescue Disk
F-Secure Rescue CD
Avira AntiVir Rescue System

## for cloning:

Clonezilla

## for data recovery:

TestDisk
PhotoRec

# System Rescue:

## for Linux:

SystemRescueCD
Knoppix
Grml https://grml.org/features/
rescatux https://www.supergrubdisk.org/rescatux/
GParted Live

## For Windows:

Hiren's BootCD
Ultimate Boot CD
FalconFour's Ultimate Boot CD
Trinity Rescue Kit
Windows Preinstallation Environment (WinPE)

### Linux installations images:

#### Debian-based:

- Tails
- Ubuntu
- Linux Mint
- Debian

#### Red Hat-based:

- Fedora

#### SUSE-based:

- openSUSE

#### Slackware-based:

- Slackware

#### Arch-based:

- Arch Linux

#### Raspberry Pi OS:

- Raspberry Pi OS
- EmulationStation

### Windows installations images:

- windows 11
- Windows 10

---

# Install using YUMI

## install YUMI on Linux: https://pendrivelinux.com/yumi-multiboot-usb-creator/

Using YUMI on Linux
Question: Can I use YUMI on Linux?
Answer: Yes, you can use the YUMI4Linux "YUMI.sh" script to make a Multibooting USB from within Linux. After preparation, you'll be able to drag and drop ISO files into the YUMI folder on the prepared drive. ISO files stored there will be detected and then added to the menu for USB booting.

Here's how to get started using YUMI in Linux:
The following steps assume that gzip and WINE packages are already installed on your system. If they, aren't you'll want to install them both before proceeding.

First, open a terminal. Ctrl+Alt+T
Next, from the open terminal window, cd to your desktop:
cd Desktop
Now download YUMI4Linux gzipped tarball using the wget command:
wget https://yumiusb.com/downloads/YUMI/YUMI4Linux.tar.gz
Then, use the following tar command to extract the archive:
(Note: you may be able to just double click the file to extract.)
tar xzvf YUMI4Linux.tar.gz
Use the cd command to switch to the YUMI4Linux folder:
cd YUMI4Linux
To set permissions and run the YUMI Linux script from a terminal:
chmod +x ./YUMI.sh && ./YUMI.sh
Once finished, the included YUMI-exFAT-1.0.2.4.exe can be run from WINE to learn more about a distro, download related ISO files, and install additional distributions + create persistence files on any prepared drive.

Note that distros can be conveniently added or removed with the .exe at any time on prepared drives.

To do this, you can simply issue the wine command from the directory containing YUMI-exFAT-1.0.2.4.exe as follows:

wine YUMI-exFAT\*

## prepare USB drive:

For Debian-based systems (e.g., Ubuntu):
Install exFAT Utilities:
Open a terminal and run the following commands to install the exFAT utilities:

bash
Copy code
sudo apt update
sudo apt install exfat-utils
Insert USB Drive:
Plug in your USB drive to your computer.

Identify the USB Drive:
Use the following command to identify the device name of your USB drive. Be careful with this step to avoid formatting the wrong drive:

bash
Copy code
sudo fdisk -l
Look for your USB drive in the list. It will likely be something like /dev/sdX, where 'X' is a letter representing the drive.

Format as exFAT:
Use the mkfs.exfat command to format the USB drive with exFAT. Replace /dev/sdX with the actual device name of your USB drive:

bash
Copy code
sudo mkfs.exfat /dev/sdX

---

# Install Manually (advanced)

## https://pendrivelinux.com/install-grub2-on-usb-from-ubuntu-linux/

## https://pendrivelinux.com/boot-multiple-iso-from-usb-via-grub2-using-linux/

## https://github.com/adi1090x/uGRUB

## https://www.gnome-look.org/p/2072033