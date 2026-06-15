# Enterprise Trading Floor Network Infrastructure Design

## Overview

This project demonstrates the design and implementation of a highly available enterprise campus network for a trading floor support organization with approximately 600 employees.

The organization is relocating to a new three-story office building and requires a modern network infrastructure capable of supporting business operations, wireless connectivity, centralized services, redundancy, and future growth.

The solution was designed using Cisco Packet Tracer and follows enterprise network design principles including hierarchical architecture, network segmentation, dynamic routing, redundancy, centralized services, and network security.

---

## Business Scenario

A trading floor support center is relocating its operations into a new three-floor office building. The objective is to deploy a scalable and resilient network infrastructure capable of supporting multiple business departments while ensuring high availability and secure communication.

The network was designed to provide:

* Departmental network segmentation
* Wireless connectivity
* Redundant routing infrastructure
* Centralized DHCP services
* Dynamic routing
* Secure remote administration
* Internet redundancy through dual ISPs
* Network security controls

---

## Department Structure

### First Floor

#### Sales and Marketing Department

* 25 Users

#### Human Resources and Logistics Department

* 25 Users

---

### Second Floor

#### Finance and Accounts Department

* 25 Users

#### Administration and Public Relations Department

* 25 Users

---

### Third Floor

#### Information Technology Department

* 25 Users

#### Server Room

* 25 Devices

---

## Network Architecture

The solution follows a hierarchical enterprise network model.

### Core Layer

* Router 1
* Router 2
* ISP Provider 1
* ISP Provider 2

### Distribution Layer

* Multilayer Switch 1
* Multilayer Switch 2

### Access Layer

* Departmental Access Switches
* Wireless Access Points

### Server Infrastructure

The server room hosts:

* DHCP Server
* Network Management Services
* Internal Enterprise Services

---

## Technologies Implemented

### Enterprise Network Design

* Hierarchical Network Design
* Redundant Infrastructure
* Campus Network Architecture

### Switching Technologies

* VLAN Segmentation
* Inter-VLAN Routing
* Switch Virtual Interfaces (SVIs)

### Routing Technologies

* OSPF Dynamic Routing
* Default Routing

### Security Technologies

* SSH Remote Administration
* Port Security
* Access Control Lists (ACLs)

### Internet Technologies

* NAT Overload (PAT)
* Dual ISP Connectivity

### Wireless Technologies

* Departmental Wireless Networks
* Cisco Access Points

### Network Services

* DHCP Services
* Centralized Address Management

---

## VLAN Design

Each department was placed in an independent VLAN to improve security, performance, and network management.

| VLAN    | Department                          |
| ------- | ----------------------------------- |
| VLAN 10 | Sales and Marketing                 |
| VLAN 20 | HR and Logistics                    |
| VLAN 30 | Finance and Accounts                |
| VLAN 40 | Administration and Public Relations |
| VLAN 50 | Information Technology              |
| VLAN 60 | Server Room                         |

---

## IP Addressing Plan

### Base Network

172.16.1.0/24

Subnetting was performed to allocate separate address spaces to each department while allowing room for future expansion.

Example allocation:

| Department               | Network         |
| ------------------------ | --------------- |
| Sales & Marketing        | 172.16.1.0/27   |
| HR & Logistics           | 172.16.1.32/27  |
| Finance & Accounts       | 172.16.1.64/27  |
| Admin & Public Relations | 172.16.1.96/27  |
| IT Department            | 172.16.1.128/27 |
| Server Room              | 172.16.1.160/27 |

---

## Public Addressing

The enterprise Internet edge was configured using the following public address ranges:

* 195.136.17.0/30
* 195.136.17.4/30
* 195.136.17.8/30
* 195.136.17.12/30

These links provide Internet redundancy through two independent service providers.

---

## Security Implementation

### SSH

Secure remote management was configured on:

* Routers
* Layer 3 Switches

### Port Security

Finance and Accounts switch ports were secured using:

* Sticky MAC Learning
* Maximum One MAC Address
* Violation Mode Shutdown

This protects sensitive financial systems from unauthorized device connections.

### Access Control

ACLs were implemented to support:

* NAT functionality
* Traffic filtering
* Administrative security controls

---

## High Availability Features

* Dual Core Routers
* Dual Layer 3 Switches
* Dual ISP Connections
* OSPF Dynamic Routing
* Redundant Layer Design

These features reduce single points of failure and improve network resilience.

---

## Services Implemented

### DHCP

A centralized DHCP server provides:

* Dynamic IP Assignment
* Gateway Configuration
* DNS Distribution

### Inter-VLAN Routing

Multilayer switches perform:

* Layer 2 Switching
* Layer 3 Routing
* VLAN Gateway Services

### NAT Overload (PAT)

Internal users share public IP addresses for Internet access while preserving public address space.

---

## Testing and Verification

The following tests were completed successfully:

* VLAN Connectivity Testing
* Inter-VLAN Routing Verification
* DHCP Address Assignment
* OSPF Neighbor Formation
* Internet Connectivity Testing
* NAT Translation Verification
* Wireless Client Connectivity
* SSH Remote Login Testing
* Port Security Validation
* End-to-End Communication Testing

All configured services were verified and functioned as expected.

---

## Skills Demonstrated

* Enterprise Campus Network Design
* VLAN Design and Segmentation
* Layer 3 Switching
* Inter-VLAN Routing
* OSPF Routing
* DHCP Administration
* NAT/PAT Configuration
* SSH Hardening
* Port Security Implementation
* Wireless Network Deployment
* High Availability Design
* Cisco Packet Tracer
* Network Troubleshooting

---

## Repository Structure

```text
enterprise-trading-floor-network/
│
├── README.md
├── Trading_Floor_Network.pkt
├── Trading_Floor_Report.pdf
├── topology.png

```


---

## Author

Chibuike Obika

Enterprise Network Engineering Portfolio Project
