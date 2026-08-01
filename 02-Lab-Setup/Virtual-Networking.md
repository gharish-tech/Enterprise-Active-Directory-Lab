# Virtual Networking in VMware

## Objective

Configure virtual networking so that the Domain Controller (DC01) and Client (CLIENT01) can communicate with each other while also having internet access.


# Why is Virtual Networking Required?

Since both Windows Server and Windows 11 are running as virtual machines inside VMware Workstation, they require a virtual network to communicate.

Without virtual networking:

- The Domain Controller cannot communicate with the client.
- The client cannot join the domain.
- DNS resolution will fail.
- Active Directory authentication will not work.


# Network Mode Used

Network Adapter: NAT (Network Address Translation)

Reason:

- Allows all virtual machines to communicate with each other.
- Provides internet access to the virtual machines.
- Uses VMware's virtual NAT network.
- No additional router configuration is required.


# VMware NAT Network

In this lab VMware automatically created a NAT network.

Example:

VMware NAT Network

Subnet:

192.168.182.0/24

Gateway:

192.168.182.2

The NAT gateway allows virtual machines to reach external networks through the host operating system.


# IP Address Configuration

## Domain Controller (DC01)

IP Address:

192.168.182.10

Subnet Mask:

255.255.255.0

Default Gateway:

192.168.182.2

Preferred DNS:

192.168.182.10


## Client (CLIENT01)

IP Address:

192.168.182.20

Subnet Mask:

255.255.255.0

Default Gateway:

192.168.182.2

Preferred DNS:

192.168.182.10


# Why Static IP Addresses?

The Domain Controller must always be reachable using the same IP address.

If DHCP changes the IP address:

- Clients cannot locate the Domain Controller.
- DNS records become incorrect.
- Authentication and domain services may fail.

Therefore static IP addresses were configured for both virtual machines.


# Communication Flow

CLIENT01

↓

DNS Request

↓

DC01 (DNS + Active Directory)

↓

Authentication

↓

Access Granted


# Internet Connectivity Flow

Internet

↓

Router / Mobile Hotspot

↓

Host Windows Computer

↓

VMware NAT

↓

DC01 / CLIENT01

VMware translates the virtual machine traffic and forwards it through the host operating system to the internet.


# Connectivity Verification

The following tests were performed successfully:

- Ping from CLIENT01 to DC01
- Ping from CLIENT01 to VMware NAT Gateway
- Internet access from both virtual machines
- Name resolution using the Domain Controller


# Troubleshooting Performed

Issue:

CLIENT01 could not communicate with the Domain Controller.

Resolution:

- Verified both virtual machines were connected to the NAT network.
- Verified static IP configuration.
- Verified subnet mask.
- Verified default gateway.
- Verified preferred DNS server.
- Tested connectivity using ping.


# Result

Both virtual machines successfully communicated over the VMware NAT network.

The client was able to reach the Domain Controller, resolve DNS queries, access the internet, and later join the Active Directory domain.
