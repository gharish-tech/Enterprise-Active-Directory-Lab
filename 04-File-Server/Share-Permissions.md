# Share Permissions

## Objective

Learn how to share folders over the network and control who can access them using Share Permissions.

## What are Share Permissions?

Share Permissions are permissions applied to a shared folder that control how users access that folder over the network.

They are checked only when a user accesses a shared folder through the network.

Example:

\\DC01\HR

## Why do we need Share Permissions?

Without sharing a folder, users on other computers cannot access it over the network, even if NTFS permissions are configured correctly.

Share Permissions provide the first layer of security for network file sharing.

## Types of Share Permissions

### Read

- View files and folders
- Open files
- Cannot modify or delete files

### Change

- Read files
- Create files
- Modify files
- Delete files

### Full Control

- Read
- Change
- Modify permissions
- Take ownership

---

## Practical

1. Opened Folder Properties.
2. Opened the Sharing tab.
3. Selected Advanced Sharing.
4. Enabled "Share this folder".
5. Configured Share Permissions.
6. Removed the default "Everyone" group.
7. Added the HR_DL_Modify Domain Local Group.
8. Granted Change and Read permissions.
9. Verified access from CLIENT01.

## Internal Working

When a user accesses:

\\DC01\HR

Windows performs the following checks:

Client
↓
DNS resolves DC01
↓
SMB connection established
↓
Share Permission check
↓
NTFS Permission check
↓
Access Granted / Access Denied


## Difference Between Share Permissions and NTFS Permissions

| Share Permissions               | NTFS Permissions                            
| Apply only over the network     | Apply locally and over the network 
| Configured from the Sharing tab | Configured from the Security tab 
| First layer of network access   | Controls what users can do inside the folder 

## Best Practice

In enterprise environments, permissions are not assigned directly to users.

Instead, Microsoft recommends the AGDLP model:

User
↓
Global Group
↓
Domain Local Group
↓
Share Permission
↓
NTFS Permission
↓
Resource

This makes permission management easier and more scalable.

## Result

Successfully configured Share Permissions for the HR shared folder using the AGDLP model and verified access from CLIENT01.

## Interview Questions

### What are Share Permissions?

Share Permissions control how users access shared folders over the network.

### What protocol is used for Windows file sharing?

SMB (Server Message Block)

Default Port: TCP 445

### Why does Windows check both Share Permissions and NTFS Permissions?

Share Permissions control network access, while NTFS Permissions control access to files and folders. Windows evaluates both, and the most restrictive permission is applied.
### Why shouldn't permissions be assigned directly to users?

Assigning permissions to groups simplifies administration. When employees join or leave, administrators only need to update group membership instead of modifying folder permissions.