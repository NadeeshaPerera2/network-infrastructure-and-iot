# Network Infrastructure and IoT

A practical Cisco Packet Tracer network infrastructure project demonstrating VLAN segmentation, IP addressing, switching, inter-VLAN routing, network troubleshooting, and IoT integration through the design and simulation of a structured network environment.

##  Project Overview

This project was developed to apply networking and IoT concepts in a practical Cisco Packet Tracer environment.

The project focuses on designing, configuring, testing, and troubleshooting a structured network containing separate user, server, and NOC segments, together with a  Smart Office IoT implementation.

##  Network Architecture

The network follows a structured topology:

EDGE-R1 → CORE-SW1 → Access Switches

Access switches:

- USER-SW1
- SERVER-SW1
- NOC-SW1

Connected endpoints include:

- User PCs
- Server PCs
- NOC PCs
- IoT Control PC
- Smart Office IoT Gateway
- Smart Light

##  VLAN and IP Addressing

| VLAN | Purpose | Network | Gateway |
|------|---------|---------|---------|
| VLAN 10 | Users | 192.168.10.0/24 | 192.168.10.1 |
| VLAN 20 | Servers | 192.168.20.0/24 | 192.168.20.1 |
| VLAN 30 | NOC | 192.168.30.0/24 | 192.168.30.1 |

The VLAN structure provides logical separation between different network segments.

##  Routing and Switching

The project implements:

- VLAN configuration
- Access port configuration
- Trunk links
- IPv4 addressing
- Switch management addressing
- Router-on-a-Stick configuration
- Inter-VLAN routing
- ICMP connectivity testing

##  NOC Troubleshooting Scenarios

Three controlled network incidents were introduced and resolved as part of the project.

### Incident 01 — User Connectivity Failure

A switch port connected to USER-PC1 was disabled.

Troubleshooting process:

1. Identified the connectivity failure.
2. Verified the PC IP configuration.
3. Checked the switch port status.
4. Identified the disabled interface.
5. Restored the interface.
6. Retested connectivity successfully.

### Incident 02 — Server Connectivity Failure

The switch port connected to SERVER-PC1 was disabled.

The issue was identified through connectivity testing and switch interface verification.

The interface was restored and connectivity was successfully retested.

### Incident 03 — Incorrect VLAN Assignment

USER-PC2 was incorrectly assigned to the Server VLAN.

The issue was identified by checking the switch port VLAN configuration.

The port was returned to VLAN 10 and connectivity was successfully restored.

These scenarios demonstrate a structured troubleshooting approach:

**Symptom → Verification → Root Cause → Resolution → Retesting**

##  IoT Implementation

A basic Smart Office IoT environment was implemented using Cisco Packet Tracer.

### IoT Components

- SMART-OFFICE-GW
- IOT-CONTROL-PC
- SMART-LIGHT-01

### IoT Configuration

The implementation includes:

- Smart Office wireless network
- SSID: `SmartOffice-IoT`
- Wireless connectivity
- DHCP addressing
- Home Gateway IoT server
- Smart device registration
- Remote smart-light control

The smart light was successfully controlled through the Home Gateway, including:

- ON
- DIM
- OFF

##  Testing and Validation

The completed network was tested using ICMP connectivity tests.

Examples of verified connectivity include:

- User PC → Default Gateway
- User PC → Server VLAN
- User PC → NOC VLAN
- IoT Control PC → IoT Gateway
- IoT Control PC → Smart Light

Final connectivity tests were successfully completed with 0% packet loss on the verified connections.

##  Technologies and Tools

- Cisco Packet Tracer
- Cisco Networking concepts
- VLANs
- IPv4 addressing
- Switching
- Trunking
- Router-on-a-Stick
- Inter-VLAN Routing
- Network Troubleshooting
- Wireless Networking
- Internet of Things (IoT)

##  Project File

The complete Cisco Packet Tracer simulation is available in:

`NOC_Network_Lab.pkt`

Open the file using Cisco Packet Tracer to explore the network topology, configurations, troubleshooting scenarios, and IoT implementation.

##  Project Objective

The main objective of this project was to move beyond theoretical learning and apply networking and IoT concepts through practical network design, configuration, troubleshooting, testing, and validation.
