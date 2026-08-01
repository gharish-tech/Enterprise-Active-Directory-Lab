# Group Policy Basics

## Objective

Understand what Group Policy is, why organizations use it, and how it centrally manages Windows computers and users in an Active Directory environment.

## What is Group Policy?

Group Policy (GPO) is a Windows feature that allows administrators to centrally configure and enforce settings for users and computers in an Active Directory domain.

Instead of configuring each computer manually, administrators create a Group Policy once and apply it to multiple users or computers.

## Why is Group Policy Used?

In enterprise environments, hundreds or thousands of computers exist.

Without Group Policy, administrators would have to configure each computer manually.

Group Policy helps by:

- Centralizing administration
- Enforcing security policies
- Maintaining consistency across the organization
- Reducing administrative effort
- Improving security and compliance

## What Can Group Policy Configure?

Examples include:

- Password Policy
- Account Lockout Policy
- Desktop Wallpaper
- USB Storage Restriction
- Command Prompt Restriction
- Control Panel Restriction
- Login Banner
- Windows Update Settings
- Software Installation
- Security Settings

## User Configuration vs Computer Configuration

### User Configuration

Applies settings to user accounts.

Examples:

- Desktop Wallpaper
- Control Panel Restriction
- Command Prompt Restriction

The policy follows the user regardless of which domain-joined computer they log into.

### Computer Configuration

Applies settings to computer objects.

Examples:

- USB Storage Restriction
- Login Banner
- Windows Update Configuration

The policy follows the computer regardless of which user logs in.

## How Does Group Policy Work?

1. Administrator creates a GPO.
2. The GPO is linked to a Site, Domain, or Organizational Unit (OU).
3. During startup and user logon, Windows downloads the applicable policies from the Domain Controller.
4. Windows applies the settings automatically.

## GPO Processing Order (LSDOU)

Windows processes Group Policies in the following order:

1. Local
2. Site
3. Domain
4. Organizational Unit (OU)

If multiple GPOs configure the same setting, the last applied policy normally takes precedence.

## Important Concepts Learned

- User Configuration
- Computer Configuration
- LSDOU Processing
- Block Inheritance
- Enforced
- Loopback Processing

## Benefits of Group Policy

- Centralized management
- Improved security
- Consistent configuration
- Faster administration
- Easier troubleshooting
- Better compliance with organizational policies

## Conclusion

Group Policy is one of the core components of Active Directory administration. It enables administrators to centrally manage and secure Windows computers and users by applying consistent configurations across the enterprise.