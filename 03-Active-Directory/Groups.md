# Active Directory Groups

## Objective

Create Security Groups for different departments and assign users as members.

## Groups Created

- HR Users
- Finance Users
- IT Users

## Group Type

- Security

## Group Scope

- Global

## Result

Department-based Security Groups were created successfully, and users were added as members.

## Group Scope
- Domain Local
- Global
- Universal

1.Global:
-- Global Groups are mainly used to organize users who have the same job role.
Global Groups contain users.

2.Domain local:
-- Domain Local Groups receive permissions on resources.
We don't add users here.
We add permissions.

3.Universal:
-- Universal Groups are used when we have the muliple domains with forest.

## AGDLP (ACCOUNTS GLOBAL GROUP DOMAIN LOCAL GROUP PERMISSIONS)
-- AGDLP is Microsoft's recommended permission model where Accounts (users) are added to Global Groups, Global Groups are added to Domain Local Groups, and permissions are assigned only to the Domain Local Groups. This simplifies administration and makes permission management more scalable.




