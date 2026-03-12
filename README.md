# Multi-Site Enterprise Network Design and Simulation

This project presents a scalable enterprise network designed and implemented in Cisco Packet Tracer for an agricultural cooperative 
with 8 branch sites and a central data centre. The design focuses on scalability, efficient IP address allocation, dynamic routing, WAN connectivity, 
and security planning.

## Project Overview

The network was designed using the 107.6.2.0/23 address block and structured to support current users as well as future growth. Variable Length Subnet Masking (VLSM) was used to allocate IP space efficiently across branch LANs, WAN links, and the data centre, with additional reserved subnet blocks and WAN links included for expansion.

Since Cisco Packet Tracer does not natively support MPLS, the WAN portion of the design was simulated using an interconnected cluster of service-provider routers to represent MPLS-style any-to-any connectivity. OSPF was configured as the routing protocol to provide dynamic end-to-end communication across the network.

## Key Features

- Designed a multi-site enterprise network connecting 8 branch sites and a central data centre.
- Applied VLSM subnetting to allocate IPv4 addresses efficiently based on site size and future growth.
- Reserved additional subnet blocks and WAN links for scalability.
- Simulated MPLS-style WAN connectivity using a service-provider router cloud in Packet Tracer.
- Configured OSPF for dynamic routing across branch routers and the simulated provider network.
- Assigned first usable IP addresses as default gateways for each site router.
- Verified inter-site communication and remote web access to the data centre server.
- Performed a security risk assessment covering Zero Trust principles and enterprise security controls.

## Network Design Goals

The project was developed around four main design goals:

- **Scalability:** Support future network growth with reserved address space and WAN capacity.
- **Efficiency:** Use VLSM to avoid wasting IP addresses.
- **Availability and Redundancy:** Simulate resilient WAN connectivity and maintain management access through console backup access.
- **Security:** Isolate the data centre and propose layered security controls for enterprise protection.

## Technologies Used

- Cisco Packet Tracer
- IPv4 addressing and VLSM subnetting
- OSPF dynamic routing
- MPLS-style WAN simulation
- Basic HTTP connectivity testing
- Network security analysis

## Security Considerations

The project also includes a security-focused design review. Key controls proposed in the report include:

- Zero Trust architecture
- IPsec-over-MPLS for WAN confidentiality
- IEEE 802.1X for device authentication
- Next-Generation Firewall (NGFW) for application-aware filtering and intrusion prevention
- TACACS+ for secure administrative access
- Full-Disk Encryption (FDE) and endpoint protection controls

## Testing and Validation

The implemented Packet Tracer network was tested to verify full end-to-end connectivity. Validation included successful ping tests between remote sites and successful HTTP access from a branch site to the web server hosted in the data centre.

## Repository Contents

- `multi-site-enterprise-network.pkt` — Cisco Packet Tracer project file
- `README.md` — project overview and documentation
- `topology.png` — optional screenshot of the network topology
- `report.pdf` — optional full project report

## How to Open

1. Download the `.pkt` file from this repository.
2. Open it in Cisco Packet Tracer.
3. Review the branch sites, data centre, WAN links, and service-provider cloud design.
4. Test connectivity using ping and HTTP from branch PCs to the data centre server.

## Learning Outcomes

Through this project, I strengthened my understanding of:

- Enterprise IP addressing and subnet planning
- VLSM-based network design
- Dynamic routing with OSPF
- WAN design concepts and MPLS-style connectivity
- Network verification and troubleshooting
- Security design principles for enterprise networks

## Notes

This project simulates MPLS-style connectivity conceptually because Cisco Packet Tracer does not provide native MPLS support. OSPF was used as the practical routing mechanism to enable the network simulation.
