Cisco Packet Tracer Enterprise Network

A multi-branch enterprise network designed and implemented in Cisco Packet Tracer as part of my ICT Practical Engineering final project.

The project simulates a Nintendo enterprise network connecting three geographic branches:

Kyoto, Japan

Paris, France

Redmond, USA

Each branch contains multiple network segments/buildings and uses routing, switching, security, network services, and redundancy technologies to model a realistic enterprise environment.

Note: This is an educational project. It is not affiliated with or endorsed by Nintendo.

Project Goals

Design a scalable multi-site enterprise network.

Segment users and departments using VLANs and subnetting.

Provide communication between VLANs, buildings, and geographic branches.

Implement dynamic routing and redundant network paths.

Apply Layer 2 and Layer 3 security controls.

Configure common enterprise network services.

Test and validate connectivity and network configuration.

Technologies and Features

Routing and Switching

VLANs

VTP

802.1Q trunking

Inter-VLAN routing

Router-on-a-Stick

Layer 3 switching

Static routing

EIGRP

OSPF

BGP

DHCP

IP Helper

Passive interfaces

NAT

Layer 2 Resiliency

STP

PVST load balancing

BPDU Guard

Root Guard

Redundant switching paths

Security

Port Security

ACLs

SSH

AAA

RADIUS

TACACS+

VPN

Secure management configuration

Network Services

The simulated environment includes several common enterprise services:

DNS

DHCP

HTTP

FTP

Mail

Syslog

NTP

Gateway / Availability

Standby gateway configuration is used to provide first-hop redundancy and improve network availability.

Network Topology

The network is divided into three main geographic sites:

                    Enterprise WAN
                         |
        +----------------+----------------+
        |                |                |
      Kyoto            Paris           Redmond
      Japan            France            USA
        |                |                |
   Multiple          Multiple          Multiple
   buildings         buildings         buildings
        |                |                |
  VLANs / Users     VLANs / Users     VLANs / Users

Each site contains multiple VLANs representing different organizational departments and uses routers, multilayer switches, access switches, end devices, and servers.

Example Configuration Areas

The project includes configurations for:

VLAN creation and access-port assignment

VTP server/client/transparent modes

Trunk links between switches

Inter-VLAN routing

Dynamic route advertisement

Access-control rules

Port Security and MAC restrictions

Secure SSH management

NAT inside/outside interfaces

DHCP addressing

Gateway redundancy

Routing protocol verification

Validation and Troubleshooting

Configurations were validated using Cisco IOS commands and connectivity tests, including examples such as:

show vlan brief
show vtp status
show port-security
show port-security address
show ip eigrp topology
show ip eigrp neighbors

End-to-end connectivity was also tested between permitted network segments and branches.

How to Run the Project

Install Cisco Packet Tracer.

Clone or download this repository.

Open the included .pkt Packet Tracer project file.

Allow the topology to converge after opening.

Inspect the routers, switches, servers, VLANs, and routing tables.

Use Packet Tracer simulation tools and Cisco IOS commands to test connectivity and configuration.

What I Learned

This project gave me hands-on experience designing a larger enterprise network and working with:

IP addressing and subnetting

Routing and switching

Enterprise network segmentation

Dynamic routing protocols

Network redundancy

Access control and network security

Network services

Troubleshooting and configuration verification

Author

Daniel Aptekarev
ICT Practical Engineer

