# AGDLP Permission Implementation

## Objective

Implement enterprise permission management using AGDLP.

## Steps

1. Created Domain Local Groups.
2. Added Global Groups into Domain Local Groups.
3. Assigned NTFS permissions to Domain Local Groups.

   -- Inheritance was disabled for the HR folder so that it could have department-specific permissions. Existing inherited permissions were converted into explicit permissions, the default Users group was removed, and the HR_DL_Modify Domain Local Group was granted Modify permission. This follows the AGDLP model and allows centralized permission management.

4. Assigned Share permissions to Domain Local Groups.
5. Verified access from CLIENT01.

## Result

Users received access through group membership instead of direct permissions.