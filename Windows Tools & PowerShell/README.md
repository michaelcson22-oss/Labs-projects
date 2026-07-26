# Windows Administration & PowerShell Lab

## Overview

This repository documents my experience using Windows administrative tools, PowerShell, and Command Prompt to automate tasks, troubleshoot systems, and manage Windows environments. The scripts and commands included here reflect common responsibilities performed by IT Support Technicians and Systems Administrators in enterprise environments.

The purpose of this repository is to strengthen my Windows administration skills while building a reference library of practical commands used for system management and troubleshooting.

---

# Objectives

- Learn PowerShell fundamentals
- Automate repetitive administrative tasks
- Gather system and hardware information
- Troubleshoot Windows devices
- Practice networking commands
- Manage Windows services and processes
- Develop PowerShell scripting skills
- Build an IT administration command reference

---

# Environment

| Component | Description |
|------------|-------------|
| Operating System | Windows 11 Pro |
| PowerShell | Windows PowerShell 5.1 / PowerShell 7 |
| Terminal | Windows Terminal |
| Code Editor | Visual Studio Code |

---

# Skills Demonstrated

- Windows Administration
- PowerShell Scripting
- Windows Troubleshooting
- Network Troubleshooting
- Active Directory Administration
- Microsoft 365 Administration
- Automation
- Documentation
- Problem Solving

---

# Administrative Commands

## System Information

Retrieve hardware and operating system information.

| Command | Description |
|---------|-------------|
| `Get-ComputerInfo` | Displays detailed system information |
| `systeminfo` | Displays operating system information |
| `hostname` | Displays the computer name |
| `Get-CimInstance Win32_ComputerSystem` | Displays manufacturer and model |
| `Get-CimInstance Win32_BIOS` | Displays BIOS information |
| `Get-CimInstance Win32_OperatingSystem` | Displays operating system details |

---

## Networking

Common commands used for diagnosing network connectivity.

| Command | Description |
|---------|-------------|
| `ipconfig` | View IP configuration |
| `ipconfig /all` | Detailed network configuration |
| `ipconfig /release` | Release DHCP lease |
| `ipconfig /renew` | Renew DHCP lease |
| `ipconfig /flushdns` | Clear DNS cache |
| `ipconfig /registerdns` | Register DNS records |
| `ping google.com` | Test network connectivity |
| `tracert google.com` | Trace route to destination |
| `nslookup microsoft.com` | Test DNS resolution |
| `Test-NetConnection microsoft.com -Port 443` | Test port connectivity |
| `Get-NetAdapter` | Display network adapters |
| `Get-NetIPAddress` | Display IP addresses |
| `Get-NetIPConfiguration` | Display network configuration |
| `Get-NetRoute` | Display routing table |

---

## Active Directory & Group Policy

Common commands used in domain environments.

| Command | Description |
|---------|-------------|
| `gpupdate /force` | Refresh all Group Policies |
| `gpupdate /target:user` | Refresh user policies |
| `gpupdate /target:computer` | Refresh computer policies |
| `gpresult /r` | Display applied Group Policies |
| `gpresult /h gporeport.html` | Generate HTML Group Policy report |

---

## User Administration

Manage local user accounts.

| Command | Description |
|---------|-------------|
| `Get-LocalUser` | List local users |
| `Get-LocalGroup` | List local groups |
| `Get-LocalGroupMember Administrators` | Display local administrators |
| `New-LocalUser` | Create local user |
| `Enable-LocalUser` | Enable local account |
| `Disable-LocalUser` | Disable local account |

---

## Process Management

Manage running applications and processes.

| Command | Description |
|---------|-------------|
| `Get-Process` | View running processes |
| `Stop-Process` | Stop a process |
| `Start-Process` | Start an application |

---

## Windows Services

Manage Windows services.

| Command | Description |
|---------|-------------|
| `Get-Service` | View all services |
| `Start-Service` | Start a service |
| `Stop-Service` | Stop a service |
| `Restart-Service Spooler` | Restart Print Spooler |

---

## Disk Management

Retrieve storage information.

| Command | Description |
|---------|-------------|
| `Get-Disk` | Display physical disks |
| `Get-Partition` | Display partitions |
| `Get-Volume` | Display storage volumes |
| `Get-PSDrive` | Display available drives |

---

## Event Logs

Review Windows event logs.

| Command | Description |
|---------|-------------|
| `Get-WinEvent -LogName System -MaxEvents 20` | View recent System logs |
| `Get-EventLog System -Newest 20` | View recent System events |
| `Get-EventLog Application -Newest 20` | View recent Application events |

---

## Windows Updates

Review installed updates.

| Command | Description |
|---------|-------------|
| `Get-HotFix` | View installed Windows updates |

---

## Installed Software

Retrieve installed applications.

| Command | Description |
|---------|-------------|
| `Get-Package` | List installed packages |
| `Get-AppxPackage` | List Microsoft Store applications |
| `Get-ItemProperty HKLM:\Software\Microsoft\Windows\CurrentVersion\Uninstall\*` | List installed desktop applications |

---

## File Management

Manage files and folders.

| Command | Description |
|---------|-------------|
| `Get-ChildItem` | List files and folders |
| `Copy-Item` | Copy files |
| `Move-Item` | Move files |
| `Rename-Item` | Rename files |
| `Remove-Item` | Delete files |
| `New-Item` | Create files or folders |

---

## Windows Administrative Tools

Frequently used Microsoft Management Console (MMC) tools.

| Command | Opens |
|---------|-------|
| `compmgmt.msc` | Computer Management |
| `devmgmt.msc` | Device Manager |
| `diskmgmt.msc` | Disk Management |
| `eventvwr.msc` | Event Viewer |
| `services.msc` | Services |
| `gpedit.msc` | Local Group Policy Editor |
| `lusrmgr.msc` | Local Users and Groups |
| `taskschd.msc` | Task Scheduler |
| `perfmon.msc` | Performance Monitor |
| `resmon.exe` | Resource Monitor |
| `msinfo32` | System Information |
| `regedit` | Registry Editor |
| `msconfig` | System Configuration |

---

# PowerShell Scripts

This repository also includes PowerShell scripts for common administrative tasks.

- SystemInfo.ps1
- NetworkInfo.ps1
- InstalledPrograms.ps1
- DiskUsage.ps1
- RunningProcesses.ps1
- ServiceStatus.ps1
- EventLogErrors.ps1
- LocalUsers.ps1
- WindowsUpdates.ps1

---

# Troubleshooting Scenarios

Examples of common troubleshooting tasks practiced:

- Diagnosing internet connectivity issues
- Renewing DHCP leases
- Flushing and registering DNS
- Testing DNS resolution
- Refreshing Group Policy
- Reviewing Windows Event Logs
- Restarting Windows services
- Checking disk utilization
- Identifying resource-intensive processes
- Verifying Windows Updates

---

# Screenshots

Include screenshots of:

- Windows Terminal
- PowerShell Console
- Visual Studio Code
- Event Viewer
- Device Manager
- Services Console
- Group Policy Results
- Network Adapter Configuration
- Example PowerShell script output

---

# Lessons Learned

Working with Windows administration tools and PowerShell has strengthened my understanding of system management, troubleshooting, and automation. Building this repository has improved my ability to diagnose common Windows issues, gather system information efficiently, and automate repetitive administrative tasks commonly performed in enterprise IT environments.

---

# Future Improvements

- Active Directory PowerShell
- Microsoft Graph PowerShell
- Microsoft 365 PowerShell
- Exchange Online PowerShell
- Microsoft Entra PowerShell
- Bulk User Management
- Remote PowerShell
- Scheduled Task Automation
- Logging & Error Handling
- Desired State Configuration (DSC)
