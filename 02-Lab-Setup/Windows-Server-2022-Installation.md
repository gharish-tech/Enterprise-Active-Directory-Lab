# Windows Server 2022 Installation

# Introduction

Before installing Windows Server, it is important to understand why organizations use a server operating system instead of a client operating system like Windows 10 or Windows 11.

This section explains the basic concepts required to understand the purpose of Windows Server and how it fits into an enterprise network.

# What is an Operating System?

An Operating System (OS) is system software that acts as an interface between the user, applications, and computer hardware. It manages hardware resources such as the CPU, memory, storage, and input/output devices while providing an environment for applications to run.

Without an operating system, software applications cannot communicate with computer hardware.

# Why Do We Need an Operating System?

An operating system performs several important tasks:

- Manages CPU and memory
- Controls storage devices
- Manages files and folders
- Controls hardware devices
- Provides security
- Supports networking
- Allows applications to communicate with hardware

Without an operating system, a computer cannot perform useful tasks because hardware and software cannot communicate with each other.


# What is Windows Server?

Windows Server is a server operating system developed by Microsoft for managing enterprise networks, users, computers, applications, and shared resources.

Unlike Windows 11, which is designed primarily for personal use, Windows Server is designed to provide centralized management and network services for organizations.

It allows administrators to manage multiple computers from a central location instead of configuring each computer individually.


# Client Operating System vs Server Operating System
----------------------------------------------------------------------------
| Client Operating System           | Server Operating System              |
|-----------------------------------|--------------------------------------|
| Designed for personal use         | Designed for organizations           |
| Usually supports one primary user | Supports multiple users and services |
| Runs desktop applications         | Runs enterprise services             |
| Limited administration features   | Centralized administration           |
| Example: Windows 11               | Example: Windows Server 2022         |
----------------------------------------------------------------------------

# Why Do Companies Use Windows Server?

Large organizations may have hundreds or thousands of computers.

Managing each computer individually would be difficult and time-consuming.

Windows Server provides centralized management, allowing administrators to:

- Manage user accounts
- Control authentication
- Apply security policies
- Manage shared folders
- Control printers
- Manage computers from a central location

This reduces administrative effort and improves security.


## Virtual Machine Configuration

The Windows Server 2022 virtual machine was created using VMware Workstation.

Configuration:

- VM Name: DC01
- Memory: 4096 MB
- Processors: 2
- Virtual Disk: 60 GB
- Network Adapter: NAT
- Installation Media: Windows Server 2022 ISO

These settings provide sufficient resources for building an Active Directory lab while maintaining stable performance on the host system.
The Desktop Experience edition was selected to simplify administration and learning. After installation, Server Manager opened successfully, confirming that the operating system was installed correctly.


## Server Mangager

Server Manager is the central management console in Windows Server. It allows administrators to install server roles and features, monitor server health, manage local settings, and configure services such as Active Directory, DNS, DHCP, File Server, and Group Policy.

It opens automatically after login so administrators can immediately begin configuring the server.


## Renaming the Server

After installing Windows Server 2022, the default computer name was changed to **DC01**.

Using a meaningful server name improves administration, troubleshooting, and identification in enterprise environments.

The server was restarted to apply the new computer name successfully.