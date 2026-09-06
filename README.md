**Networking Project **

Secure Multi-Department Office Network
Network Security and Segmentation Project
Project: Contip Solutions – Network Design & Security

**Tool Used:**
Cisco Packet Tracer

Focus: Network Design, IP Addressing, Connectivity Testing & Access Control

A Cisco Packet Tracer networking project demonstrating enterprise network design, subnetting, inter-network routing, DHCP/DNS services, connectivity testing, and access control. The project focuses on applying practical cybersecurity principles through network segmentation and Access Control Lists (ACLs).

**Project Overview**

The project was developed using Cisco Packet Tracer to design and configure a segmented enterprise network consisting of separate IT, HR, and Sales departments.

**The main objectives:**

Design separate departmental LANs using appropriate IP addressing.
Configure a Cisco 2911 router for inter-network communication.
Configure Cisco 2960 switches to provide Layer 2 connectivity.
Implement DHCP and DNS services.
Configure clients to obtain network settings automatically.
Test connectivity between departmental networks.
Implement an extended Access Control List (ACL) to restrict unauthorised communication.
Apply cybersecurity principles such as network segmentation and Least Privilege.
Network Topology

The network consists of three independent departmental LANs connected through a central Cisco router.

Department	Network	Purpose
IT	192.168.10.0/24	IT resources and DHCP/DNS server
HR	192.168.20.0/24	Human Resources network
Sales	192.168.30.0/24	Sales network

**Network Devices**
1 × Cisco 2911 Router – Provides inter-network routing.
3 × Cisco 2960 Switches – Provide Layer 2 connectivity for each department.
End-user PCs – Connected to the departmental switches.
DHCP/DNS Server – Located within the IT department.

The three departmental networks are logically separated into independent LANs. The router enables communication between the networks while the ACL controls which traffic is permitted.

**Tools and Technologies**
Cisco Packet Tracer – Network design, configuration, and simulation.
Cisco 2911 Router – Inter-network routing.
Cisco 2960 Switches – Layer 2 network connectivity.
DHCP – Automatic allocation of IP addresses and network configuration.

DNS – Name resolution services.
IPv4 Subnetting – Departmental network segmentation.
Extended ACLs – Network traffic filtering and access control.
Ping – Connectivity and troubleshooting testing.
Network Segmentation – Separation of departmental resources.
Principle of Least Privilege – Restriction of access to sensitive resources.

**Configuration Steps**
Designed the network topology in Cisco Packet Tracer using one Cisco 2911 router and three Cisco 2960 switches.
Created separate departmental networks:
IT: 192.168.10.0/24
HR: 192.168.20.0/24
Sales: 192.168.30.0/24

Connected the departmental switches to the Cisco 2911 router to enable communication between the different LANs.
Configured IP addressing for the network devices and end-user computers.
Configured the DHCP service on the IT server so that client devices could automatically obtain:

IP addresses
Subnet masks
Default gateways
DNS server information
Configured DNS services on the IT server to provide name-resolution functionality.
Configured router interfaces to provide gateways for the three departmental networks.

Tested DHCP functionality by verifying that client devices successfully received their network configuration automatically.
Performed connectivity testing using ping between devices on different departmental networks.

Verified inter-network routing by successfully testing connectivity from the Sales network to the IT network.

Configured an extended ACL on the router to deny traffic originating from the HR subnet to the IT subnet.

Configured the ACL to permit other legitimate traffic, ensuring that the security control did not unnecessarily disrupt business communications.

Tested the ACL configuration by attempting communication from HR to IT and confirming that the traffic was blocked.

Validated the security policy by comparing connectivity before and after applying the ACL.

**Results and Findings**
The project successfully demonstrated the implementation of a segmented enterprise network with controlled communication between departments.

**Key Results**
DHCP configuration was successful, with client devices automatically receiving the required network parameters.
DNS services were configured within the IT network.
Inter-network routing was operational, demonstrated by successful ping connectivity from Sales to IT.
The ACL successfully blocked HR-to-IT traffic after implementation.
Other permitted network traffic remained available.
Network segmentation helped isolate departmental resources.
The ACL demonstrated the Principle of Least Privilege by restricting HR access to sensitive IT resources while allowing legitimate communications elsewhere.
Cybersecurity Significance

This project demonstrates practical cybersecurity and networking skills, including:

Network segmentation
IPv4 addressing and subnetting
Router configuration
Switch configuration
DHCP/DNS implementation
Network troubleshooting
Traffic filtering
Access Control Lists
Least Privilege
Secure network design

Overall, the project demonstrates how network infrastructure can be designed with security controls that limit unauthorised access while maintaining required business connectivity.

Author

Faith Ejele

Cybersecurity – Cohort July 2026
Focus: Cybersecurity and Network Security
Project: Enterprise Network Segmentation and ACL Implementation
