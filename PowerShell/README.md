# PowerShell Administration Lab

## Overview

This repository documents my experience learning and using PowerShell to automate administrative tasks, troubleshoot Windows systems, and gather system information. The scripts included in this lab focus on practical tasks commonly performed by IT Support Technicians and Systems Administrators.

The goal of this project is to strengthen my scripting skills while improving efficiency in Windows administration and troubleshooting.

---

# Objectives

- Learn PowerShell fundamentals
- Automate repetitive administrative tasks
- Gather system and network information
- Troubleshoot Windows devices
- Practice using PowerShell cmdlets
- Improve scripting and documentation skills

---

# Environment

| Component | Description |
|------------|-------------|
| Operating System | Windows 11 |
|Command Prompt | 
| PowerShell Version | PowerShell 7 / Windows PowerShell 5.1 |
| Editor | Visual Studio Code |
| Terminal | Windows Terminal |
| Platform | Windows Desktop |

---

# Skills Demonstrated

- PowerShell Scripting
- Windows Administration
- System Information Gathering
- Network Troubleshooting
- Service Management
- Process Management
- File Management
- Automation
- Documentation

---

# Common Administrative Tasks

## System Information

Scripts to retrieve:

- Computer Name
- Operating System
- BIOS Version
- Manufacturer
- Model
- CPU Information
- Installed RAM
- Disk Information
- Serial Number
- Uptime

Example Commands

```powershell
Get-ComputerInfo

hostname

systeminfo

Get-CimInstance Win32_OperatingSystem

Get-CimInstance Win32_ComputerSystem

Get-CimInstance Win32_BIOS
```

---

## User Administration

Examples include:

- List local users
- Create local users
- Disable accounts
- Reset passwords
- View group membership

Example Commands

```powershell
Get-LocalUser

Get-LocalGroup

Get-LocalGroupMember Administrators

New-LocalUser

Enable-LocalUser

Disable-LocalUser
```

---

## Network Administration

Examples include:

- View IP configuration
- Test network connectivity
- Check DNS resolution
- Display network adapters
- View routing table

Example Commands

```powershell
ipconfig /all

Get-NetIPAddress

Get-NetAdapter

Get-NetIPConfiguration

Test-Connection google.com

Resolve-DnsName google.com

Test-NetConnection google.com -Port 443

Get-NetRoute
```

---

## Process Management

Examples include:

- List running processes
- Stop a process
- Start applications

Example Commands

```powershell
Get-Process

Stop-Process

Start-Process

Get-Service
```

---

## Service Management

Examples include:

- View services
- Restart services
- Stop services
- Start services

Example Commands

```powershell
Get-Service

Start-Service

Stop-Service

Restart-Service
```

---

## Disk Administration

Examples include:

- View disk usage
- Check storage
- List volumes

Example Commands

```powershell
Get-Volume

Get-PSDrive

Get-Disk

Get-Partition
```

---

## Event Logs

Examples include:

- View Windows logs
- Filter errors
- Investigate crashes

Example Commands

```powershell
Get-EventLog

Get-WinEvent

Get-EventLog System

Get-EventLog Application
```

---

## Installed Software

Examples include:

```powershell
Get-Package

Get-AppxPackage

Get-ItemProperty HKLM:\Software\Microsoft\Windows\CurrentVersion\Uninstall\*
```

---

## Windows Updates

Examples include:

```powershell
Get-HotFix
```

---

## File Management

Examples include:

```powershell
Get-ChildItem

Copy-Item

Move-Item

Remove-Item

New-Item

Rename-Item
```

---

## PowerShell Scripts

Scripts included in this repository:

- SystemInfo.ps1
- InstalledPrograms.ps1
- RunningProcesses.ps1
- DiskUsage.ps1
- NetworkInfo.ps1
- PingTest.ps1
- EventLogErrors.ps1
- ServiceStatus.ps1
- LocalUsers.ps1
- WindowsUpdates.ps1

---

# Troubleshooting Tasks

Examples practiced:

- Check internet connectivity
- Verify DNS resolution
- View running services
- Find high CPU usage
- Check disk utilization
- Review event logs
- Verify Windows Updates
- Collect system information

---

# Lessons Learned

Working with PowerShell has improved my understanding of Windows administration by allowing me to automate repetitive tasks, collect system information efficiently, and troubleshoot Windows devices using built-in cmdlets. Developing scripts has also strengthened my problem-solving skills and introduced me to automation concepts commonly used in enterprise environments.

---

# Future Improvements

- Microsoft Graph PowerShell
- Microsoft 365 PowerShell
- Exchange Online PowerShell
- Microsoft Entra PowerShell
- Active Directory PowerShell
- Bulk User Creation
- Remote Administration
- Scheduled Tasks
- Logging and Error Handling
