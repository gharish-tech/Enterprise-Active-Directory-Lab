# USB Storage Restriction

## Objective

Prevent HR users from accessing USB storage devices.

## Configuration

Computer Configuration

Administrative Templates

System

Removable Storage Access

All Removable Storage classes: Deny all access

Enabled

## Testing

Applied the GPO.

Restarted CLIENT01.

Inserted a USB flash drive.

Verified that the storage device was inaccessible while the USB keyboard and mouse continued to function.

## Result

USB storage devices were successfully blocked.

