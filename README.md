# 🏢 Enterprise Active Directory Lab

##  Project Overview

This repository documents the complete deployment, configuration, and administration of an **Enterprise Active Directory Lab** built using **Windows Server 2022**, **Windows 11**, and **VMware Workstation**.

The project simulates a real-world enterprise environment where users, computers, groups, file servers, and security policies are centrally managed through **Active Directory Domain Services (AD DS)**.

The repository includes detailed documentation, architecture diagrams, practical configurations, troubleshooting guides, and **124 screenshots** covering every stage of the implementation.

---

#  Project Statistics

* 📁 **8 Project Modules**
* 📄 **40+ Documentation Files**
* 📸 **124 Screenshots**
* 🖥️ **2 Virtual Machines**
* 🌐 **1 Active Directory Domain**
* 👥 Multiple Users, Groups & OUs
* 📂 Enterprise File Server
* 🛡️ Enterprise Group Policy Configuration
* 🔧 Real-World Troubleshooting Scenarios

---

#  Project Objectives

* Build an Enterprise Active Directory environment from scratch.
* Configure centralized authentication and authorization.
* Deploy and manage Active Directory Domain Services.
* Implement enterprise user and group management.
* Configure secure file sharing using the AGDLP model.
* Apply and test enterprise Group Policies.
* Document common troubleshooting scenarios.
* Build a strong foundation for Active Directory Security and Attack & Defense.


#  Lab Environment

| Component         | Details                         |
| ----------------- | ------------------------------- |
| Hypervisor        | VMware Workstation              |
| Server OS         | Windows Server 2022             |
| Client OS         | Windows 11                      |
| Domain            | harish.local                    |
| Domain Controller | DC01                            |
| Client Machine    | CLIENT01                        |
| Networking        | VMware NAT                      |
| DNS               | Active Directory Integrated DNS |



# 🧱 Lab Architecture

<img width="1197" height="1314" alt="image" src="https://github.com/user-attachments/assets/eb529bdf-0f7e-44a4-bfb0-7886f5befaf8" />


---

# 📂 Project Structure
<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/8f5d5149-11a6-4efd-b340-e89ffad2e86d" />

```text
Enterprise-Active-Directory-Lab
│
├── 01-Project-Overview
│   ├── Lab-Architecture.md
│   ├── Lab-Requirements.md
│   ├── Learning-Roadmap.md
│   ├── Project-Goal.md
│
├── 02-Lab-Setup
│   ├── Screenshots
│   ├── Windows-11-Screenshots
│   ├── VMware-Installation.md
│   ├── Virtual-Networking.md
│   ├── Windows-Server-2022-Installation.md
│   ├── Windows-11-Installation.md
│   └── Static-IP-Configuration.md
│
├── 03-Active-Directory
│   ├── Screenshots
│   ├── Active-Directory-Basics.md
│   ├── ADDS-Installation.md
│   ├── DNS-Configuration.md
│   ├── Domain-Controller.md
│   ├── Organizational-Units.md
│   ├── Users.md
│   ├── Groups.md
│   └── Client-Domain-Join.md
│
├── 04-File-Server
│   ├── Screenshots
│   ├── Shared-Folders.md
│   ├── NTFS-Permissions.md
│   ├── Share-Permissions.md
│   └── Access-Based-Enumeration.md
│
├── 05-Group-Policy
│   ├── Screenshots
│   ├── GPO-Basics.md
│   ├── Password-Policy.md
│   ├── Account-Lockout-Policy.md
│   ├── Desktop-Wallpaper-Policy.md
│   ├── Control-Panel-Restriction.md
│   ├── USB-Restriction.md
│   ├── Command-Prompt-Restriction.md
│   ├── Login-Banner.md
│   ├── GPO-Processing.md
│   ├── Block-Inheritance.md
│   ├── Enforced.md
│   └── Loopback-Processing.md
│
├── 06-Troubleshooting
│   ├── Installation-Issues.md
│   ├── Network-Issues.md
│   ├── DNS-Issues.md
│   ├── Domain-Join-Issues.md
│   ├── Login-Issues.md
│   ├── GPO-Issues.md
│   ├── File-Server-Issues.md
│   └── Common-Errors.md
│
├── 07-Commands
│   ├── Active-Directory-Commands.md
│   ├── Networking-Commands.md
│   ├── File-Server-Commands.md
│   ├── Group-Policy-Commands.md
│   ├── PowerShell-Commands.md
│   └── Troubleshooting-Commands.md
│
├── README.md
├── LICENSE
└── .gitignore
```

---

# 🛠️ Technologies Used

* Windows Server 2022
* Windows 11
* VMware Workstation
* Active Directory Domain Services (AD DS)
* DNS Server
* SMB File Sharing
* NTFS Permissions
* Group Policy Management
* Active Directory Users and Computers
* Active Directory Administrative Center
* PowerShell
* Windows Networking

---

# 📖 Topics Covered

## Active Directory

* Active Directory Basics
* Active Directory Domain Services (AD DS)
* Domain Controller
* Forest and Domain
* Organizational Units (OU)
* Users and Groups
* AGDLP Permission Model
* Active Directory Database

---

## Networking

* VMware NAT Networking
* Static IP Configuration
* DNS Configuration
* Default Gateway
* Name Resolution
* Client Connectivity

---

## Client Management

* Windows 11 Installation
* Local Administrator Configuration
* Domain Join
* Domain Authentication

---

## File Server

* SMB File Sharing
* Shared Folders
* NTFS Permissions
* Share Permissions
* AGDLP Implementation

---

## Group Policy

* Password Policy
* Account Lockout Policy
* Desktop Wallpaper
* USB Storage Restriction
* Command Prompt Restriction
* Control Panel Restriction
* Login Banner
* LSDOU Processing
* Block Inheritance
* Enforced
* Loopback Processing

---

## Troubleshooting

* Installation Issues
* Networking Issues
* DNS Issues
* Domain Join Issues
* Login Issues
* Group Policy Issues
* File Server Issues
* Common Administrative Errors

---

# 📸 Screenshots

This repository contains **124 screenshots** documenting every stage of the lab, including:

* VMware setup
* Virtual networking
* Windows Server installation
* Windows 11 installation
* Active Directory deployment
* DNS configuration
* Organizational Units
* User and Group management
* Client domain join
* File Server configuration
* NTFS & Share permissions
* Group Policy implementation
* Testing and validation
* Troubleshooting scenarios

These screenshots provide a complete visual walkthrough of the entire lab.

---

# 💡 Skills Demonstrated

* Windows Server Administration
* Active Directory Administration
* DNS Configuration
* Enterprise Networking
* User & Group Management
* AGDLP Permission Model
* File Server Administration
* Group Policy Management
* Windows Troubleshooting
* Technical Documentation

---

# 👨‍💻 Author

**Harish**

Cybersecurity enthusiast focused on Windows Infrastructure, Active Directory, Networking, Enterprise Security, and Offensive Security.

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub.
