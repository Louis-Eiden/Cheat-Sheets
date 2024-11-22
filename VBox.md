# VBox Documentation

---

## **UNDER CONSTRUCTION**

---

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Virtual Machine Management](#virtual-machine-management)
  - [Creating VMs](#creating-vms)
  - [Starting and Stopping](#starting-and-stopping)
  - [Snapshots](#snapshots)
  - [Import/Export](#importexport)
- [Network Configuration](#network-configuration)
  - [Network Types](#network-types)
  - [Port Forwarding](#port-forwarding)
- [Storage Management](#storage-management)
  - [Storage Types](#storage-types)
  - [Adding Storage](#adding-storage)
  - [Shared Folders](#shared-folders)
    - [VirtualBox Shared Folder Permissions](#virtualbox-shared-folder-permissions)
- [System Settings](#system-settings)
  - [Memory](#memory)
  - [CPU](#cpu)
  - [Display](#display)
- [Guest Additions](#guest-additions)
- [Shared Folders](#shared-folders)
- [Command Line Interface](#command-line-interface)
- [Troubleshooting](#troubleshooting)
- [Best Practices](#best-practices)
- [Tutorials](#tutorials)

## Introduction

VirtualBox (VBox) is a powerful x86 and AMD64/Intel64 virtualization product for enterprise as well as home use. It is a general-purpose full virtualizer for x86 hardware, targeted at server, desktop and embedded use.

<details>
<summary>Features</summary>

- High performance
- Portability
- Guest Additions for Windows, Linux, and Solaris
- Great hardware support
- Full ACPI support
- Multiscreen resolutions
- Built-in iSCSI support
- PXE Network boot
</details>

## Installation

<details>
<summary>Windows Installation</summary>

1. Download VirtualBox from official website
2. Run the installer with administrative privileges
3. Follow installation wizard
4. Restart system after installation

Optional: Install via command line

</details>

```bash
choco install virtualbox
```

<details>
<summary>MacOS Installation</summary>

1. Download VirtualBox from official website
2. Run the installer with administrative privileges
3. Follow installation wizard
4. Restart system after installation
</details>

Optional: Install via command line

```bash
brew install --cask virtualbox
```

</details>

<details>
<summary>Linux Installation</summary>

1. Download VirtualBox from official website
2. Run the installer with administrative privileges
3. Follow installation wizard
4. Restart system after installation
</details>

Optional: Install via command line

```bash
sudo apt install virtualbox
```

</details>

## Virtual Machine Management

<details>
<summary>Creating VMs</summary>

1. Open VirtualBox
2. Click on "New" button
3. Fill in the details
4. Click on "Create" button

Optional: Create via command line

```bash
vboxmanage createvm --name "VMName" --ostype "Ubuntu" --register
```

</details>

<details>
<summary>Command Line Interface</summary>

## Creating VMs

```bash
vboxmanage createvm --name "VMName" --ostype "Ubuntu" --register
```

## Starting and Stopping VMs

```bash
vboxmanage startvm "VMName" --type headless
```

## List VMs

```bash
vboxmanage list vms
```

## Stop VM

```bash
vboxmanage controlvm "VMName" poweroff
```

## Create Snapshot

```bash
vboxmanage snapshot "VMName" take "SnapshotName"
```

## Restore Snapshot

```bash
vboxmanage snapshot "VMName" restore "SnapshotName"
```

</details>

</details>

## Troubleshooting

<details>
<summary>Common Issues</summary>

1. VM won't start

   - Check hardware virtualization is enabled in BIOS
   - Verify sufficient system resources
   - Check VM settings compatibility

2. Network connectivity issues
   - Verify network adapter settings
   - Check host network configuration
   - Ensure proper network type selection
   </details>

## Best Practices

<details>
<summary>Performance Optimization</summary>

- Allocate appropriate memory
- Use dynamic allocation for storage
- Install Guest Additions
- Enable hardware virtualization
- Regular snapshots for backup
- Clean unused snapshots
</details>

---

For more detailed information, visit the [official VirtualBox documentation](https://www.virtualbox.org/manual/).

## Tutorials

- [Creating a VM For MacOS](./tutorials/creating-a-vm-for-macos.md)

###

## Creating a VM For MacOs [source&nearr;](https://www.youtube.com/watch?v=vQJrM7HqezQ)

1. Download VirtualBox and Virtual Box Extension Pack [source&nearr;](https://www.oracle.com/de/virtualization/technologies/vm/downloads/virtualbox-downloads.html)
2. Download MacOS from [Internet Archive](https://archive.org/download/macos_iso)
3. Create a VM for MacOSx 64bit with at least4GB RAM, 100GB storage, and 2 CPUs.(opt for higher specs if possible)
4. After creating the VM, tweak the following settings: uncheck Floppy, Chipset to ICH9, Enable EFI, Video Memory to 128MB, Enable 3D Acceleration, create a second network adapter of type Bridged Adapter, and connect to Wifi Card, Enable USB 3.0 (xHCI) Controller.
5. Disable Hyper-V [source&nearr;](https://learn.microsoft.com/en-us/troubleshoot/windows-client/application-management/virtualization-apps-not-work-with-hyper-v)
6. Patch the VM to work with the downloaded MacOS ISO

Run the following commands in the Host Machine (Windows) CMD:

### Intel Processor

```bash
cd "C:\Program Files\Oracle\VirtualBox\"

VBoxManage.exe modifyvm "VM Name" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac19,3"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 0

VBoxManage setextradata "VM Name" "VBoxInternal/TM/TSCMode" "RealTSCOffset"
```

### AMD Processor

```bash
cd "C:\Program Files\Oracle\VirtualBox\"

VBoxManage.exe modifyvm "VM Name" --cpuidset 00000001 000106e5 00100800 0098e3fd bfebfbff

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemProduct" "iMac19,3"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiSystemVersion" "1.0"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/efi/0/Config/DmiBoardProduct" "Iloveapple"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/DeviceKey" "ourhardworkbythesewordsguardedpleasedontsteal(c)AppleComputerInc"

VBoxManage setextradata "VM Name" "VBoxInternal/Devices/smc/0/Config/GetKeyFromRealSMC" 0

VBoxManage modifyvm "VM Name" --cpu-profile "Intel Core i7-6700K"

VBoxManage setextradata "VM Name" "VBoxInternal/TM/TSCMode" "RealTSCOffset"

```

### VirtualBox Shared Folder Permissions [source&nearr;](https://stackoverflow.com/questions/26740113/virtualbox-shared-folder-permissions)

1. Add user to vboxsf group via command line

```bash
sudo adduser <USERNAME> vboxsf
```

On Suse:

```bash
sudo usermod --append --groups vboxsf $USER
```

2. Edit the file /etc/group (you will need root privileges). Look for the line vboxsf:x:999 and add at the end :yourusername -- use this solution if you don't have sudo
