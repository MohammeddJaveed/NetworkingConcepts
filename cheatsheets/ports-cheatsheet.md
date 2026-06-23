# Ports Cheatsheet

## Common Ports

| Port | Protocol | Service |
| ---: | --- | --- |
| `20/21` | TCP | FTP |
| `22` | TCP | SSH |
| `25` | TCP | SMTP |
| `53` | UDP/TCP | DNS |
| `67/68` | UDP | DHCP |
| `80` | TCP | HTTP |
| `110` | TCP | POP3 |
| `123` | UDP | NTP |
| `143` | TCP | IMAP |
| `443` | TCP | HTTPS |
| `993` | TCP | IMAPS |
| `3306` | TCP | MySQL |
| `5432` | TCP | PostgreSQL |
| `6379` | TCP | Redis |
| `27017` | TCP | MongoDB |

## Security Notes

- Do not expose SSH or RDP to the whole internet.
- Databases should usually listen only on private networks.
- Public web services should use HTTPS.
- Opening a port in a firewall is not enough; the application must also be listening.
