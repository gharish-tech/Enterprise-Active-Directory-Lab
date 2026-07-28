# Windows 11 Installation

## Objective

Install Windows 11 Professional to use as the client machine in the Active Directory lab.

---

## Why Windows 11 Pro?

Windows 11 Pro supports enterprise features such as:

- Active Directory Domain Join
- Group Policy
- Remote Desktop
- Enterprise Security Features

Windows 11 Home cannot join an Active Directory domain.

---

## Installation Steps

1. Created a new virtual machine in VMware Workstation.
2. Selected the Windows 11 ISO.
3. Configured:
   - 4 GB RAM
   - 2 CPU Cores
   - 60 GB Virtual Disk
   - VMnet8 (NAT) Network
4. Installed Windows 11 Pro.
5. Chose **Custom Installation**.
6. Installed Windows on the unallocated disk.
7. Completed the initial setup.
8. Selected **Work or School** during setup.
9. Clicked **Domain join instead** to create a local administrator account.
10. Logged in using the local administrator account.

---

## Why did we create a Local Administrator account?

At this stage, the computer is not yet a member of the Active Directory domain.

A local administrator account is required to:

- Configure networking
- Rename the computer
- Join the computer to the domain
- Perform administrative tasks before domain membership

---

## Result

Windows 11 Pro was installed successfully and is ready to be joined to the Active Directory domain.

