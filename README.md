# Networking Fundamentals

This repository is a structured learning path for networking fundamentals. It is written for DevOps, cloud, system administration, Kubernetes, and system design learners who need clear explanations with practical examples.

Most lessons include Mermaid diagrams. GitHub renders Mermaid blocks as visual diagrams, so the notes can be read directly in the browser.

## Learning Path

Read the folders in order:

1. [Network Basics](01-network-basics)
2. [IP Addressing](02-ip-addressing)
3. [VPC Networking](03-vpc-networking)
4. [Ports and Protocols](04-ports-and-protocols)
5. [DNS](05-dns)
6. [DHCP](06-dhcp)
7. [TCP Handshake](07-tcp-handshake)
8. [Interview Questions](08-interview-questions)
9. [Cheatsheets](cheatsheets)
10. [Diagrams](diagrams)
11. [Glossary](glossary.md)

## Topics Covered

### 01 - Network Basics

- [What is Networking?](01-network-basics/01-what-is-networking.md)
- [OSI Model](01-network-basics/osi-model.md)
- [TCP/IP Model](01-network-basics/tcp-ip-model.md)

### 02 - IP Addressing

- [IP Address](02-ip-addressing/01-ip-address.md)
- [Public IP vs Private IP](02-ip-addressing/02-public-vs-private-ip.md)
- [Subnetting](02-ip-addressing/03-subnetting.md)
- [CIDR Notation](02-ip-addressing/04-cidr-notation.md)
- [IP Addressing Examples](02-ip-addressing/05-examples.md)

### 03 - VPC Networking

- [VPC](03-vpc-networking/01-vpc.md)
- [Public Subnet](03-vpc-networking/02-public-subnet.md)
- [Private Subnet](03-vpc-networking/03-private-subnet.md)
- [Route Tables](03-vpc-networking/04-route-tables.md)
- [Internet Gateway](03-vpc-networking/05-internet-gateway.md)
- [NAT Gateway](03-vpc-networking/06-nat-gateway.md)

### 04 - Ports and Protocols

- [Ports](04-ports-and-protocols/01-ports.md)
- [TCP](04-ports-and-protocols/02-tcp.md)
- [UDP](04-ports-and-protocols/03-udp.md)
- [Common Protocols](04-ports-and-protocols/04-common-protocols.md)

### 05 - DNS

- [What is DNS?](05-dns/01-what-is-dns.md)
- [DNS Resolution](05-dns/02-dns-resolution.md)
- [DNS Record Types](05-dns/03-dns-record-types.md)

### 06 - DHCP

- [What is DHCP?](06-dhcp/01-what-is-dhcp.md)
- [DHCP DORA Process](06-dhcp/02-dhcp-dora-process.md)

### 07 - TCP Handshake

- [TCP Three-Way Handshake](07-tcp-handshake/01-three-way-handshake.md)
- [TCP Connection Termination](07-tcp-handshake/02-connection-termination.md)
- [TCP Troubleshooting](07-tcp-handshake/03-tcp-troubleshooting.md)

### 08 - Interview Questions

- [Networking Interview Questions](08-interview-questions/01-networking-questions.md)
- [Scenario-Based Questions](08-interview-questions/02-scenario-questions.md)

### Cheatsheets and Diagrams

- [Networking Cheatsheet](cheatsheets/networking-cheatsheet.md)
- [Port Cheatsheet](cheatsheets/ports-cheatsheet.md)
- [Home Network Diagram](diagrams/home-network.md)
- [Cloud VPC Diagram](diagrams/cloud-vpc.md)

### Reference

- [Glossary of Networking Abbreviations](glossary.md)

## What You Should Understand After Reading

- How devices communicate across local networks and the internet
- How OSI and TCP/IP layers organize network communication
- How IPv4, IPv6, CIDR, and subnetting work
- Difference between public and private IP addresses
- How VPCs, subnets, route tables, internet gateways, and NAT gateways work
- How ports, TCP, UDP, DNS, and DHCP support real applications
- How to reason through common troubleshooting and interview scenarios

## Recommended Practice

- Draw the packet path for a browser opening a website.
- Calculate subnet sizes from CIDR notation.
- Explain why a private subnet can access the internet through NAT but cannot be reached directly from the internet.
- Memorize common ports, but also understand why each protocol uses them.
- Practice troubleshooting from Layer 1 upward before blaming the application.
- Use the [glossary](glossary.md) whenever an abbreviation is unfamiliar.
