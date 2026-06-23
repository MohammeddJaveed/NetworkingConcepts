# Networking Cheatsheet

## Core Concepts

| Concept | Quick Meaning |
| --- | --- |
| IP address | Internet Protocol address; logical address for network communication |
| MAC address | Media Access Control address; local hardware address |
| Subnet | Smaller network inside a larger network |
| Router | Connects different networks |
| Switch | Connects devices in the same LAN |
| Firewall | Allows or blocks traffic |
| DNS | Domain Name System; converts names to IP addresses |
| DHCP | Dynamic Host Configuration Protocol; automatically assigns network settings |
| NAT | Network Address Translation; translates private addresses to public addresses |

## OSI Layers

| Layer | Name | Example |
| ---: | --- | --- |
| 7 | Application | HTTP, DNS |
| 6 | Presentation | TLS, encoding |
| 5 | Session | Session management |
| 4 | Transport | TCP, UDP |
| 3 | Network | IP, ICMP |
| 2 | Data Link | Ethernet, WiFi |
| 1 | Physical | Cable, fiber, radio |

## Private IPv4 Ranges

| Range | CIDR |
| --- | --- |
| `10.0.0.0` to `10.255.255.255` | `10.0.0.0/8` |
| `172.16.0.0` to `172.31.255.255` | `172.16.0.0/12` |
| `192.168.0.0` to `192.168.255.255` | `192.168.0.0/16` |

## Quick Troubleshooting Order

1. Physical connection or WiFi
2. IP address and subnet mask
3. Default gateway
4. DNS resolution
5. Route table
6. Firewall or security group
7. Listening port
8. Application logs
