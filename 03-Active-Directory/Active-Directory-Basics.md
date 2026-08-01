# Active Directory Basics

## Objective

Understand the fundamentals of Active Directory, its purpose, architecture, and how it is used to centrally manage users, computers, and resources in an enterprise environment.

# What is Active Directory?

Active Directory (AD) is a directory service developed by Microsoft that stores information about users, computers, groups, printers, and other network resources. It enables administrators to centrally manage and secure an organization's IT environment.

# Why Do Companies Use Active Directory?

Without Active Directory:

- Every computer has separate user accounts.
- Administrators must configure each computer individually.
- Managing permissions becomes difficult.
- Security policies are inconsistent.
- User management is time-consuming.

With Active Directory:

- Users have one account for the entire organization.
- Computers are managed centrally.
- Security policies are applied automatically.
- Resources can be shared securely.
- Administration becomes faster and easier.

# Core Functions of Active Directory

- Authentication
- Authorization
- Centralized User Management
- Computer Management
- Group Management
- Group Policy Management
- Resource Sharing
- Security Management

# Authentication vs Authorization

### Authentication

Authentication verifies the identity of a user.

Example:

Harish enters a username and password.

The Domain Controller verifies the credentials.

If correct, access is granted.


### Authorization

Authorization determines what the authenticated user is allowed to access.

Example:

Harish belongs to the HR department.

He can access only the HR shared folder.

# Active Directory Objects

Everything stored inside Active Directory is called an object.

Examples:

- Users
- Computers
- Groups
- Organizational Units (OUs)
- Printers
- Shared Folders

# Main Components of Active Directory

### Forest

The highest-level logical structure in Active Directory.

A forest contains one or more domains.

### Domain

A domain is the central administrative boundary that stores users, computers, groups, and security policies.

Example:

harish.local

### Organizational Unit (OU)

A logical container used to organize Active Directory objects.

Examples:

- HR
- Finance
- IT

### User

Represents an employee or person who can log into the domain.

Example:

Harish

### Computer

Represents a domain-joined device.

Example:

CLIENT01

### Group

Used to organize users and simplify permission management.

Example:

HR_GG

### Domain Controller (DC)

A Windows Server that stores the Active Directory database and provides authentication and authorization services.

Example:

DC01

# Active Directory Database

The Active Directory database is stored in:

C:\Windows\NTDS\NTDS.dit

It stores:

- Users
- Groups
- Computers
- Password hashes
- Security information
- Organizational Units

# Services Used by Active Directory

- DNS
- Kerberos
- LDAP
- SMB

These services work together to enable authentication, resource access, and directory services.

# Benefits of Active Directory

- Centralized Administration
- Improved Security
- Easier User Management
- Simplified Permission Management
- Policy Enforcement
- Scalability
- Better Resource Sharing

# Real-World Example

A company has:

- 500 employees
- 300 computers
- 5 departments

Without Active Directory:

Administrators create and manage accounts on each individual computer.

With Active Directory:

Administrators create one domain account for each employee.

The employee can log into any authorized domain-joined computer using the same credentials.

Permissions are managed centrally through groups and Group Policy.

# Summary

Active Directory is Microsoft's directory service that provides centralized authentication, authorization, user management, computer management, and security policy enforcement across an enterprise network. It allows organizations to efficiently manage users, devices, and resources from a central location.
