# Enterprise Windows Server & Active Directory Lab

## Overview

This project documents the deployment and administration of a simulated enterprise Windows environment using Windows Server 2022 and Windows 11 virtual machines. The goal of this lab was to gain hands-on experience with Active Directory Domain Services (AD DS), DNS, DHCP, Group Policy, PowerShell, and common IT administration tasks performed in enterprise environments.

This lab simulates many of the responsibilities of an IT Support Technician or Systems Administrator by focusing on user management, workstation administration, centralized policy management, and network services.

---

## Objectives

- Deploy a Windows Server 2022 Domain Controller
- Configure Active Directory Domain Services (AD DS)
- Configure DNS and DHCP services
- Join Windows 11 clients to the domain
- Create Organizational Units (OUs)
- Create and manage users and security groups
- Configure Group Policy Objects (GPOs)
- Manage shared folders and permissions
- Practice common IT administration tasks using PowerShell
- Document troubleshooting steps and lessons learned

---

# Lab Environment

| Component | Configuration |
|------------|---------------|
| Hypervisor | VMware Workstation Pro |
| Domain Controller | Windows Server 2022 |
| Client OS | Windows 11 Pro |
| Directory Service | Active Directory Domain Services |
| DNS | Windows DNS Server |
| DHCP | Windows DHCP Server |
| Scripting | PowerShell |
| Authentication | Active Directory |

---

# Network Topology

---

Internet
     │
     │
Host Computer
     │
───────────────────────────
VMware Workstation
     │
     ├───────────────┐
     │               │
Windows Server    Windows 11 Client
2022              Domain Joined
     │
     ├── Active Directory
     ├── DNS
     ├── DHCP
     └── Group Policy

---

# Technologies Used

- Windows Server 2022
- Windows 11 Pro
- VMware Workstation Pro
- Active Directory
- DNS
- DHCP
- Group Policy
- PowerShell
- File Services
- NTFS Permissions

---

# Lab Tasks

## Active Directory

✔ Installed Active Directory Domain Services

✔ Promoted the server to a Domain Controller

✔ Created a new Active Directory forest

✔ Configured Organizational Units (OUs)

✔ Created users and security groups

✔ Reset passwords

✔ Unlocked user accounts

✔ Disabled and enabled user accounts

✔ Added users to security groups

---

## DNS

Configured:

- Forward Lookup Zone
- Reverse Lookup Zone
- DNS Records
- Name Resolution
- Client DNS Configuration

---

## DHCP

Configured:

- DHCP Scope
- Address Pool
- Lease Duration
- Reservations
- Default Gateway
- DNS Server Assignment

---

## Group Policy

Created and configured GPOs including:

- Password Policy
- Account Lockout Policy
- Desktop Restrictions
- Windows Update Settings
- Control Panel Restrictions
- Auto Lock Screen Policy
- Mapped Network Drives

---

## User Administration

Performed common administrative tasks including:

- Creating users
- Creating groups
- Managing OUs
- Password resets
- Group membership changes
- Account lockout recovery
- User onboarding simulation
- User offboarding simulation

---

## File Services

Configured:

- Shared folders
- NTFS Permissions
- Security Groups
- Network Drive Mapping

---

## PowerShell

Practiced Windows administration using PowerShell including:

- Retrieving system information
- Managing users
- Viewing services
- Network troubleshooting
- Administrative commands

---

# Troubleshooting

Examples of issues encountered during the project:

- DNS resolution failures
- Domain join issues
- Group Policy not applying
- DHCP lease problems
- Authentication errors
- User permission conflicts

Each issue was researched, documented, and resolved to reinforce troubleshooting methodology.

---

# Screenshots

Include screenshots of:

- VMware Lab
- Active Directory Users & Computers
- DNS Manager
- DHCP Manager
- Group Policy Management
- Shared Folder Permissions
- Windows 11 joined to the domain
- PowerShell commands

---

# Skills Demonstrated

- Windows Administration
- Active Directory Administration
- Microsoft DNS
- Microsoft DHCP
- Group Policy Management
- PowerShell
- Windows Troubleshooting
- User Management
- Network Administration
- Documentation
- Problem Solving

---

# Lessons Learned

This project strengthened my understanding of enterprise Windows administration by demonstrating how centralized identity management, networking services, and Group Policy work together within an Active Directory environment. Building and troubleshooting the lab improved my ability to diagnose common Windows infrastructure issues while reinforcing best practices for user administration and system configuration.

---

# Future Improvements

Future enhancements planned for this lab include:

- Certificate Services (AD CS)
- Windows Server Update Services (WSUS)
- File Server Resource Manager (FSRM)
- Print Services
- DFS Namespaces
- Multi-Domain Environment
- Additional Windows Clients
- Microsoft Entra ID Integration
- Hybrid Active Directory
- Azure AD Connect
- Windows Hello for Business
