# ESIGELEC Hospital Network Design

A comprehensive network infrastructure design project for a modern hospital environment, simulated using Cisco Packet Tracer.

---

## Project Overview

This project presents a secure, scalable, and high-performance network architecture designed specifically for healthcare environments. The implementation addresses critical requirements including HIPAA compliance, high availability, real-time data transfer, and integration of diverse medical systems.

> **Course**: Fundamentals of Data Communication and Networking  
> **Institution**: ESIGELEC - Department of Software Engineering

---

## Team Members

| Name | Role |
|------|------|
| Asogwa Chi-Uba | Network Architect |
| Pranav Kumar | Network Administrator |
| Richard Antoine Iroudayaradjou | IT Support Specialist |
| Jie Pengyu | Network Security Specialist |

---

## Network Architecture

### Three-Tier Hierarchical Model

The network implements a hierarchical three-tier architecture designed to balance scalability, security, and performance:

> **Core Layer**  
> High-capacity routers and switches ensuring fast, reliable inter-departmental data transfer with redundancy to minimize downtime.

> **Distribution Layer**  
> Layer 3 switches managing traffic flow, implementing VLANs, and enforcing Access Control Lists (ACLs) for security compliance.

> **Access Layer**  
> Layer 2 switches and wireless access points providing secure connectivity to end-user devices with port security.

### Network Components

**Core Infrastructure:**
- Cisco 2811 and Cisco 2911 Routers
- Cisco Multilayer 3650 Switches (Distribution Layer)
- Cisco 2960 Switches (Access Layer)
- Cisco Aironet 1815i Wireless Access Points

**Connectivity:**
- Dual ISP configuration with automatic failover
- Fiber optic and Category 6A UTP cabling
- 10-Gigabit Ethernet backbone

---

## Department Segmentation

The network architecture segments nine hospital departments using VLANs for enhanced security and traffic management:

| Department | VLAN ID |
|------------|---------|
| Administration and Support Department (ASD) | VLAN 10 |
| Medical and Surgical Department (MSD) | VLAN 20 |
| Diagnostic and Imaging Department (DID) | VLAN 30 |
| Therapeutic and Rehabilitation Department (TRD) | VLAN 40 |
| Special Care Department (SCD) | VLAN 50 |
| Patient and Family Support Department (PFSD) | VLAN 60 |
| Pharmacy Department (PD) | VLAN 70 |
| Infection Control and Epidemiology (ICE) | VLAN 80 |
| Visitors and Guests (VG) | VLAN 90 |

---

## Key Features

**High Availability**
- Dual ISP configuration with primary and backup providers
- Automatic failover mechanism to ensure minimal downtime
- Redundant core infrastructure

**Security**
- Multi-layered firewall protection
- Intrusion Detection and Prevention Systems (IDS/IPS)
- Access Control Lists (ACLs) on routers and switches
- SSH-only remote access
- WPA2-Enterprise wireless security with 802.1X authentication
- HIPAA-compliant security measures

**Scalability**
- Designed to support future departmental expansion
- Support for additional branch locations
- Flexible VLAN architecture

**Performance**
- 10-Gigabit Ethernet for high-bandwidth applications
- Optimized for medical imaging (PACS) systems
- Low-latency configuration for real-time applications

**Network Management**
- Dynamic Host Configuration Protocol (DHCP) for automated IP assignment
- OSPF routing protocol for efficient inter-VLAN routing
- Centralized server infrastructure with data, communication, and backup servers

---

## Technical Specifications

### Addressing Scheme

```
ISP Connections:    255.255.255.252 (/30) - 2 usable host addresses
Department VLANs:   255.255.255.128 (/25) - 62 usable host addresses per VLAN
```

### Protocols and Standards

**Network Protocols:**
- OSPF (Open Shortest Path First) for dynamic routing
- DHCP for IP address management
- SSH for secure remote administration

**Physical Standards:**
- IEEE 802.3 (Ethernet)
- IEEE 802.11ac (Wireless LAN)

**Security Protocols:**
- 802.1X (Port-based Network Access Control)
- WPA2-Enterprise (Wireless Security)

---

## Getting Started

### Prerequisites

- Cisco Packet Tracer (version 7.0 or higher)
- Basic understanding of networking concepts
- Familiarity with Cisco IOS command-line interface

### Installation and Setup

1. Clone this repository to your local machine
2. Open the `.pkt` file using Cisco Packet Tracer
3. Review the network topology and configuration
4. Explore device configurations using the CLI or GUI
5. Run simulation mode to observe packet flows

### Configuration Examples

The project includes detailed Cisco IOS configurations for:
- Layer 2 switch setup with VLAN assignment
- Layer 3 switch configuration with inter-VLAN routing
- OSPF routing protocol implementation
- DHCP server configuration
- SSH remote access setup
- Trunk port configuration

---

## Testing and Validation

### Network Testing Procedures

**Connectivity Testing:**
- Ping tests between departments to verify inter-VLAN routing
- Packet tracer simulation mode for visual packet flow analysis
- DHCP functionality verification across all VLANs

**Redundancy Testing:**
- ISP failover mechanism validation
- Load balancing verification
- Backup route confirmation

**Security Validation:**
- Access control list effectiveness
- Wireless authentication testing
- Port security verification

---

## Project Deliverables

> **Network Design Document**  
> Complete architectural design with rationale for technology choices

> **Implementation Guide**  
> Step-by-step configuration procedures with Cisco IOS commands

> **Testing Report**  
> Comprehensive testing results demonstrating network functionality

> **Future Recommendations**  
> Strategic roadmap for network enhancements and expansion

---

## Future Enhancements

**Telemedicine Integration**
- Remote patient monitoring systems
- Secure video conferencing infrastructure
- Mobile health device connectivity

**Advanced Security**
- AI-driven threat detection and response
- Enhanced intrusion prevention systems
- Regular penetration testing protocols

**Cloud Integration**
- Hybrid cloud architecture for data storage
- Cloud-based disaster recovery solutions
- Scalable computing resources

**Next-Generation Technologies**
- 5G network integration for enhanced connectivity
- IoT medical device management
- Smart hospital automation systems
- Advanced analytics and predictive healthcare

**EHR Enhancement**
- Improved interoperability between healthcare systems
- Standardized data exchange formats
- Secure API integration for third-party applications

---

## Documentation

Complete project documentation is available in `Proposed_Network_Architecture_Design.pdf`, which includes:
- Detailed architectural diagrams
- Comprehensive security considerations
- Complete configuration guides
- Testing methodologies and results
- Bibliography and references

---

## References

- Cisco Network Academy (NetAcad)
- Cisco Packet Tracer Documentation
- Healthcare Network Architecture Best Practices
- HIPAA Compliance Guidelines
- Network Design for Healthcare Applications Research

---

## Disclaimer

> **Important**: This is an academic project designed for educational purposes. For production healthcare networks, consult with certified network engineers and ensure full compliance with all relevant healthcare regulations and security standards.

---

## License

This project is submitted as part of academic coursework at ESIGELEC. All rights reserved by the project team members.
