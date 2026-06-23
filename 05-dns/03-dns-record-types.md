# DNS Record Types

DNS records define how names map to addresses and services.

## Common DNS Records

| Record | Purpose | Example |
| --- | --- | --- |
| A | Maps a name to an IPv4 address | `example.com -> 203.0.113.10` |
| AAAA | Maps a name to an IPv6 address | `example.com -> 2001:db8::10` |
| CNAME | Alias from one name to another | `www.example.com -> example.com` |
| MX | Mail server for a domain | `example.com -> mail.example.com` |
| TXT | Text metadata | SPF, DKIM, verification records |
| NS | Authoritative name servers | `ns1.provider.com` |
| SOA | Start of authority metadata | Zone ownership and timing |
| PTR | Reverse DNS lookup | IP address to hostname |
| SRV | Service location | Used by some service discovery systems |

## A Record

An A record maps a domain name to an IPv4 address.

```text
api.example.com -> 203.0.113.25
```

Use A records when you want a name to point directly to an IPv4 address.

## CNAME Record

A CNAME record creates an alias.

```text
www.example.com -> example.com
```

CNAME records are useful when one name should follow another name's DNS answer.

## MX Record

MX records tell other mail servers where to deliver email for a domain.

```text
example.com -> mail.example.com
```

MX records have priorities. Lower numbers are preferred first.

## TXT Record

TXT records store text information. They are commonly used for:

- Domain ownership verification
- SPF email policy
- DKIM email signing
- DMARC email policy

## Common Beginner Mistakes

- Creating a CNAME at the root domain when the DNS provider does not support it.
- Forgetting that CNAME points to another name, not directly to an IP address.
- Changing DNS records without checking TTL.
- Confusing MX records for receiving email with SMTP settings for sending email.
