# WSL and WSL2 Cheat Sheet

---
## **UNDER CONSTRUCTION**
---

https://learn.microsoft.com/en-us/windows/wsl/

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [WSL](#wsl)
    - [Starting WSL](#starting-wsl)
    - [Stopping WSL](#stopping-wsl)
    - [Updating WSL](#updating-wsl)
- [WSL2](#wsl2)
    - [Starting WSL2](#starting-wsl2)
    - [Stopping WSL2](#stopping-wsl2)
    - [Updating WSL2](#updating-wsl2)

## Introduction
WSL (Windows Subsystem for Linux) is a compatibility layer for running Linux binary executables natively on Windows 10 and Windows Server 2019. WSL2 is the second version of WSL, which includes a full Linux kernel.

## Installation
To install WSL and WSL2, follow these steps:
1. Open PowerShell as Administrator.
2. Run the following command to enable WSL:
     ```powershell
     wsl --install
     ```
3. Restart your computer.

## WSL
### Starting WSL
To start WSL, open a command prompt or PowerShell window and run the following command:


## create a wslconfig file

```bash
notepad $env:USERPROFILE/.wslconfig
```

## add the following to the file

```bash
[wsl2]
memory=4GB
processors=2
```
