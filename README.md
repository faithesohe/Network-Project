**Project: Enterprise Network Segmentation and ACL Implementation**
 
Contip Solutions – Secure Multi-Department Office Network

**Tool Used:** Cisco Packet Tracer  
**Project Type:** Networking & Cybersecurity  
**Focus:** Network Design | IPv4 Addressing | Subnetting | Routing | DHCP/DNS | Network Segmentation | Access Control Lists (ACLs) | Connectivity Testing

---
## Project Overview

This project demonstrates the design, configuration, and security of a **multi-department enterprise network** for **Contip Solutions** using Cisco Packet Tracer.

The network was designed to support three departments:

- **IT Department**
- **HR Department**
- **Sales Department**

Each department operates on a separate IPv4 network, providing logical network segmentation and simplifying network management.

A **Cisco 2911 router** provides inter-network communication between the departmental LANs, while **Cisco 2960 switches** provide Layer 2 connectivity within each department.

The project also implements **DHCP, DNS, inter-network routing, connectivity testing, and an extended Access Control List (ACL)** to demonstrate how networking and cybersecurity controls can be combined to provide secure business connectivity.

---
**Problem Statement**

As Contip Solutions expanded its operations, the organisation required a more structured and secure network infrastructure.
The network requirements presented several challenges:

- No structured communication between departments
- No organised IP addressing scheme
- Difficulty managing and troubleshooting network devices
- Limited network scalability
- No access-control mechanism to protect sensitive departmental resources
- Increased security risk from unrestricted inter-department communication

A segmented network architecture was therefore required to provide reliable communication while protecting sensitive resources from unauthorised access.

**Project Objectives**

The objectives of the project were to:

- Design separate LANs for the **IT, HR, and Sales departments**
- Implement a structured IPv4 addressing scheme
- Configure a **Cisco 2911 router** for inter-network communication
- Configure **Cisco 2960 switches** for Layer 2 connectivity
- Implement **DHCP** for automatic client network configuration
- Configure **DNS** for name resolution
- Configure end-user devices to obtain network settings automatically
- Test communication between departmental networks
- Implement an **extended ACL** to restrict unauthorised traffic
- Apply **Network Segmentation** and the **Principle of Least Privilege**
- Test and validate both network connectivity and security controls

**Project Outcome**

The completed solution provides Contip Solutions with a structured, manageable, scalable, and more secure network infrastructure.

The three departments operate on separate IPv4 networks while the Cisco router provides controlled communication between them.

The extended ACL strengthens the network's security posture by preventing HR users from accessing IT resources while allowing other authorised communication.

Through this project, I gained practical hands-on experience in:

Network topology design
IPv4 addressing and subnetting
Cisco router configuration
Cisco switch configuration
Inter-network routing
DHCP and DNS services
Network segmentation
Extended ACL implementation
Traffic filtering
Connectivity testing
Network troubleshooting
Secure network architecture
---

## Proposed Solution

I designed and configured a **routed and segmented network architecture** in Cisco Packet Tracer.

The organisation was divided into three separate `/24` departmental networks:

| Department | Network | Purpose |
|---|---|---|
| **IT** | `192.168.10.0/24` | IT and administrative resources |
| **HR** | `192.168.20.0/24` | Human Resources users and resources |
| **Sales** | `192.168.30.0/24` | Sales users and resources |

Each department connects to a dedicated Cisco 2960 switch. The three switches connect to a central Cisco 2911 router, which provides Layer 3 communication between the networks.

The IT network also hosts infrastructure services, including:

- **DHCP:** `192.168.10.2`
- **DNS:** `192.168.10.3`
- Administrative/server resources

An **extended ACL** was implemented on the router to prevent the HR network from accessing the IT network while allowing other authorised traffic.

---

## Network Topology

![Contip Solutions Network Topology](images/network-topology.png)

The topology consists of three logically separated departmental LANs connected through a central **Cisco 2911 router**.

### IT Department

- Network: `192.168.10.0/24`
- Admin Server
- IT-Sheila
- IT-Tony
- DHCP and DNS services

### HR Department

- Network: `192.168.20.0/24`
- HR-Wale
- HR-Bimbo

### Sales Department

- Network: `192.168.30.0/24`
- Sales-Tom
- Sales-Mary

This architecture separates departmental resources while allowing the router to provide controlled communication between the three networks.

---

## Network Devices

| Device | Quantity | Function |
|---|---:|---|
| **Cisco 2911 Router** | 1 | Routes traffic between departmental networks and enforces ACL rules |
| **Cisco 2960 Switch** | 3 | Provides Layer 2 connectivity for each department |
| **Server** | 1 | Provides administrative/network services |
| **End-User PCs** | 6 | Represents IT, HR, and Sales users |

---

## Tools and Technologies

- **Cisco Packet Tracer** – Network design, configuration, simulation, and testing
- **Cisco 2911 Router** – Inter-network routing and ACL implementation
- **Cisco 2960 Switches** – Layer 2 network connectivity
- **IPv4 Addressing** – Addressing network devices and interfaces
- **/24 Subnetting** – Logical separation of departmental networks
- **TCP/IP** – Network communication
- **DHCP** – Automatic client network configuration
- **DNS** – Name-resolution services
- **Routing** – Communication between separate departmental networks
- **Extended ACLs** – Traffic filtering and access control
- **ICMP/Ping** – Connectivity testing and troubleshooting
- **Network Segmentation** – Separation of departmental resources
- **Principle of Least Privilege** – Restricting unnecessary access to sensitive resources

---

## Network Configuration and Implementation

### 1. Network Topology Design

The network topology was designed in Cisco Packet Tracer using:

- One Cisco 2911 router
- Three Cisco 2960 switches
- Six end-user PCs
- Server infrastructure

Each department was connected to a dedicated switch to provide logical separation.

### 2. IPv4 Addressing and Network Segmentation

Separate `/24` networks were assigned to each department:

```text
IT Department:     192.168.10.0/24
HR Department:     192.168.20.0/24
Sales Department:  192.168.30.0/24


This addressing structure improves network organisation and makes the infrastructure easier to manage, troubleshoot, secure, and scale.

Router Configuration
The three departmental switches were connected to separate interfaces on the Cisco 2911 router.
The router interfaces were configured to provide the appropriate **default gateways** for each network and enable communication between the departmental LANs.

DHCP Configuration
DHCP services were configured so that client devices could automatically obtain:

-  IP address 
-  Subnet mask 
-  Default gateway 
-  DNS server information 
DHCP functionality was verified by confirming that client devices successfully received their network configurations automatically.
DNS Configuration-DNS services were configured to provide **name-resolution functionality** within the network.

Inter-Network Routing
The Cisco 2911 router was configured to route traffic between the IT, HR, and Sales networks.
Connectivity was tested using the `ping` command between devices on different departmental networks.
Successful communication from the **Sales network to the IT network** confirmed that inter-network routing was functioning correctly.

Conclusion

The Contip Solutions Secure Multi-Department Office Network project demonstrates the practical design, configuration, testing, and security of a segmented enterprise network using Cisco Packet Tracer.

The solution successfully separates the IT, HR, and Sales departments, provides inter-network routing and essential network services, and implements an extended ACL to prevent unauthorised HR access to IT resources.

The project demonstrates an important cybersecurity principle: a secure network should not simply provide connectivity; it should provide controlled connectivity.

Author
Faith Ejele

Focus: Cybersecurity and Network Security

