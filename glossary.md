# Glossary of Networking Abbreviations

This glossary explains abbreviations used across the repository.

## Core Networking

| Abbreviation | Full Form | Meaning |
| --- | --- | --- |
| IP | Internet Protocol | Protocol used for logical addressing and routing packets between networks |
| IPv4 | Internet Protocol version 4 | 32-bit IP address format such as `192.168.1.10` |
| IPv6 | Internet Protocol version 6 | 128-bit IP address format such as `2001:db8::10` |
| MAC | Media Access Control | Hardware-style address used for local network delivery |
| LAN | Local Area Network | Network in a small area such as a home or office |
| WLAN | Wireless Local Area Network | Wireless LAN, commonly WiFi |
| MAN | Metropolitan Area Network | Network spanning a city or campus |
| WAN | Wide Area Network | Network spanning large geographic areas |
| VPN | Virtual Private Network | Encrypted logical network over another network |
| ISP | Internet Service Provider | Company that provides internet connectivity |
| VLAN | Virtual Local Area Network | Logical separation of a Layer 2 network |
| NAT | Network Address Translation | Translates private IP addresses to another address, often a public IP |
| CIDR | Classless Inter-Domain Routing | Slash notation for network size, such as `/24` |
| ICMP | Internet Control Message Protocol | Protocol used for network control messages, including many `ping` responses |

## Models and Layers

| Abbreviation | Full Form | Meaning |
| --- | --- | --- |
| OSI | Open Systems Interconnection | Seven-layer learning model for networking |
| TCP/IP | Transmission Control Protocol / Internet Protocol | Practical internet protocol stack |
| L1-L7 | Layer 1 to Layer 7 | Short names for OSI model layers |

## Transport and Connection Terms

| Abbreviation | Full Form | Meaning |
| --- | --- | --- |
| TCP | Transmission Control Protocol | Reliable, connection-oriented transport protocol |
| UDP | User Datagram Protocol | Lightweight, connectionless transport protocol |
| SYN | Synchronize | TCP flag used to start a connection |
| ACK | Acknowledgement | TCP flag used to confirm received data or connection steps |
| FIN | Finish | TCP flag used to gracefully close a connection |
| RST | Reset | TCP flag used to abruptly reset a connection |
| TLS | Transport Layer Security | Encryption protocol used by HTTPS and many secure services |

## Application Protocols

| Abbreviation | Full Form | Meaning |
| --- | --- | --- |
| HTTP | Hypertext Transfer Protocol | Protocol for web traffic |
| HTTPS | Hypertext Transfer Protocol Secure | HTTP protected with TLS encryption |
| DNS | Domain Name System | Translates names such as `example.com` into IP addresses |
| DHCP | Dynamic Host Configuration Protocol | Automatically assigns IP settings to devices |
| DORA | Discover, Offer, Request, Acknowledge | Four-step DHCP process used to lease an IP address |
| SSH | Secure Shell | Secure remote login protocol |
| FTP | File Transfer Protocol | Protocol for transferring files |
| SMTP | Simple Mail Transfer Protocol | Protocol used to send email |
| IMAP | Internet Message Access Protocol | Protocol used to read email from a mail server |
| IMAPS | Internet Message Access Protocol Secure | IMAP protected with TLS encryption |
| POP3 | Post Office Protocol version 3 | Protocol used to download email |
| NTP | Network Time Protocol | Protocol for time synchronization |
| RPC | Remote Procedure Call | Pattern where one system calls a function on another system |
| API | Application Programming Interface | Interface used by software systems to communicate |

## DNS Terms

| Abbreviation | Full Form | Meaning |
| --- | --- | --- |
| TTL | Time To Live | How long a DNS answer or packet-related value may be cached or kept |
| TLD | Top-Level Domain | Last part of a domain name, such as `.com` or `.org` |
| A | Address record | DNS record that maps a name to an IPv4 address |
| AAAA | IPv6 address record | DNS record that maps a name to an IPv6 address |
| CNAME | Canonical Name | DNS alias from one name to another name |
| MX | Mail Exchanger | DNS record that identifies mail servers for a domain |
| TXT | Text | DNS record for text metadata such as verification or email policy |
| NS | Name Server | DNS record that lists authoritative name servers |
| SOA | Start of Authority | DNS record containing zone authority and timing metadata |
| PTR | Pointer | DNS record used for reverse DNS lookups |
| SRV | Service | DNS record that identifies service location information |
| SPF | Sender Policy Framework | Email policy stored in DNS TXT records to help prevent spoofing |
| DKIM | DomainKeys Identified Mail | Email signing method that uses DNS TXT records for public keys |
| DMARC | Domain-based Message Authentication, Reporting, and Conformance | Email policy that builds on SPF and DKIM |

## Cloud Networking

| Abbreviation | Full Form | Meaning |
| --- | --- | --- |
| VPC | Virtual Private Cloud | Logically isolated cloud network |
| EC2 | Elastic Compute Cloud | AWS virtual machine service |
| AWS | Amazon Web Services | Cloud provider used in many examples |
| IGW | Internet Gateway | VPC component that enables internet access for public subnets |
| ALB | Application Load Balancer | AWS load balancer for HTTP and HTTPS traffic |
| LB | Load Balancer | Service that distributes traffic across backend targets |
| ACL | Access Control List | Rule list that allows or denies traffic |
| NACL | Network Access Control List | Subnet-level stateless firewall in AWS |
| AZ | Availability Zone | Isolated location inside a cloud region |
| DB | Database | System used to store and query data |

## Security and Administration

| Abbreviation | Full Form | Meaning |
| --- | --- | --- |
| RDP | Remote Desktop Protocol | Microsoft remote desktop protocol |
| JSON | JavaScript Object Notation | Common structured data format used by APIs and configuration files |
