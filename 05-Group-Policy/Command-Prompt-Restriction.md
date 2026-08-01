# Command Prompt Restriction

## Objective

Prevent HR users from using Command Prompt.

## Configuration

User Configuration

Administrative Templates

System

Prevent access to the command prompt

Enabled

Disable command prompt script processing

Yes

## Testing

Applied the GPO.

Logged in as an HR user.

Verified that Command Prompt was blocked.

Logged in as a Finance user.

Verified that Command Prompt opened normally.

## Result

Command Prompt access was successfully restricted for HR users.