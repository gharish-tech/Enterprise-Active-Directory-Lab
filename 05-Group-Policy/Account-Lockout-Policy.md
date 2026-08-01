# Account Lockout Policy

## Objective

Protect domain accounts from brute-force password attacks.

## Configuration

- Lockout Threshold: 5 attempts
- Lockout Duration: 15 minutes
- Reset Counter: 15 minutes

## Testing

Entered the wrong password five times from CLIENT01.

The domain account was locked.

Unlocked the account from Active Directory Users and Computers.

## Result

The Account Lockout Policy successfully protected the domain account from repeated failed logon attempts.

