# Cisco Packet Tracer Enterprise Network

A multi-site enterprise network designed and implemented in **Cisco Packet Tracer** as part of my **ICT Practical Engineering** final project.

The project models an enterprise network for Nintendo across three geographic locations:

- 🇯🇵 **Kyoto, Japan**
- 🇫🇷 **Paris, France**
- 🇺🇸 **Redmond, USA**

Each site contains multiple network segments and buildings, with routing, switching, security, network services, and redundancy configured to simulate a realistic enterprise environment.

> **Disclaimer:** This is an educational project and is not affiliated with or endorsed by Nintendo.

## Project File

[**Open / download the Cisco Packet Tracer project**](./Cisco%20Practical%20Engineering%20project.pkt)

> Requires **Cisco Packet Tracer** to open the `.pkt` file.

## Project Goals

- Design a scalable multi-site enterprise network.
- Segment departments using VLANs and subnetting.
- Provide communication between VLANs, buildings, and branches.
- Configure dynamic routing between network segments and sites.
- Implement Layer 2 and Layer 3 security controls.
- Add redundancy to improve network availability.
- Configure common enterprise network services.
- Validate connectivity and network configuration using Cisco IOS commands.

## Technologies & Features

### Routing & Switching

- VLANs
- VTP
- 802.1Q trunking
- Inter-VLAN routing
- Router-on-a-Stick
- Layer 3 switching
- Static routing
- EIGRP
- OSPF
- BGP
- DHCP
- IP Helper
- NAT
- Passive interfaces

### Layer 2 Resiliency

- STP
- PVST load balancing
- BPDU Guard
- Root Guard
- Redundant switching paths

### Security

- Port Security
- Access Control Lists (ACLs)
- SSH
- AAA
- RADIUS
- TACACS+
- VPN
- Secure device-management configuration

### Network Services

- DNS
- DHCP
- HTTP
- FTP
- Mail
- Syslog
- NTP

### Availability

- First-hop / standby gateway redundancy
- Redundant network paths

## High-Level Topology

```text
                       Enterprise WAN
                            |
          +-----------------+-----------------+
          |                 |                 |
        Kyoto             Paris            Redmond
        Japan             France             USA
          |                 |                 |
      Multiple          Multiple          Multiple
      buildings         buildings         buildings
          |                 |                 |
     VLANs / Users     VLANs / Users     VLANs / Users
```

Each site uses routers, multilayer switches, access switches, end devices, servers, and multiple VLANs representing different organizational network segments.

## Configuration Areas

The project includes hands-on configuration of:

- VLAN creation and access-port assignment
- VTP server, client, and transparent modes
- Trunk links between switches
- Inter-VLAN routing
- Dynamic route advertisement
- Layer 3 switching
- ACL-based traffic control
- Port Security and MAC restrictions
- Secure SSH management
- NAT inside/outside interfaces
- DHCP and IP Helper
- Gateway redundancy
- Routing protocol verification

## Validation & Troubleshooting

The network was validated using Cisco IOS verification commands and end-to-end connectivity testing.

Examples include:

```text
show vlan brief
show vtp status
show port-security
show port-security address
show ip eigrp topology
show ip eigrp neighbors
```

Connectivity was tested between permitted VLANs, network segments, and branch locations.

## How to Run

1. Install **Cisco Packet Tracer**.
2. Clone this repository or download the `.pkt` file.
3. Open `Cisco Practical Engineering project.pkt`.
4. Allow routing and switching protocols to converge.
5. Inspect routers, switches, servers, VLANs, and routing tables.
6. Use Cisco IOS `show` commands and Packet Tracer simulation tools to explore and test the network.

```bash
git clone https://github.com/Dnrxiel/Packet-Tracer.git
```

## What I Learned

This project gave me practical experience with:

- Enterprise network design
- IP addressing and subnetting
- Routing and switching
- VLAN-based network segmentation
- Dynamic routing protocols
- Network redundancy
- Access control and network security
- Enterprise network services
- Troubleshooting and configuration verification

## Author

**Daniel Aptekarev**  
ICT Practical Engineer
