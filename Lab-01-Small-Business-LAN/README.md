# Lab 01 — Small Business LAN

## Overview
Built and configured a basic Local Area Network (LAN) using Cisco Packet Tracer.

## Network Topology
- 1 Cisco Catalyst 2960 switch
- 4 end devices (PCs)
- Copper straight-through Ethernet cables

## IP Addressing

| Device | IPv4 Address | Subnet Mask |
|---|---|---|
| PC1 | 192.168.10.10 | 255.255.255.0 |
| PC2 | 192.168.10.11 | 255.255.255.0 |
| PC3 | 192.168.10.12 | 255.255.255.0 |
| PC4 | 192.168.10.13 | 255.255.255.0 |

## Skills Demonstrated
- Basic LAN design and topology
- Ethernet switching
- Static IPv4 configuration
- Subnet masks and CIDR notation
- ICMP and ping connectivity testing
- ARP and MAC address learning
- Cisco IOS CLI
- Basic network troubleshooting

## Testing and Results
Successfully verified connectivity between all four PCs using ICMP ping.

Used the Cisco IOS command `show mac address-table` to inspect dynamically learned MAC addresses and switch ports.

## Troubleshooting
Temporarily assigned PC4 an IP address from a different subnet (192.168.20.0/24).

Connectivity failed because the Layer 2 switch was not configured to route between different IP networks.

Restored PC4's original IP address and verified connectivity again.

## What I Learned
A Layer 2 switch forwards Ethernet frames within a LAN using MAC addresses. Communication between different IP subnets requires a Layer 3 device, such as a router.

## Future Improvements
- Introduce a router and default gateway
- Configure DHCP
- Implement VLANs
- Configure inter-VLAN routing
- Introduce network security and ACLs
