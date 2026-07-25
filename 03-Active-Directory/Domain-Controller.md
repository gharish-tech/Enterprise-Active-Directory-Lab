# Promoting the Server to a Domain Controller

## Objective

Promote the Windows Server 2022 system to the first Domain Controller in a new Active Directory forest.

## Configuration

- Forest: harish.local
- Domain: harish.local
- Functional Level: Windows Server 2016
- DNS Server: Installed
- Global Catalog: Enabled

## Result

The server was successfully promoted to a Domain Controller. Active Directory, DNS, NTDS database, and SYSVOL were configured automatically, and the new domain `harish.local` was created.
