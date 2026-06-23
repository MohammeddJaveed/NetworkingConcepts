# Ports Cheatsheet

## Common Ports

| Port | Protocol | Service |
| ---: | --- | --- |
| `20/21` | TCP | FTP, File Transfer Protocol |
| `22` | TCP | SSH, Secure Shell |
| `25` | TCP | SMTP, Simple Mail Transfer Protocol |
| `53` | UDP/TCP | DNS, Domain Name System |
| `67/68` | UDP | DHCP, Dynamic Host Configuration Protocol |
| `80` | TCP | HTTP, Hypertext Transfer Protocol |
| `110` | TCP | POP3, Post Office Protocol version 3 |
| `123` | UDP | NTP, Network Time Protocol |
| `143` | TCP | IMAP, Internet Message Access Protocol |
| `443` | TCP | HTTPS, HTTP Secure |
| `993` | TCP | IMAPS, IMAP over TLS |
| `3306` | TCP | MySQL |
| `5432` | TCP | PostgreSQL |
| `6379` | TCP | Redis |
| `27017` | TCP | MongoDB |

## Security Notes

- Do not expose SSH or RDP to the whole internet.
- Databases should usually listen only on private networks.
- Public web services should use HTTPS.
- Opening a port in a firewall is not enough; the application must also be listening.
