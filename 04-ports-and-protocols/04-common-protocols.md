# Common Protocols

A protocol is a set of rules that systems follow to communicate.

Different protocols solve different problems: websites, name resolution, remote login, email, time synchronization, and file transfer all use different communication rules.

## Common Protocol Table

| Protocol | Port | Transport | Purpose |
| --- | ---: | --- | --- |
| HTTP | `80` | TCP | Unencrypted web traffic |
| HTTPS | `443` | TCP | Encrypted web traffic |
| DNS | `53` | UDP/TCP | Name resolution |
| SSH | `22` | TCP | Secure remote login |
| SMTP | `25` | TCP | Send email between mail servers |
| IMAP | `143` | TCP | Read email |
| IMAPS | `993` | TCP | Secure IMAP |
| POP3 | `110` | TCP | Download email |
| NTP | `123` | UDP | Time synchronization |
| DHCP | `67/68` | UDP | Automatic IP configuration |
| FTP | `20/21` | TCP | File transfer |
| MySQL | `3306` | TCP | MySQL database |
| PostgreSQL | `5432` | TCP | PostgreSQL database |

## Protocol Stack Example

```mermaid
flowchart TB
    HTTPS["HTTPS"]
    TLS["TLS Encryption"]
    TCP["TCP Port 443"]
    IP["IP Routing"]
    Ethernet["Ethernet or WiFi"]

    HTTPS --> TLS --> TCP --> IP --> Ethernet
```

When you visit an HTTPS website, multiple protocols work together. HTTPS uses TLS for encryption, TLS uses TCP for reliable delivery, TCP uses IP for routing, and IP uses Ethernet or WiFi for local delivery.

## Important Distinction

Ports and protocols are related but not the same.

- A protocol defines communication rules.
- A port identifies where a service listens.

For example, HTTPS usually uses TCP port `443`, but port `443` alone does not magically make traffic secure. The application must actually use TLS/HTTPS correctly.

## Common Beginner Mistakes

- Memorizing port numbers without understanding what the protocol does.
- Assuming every protocol uses only one transport. DNS commonly uses UDP, but it can also use TCP.
- Thinking HTTPS is only HTTP on a different port. HTTPS adds encryption with TLS.
