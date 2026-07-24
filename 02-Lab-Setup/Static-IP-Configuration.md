# Static IP Configuration

## Objective

Configure a static IPv4 address for the Windows Server before installing Active Directory Domain Services.

## Why Static IP?

A Domain Controller should always use a static IP address because clients rely on a consistent address to communicate with services such as Active Directory and DNS.

## Configuration

- IP Address: 192.168.182.10
- Subnet Mask: 255.255.255.0
- Default Gateway: 192.168.182.2
- Preferred DNS: 192.168.182.10

## Result

The server was successfully configured with a static IPv4 address and is ready for Active Directory installation.