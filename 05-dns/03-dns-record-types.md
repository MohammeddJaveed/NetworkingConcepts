# DNS Record Types

DNS records define how names map to addresses and services.

## Common DNS Records

| Record | Purpose | Example |
| --- | --- | --- |
| A | Address record; maps a name to an IPv4 address | `example.com -> 203.0.113.10` |
| AAAA | IPv6 address record; maps a name to an IPv6 address | `example.com -> 2001:db8::10` |
| CNAME | Canonical Name; alias from one name to another | `www.example.com -> example.com` |
| MX | Mail Exchanger; mail server for a domain | `example.com -> mail.example.com` |
| TXT | Text record; stores text metadata | SPF, DKIM, verification records |
| NS | Name Server; authoritative name servers | `ns1.provider.com` |
| SOA | Start of Authority; zone ownership and timing metadata | Zone authority details |
| PTR | Pointer record; reverse DNS lookup | IP address to hostname |
| SRV | Service record; service location | Used by some service discovery systems |

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
- SPF, or Sender Policy Framework, email policy
- DKIM, or DomainKeys Identified Mail, email signing
- DMARC, or Domain-based Message Authentication, Reporting, and Conformance, email policy

## Common Beginner Mistakes

- Creating a CNAME at the root domain when the DNS provider does not support it.
- Forgetting that CNAME points to another name, not directly to an IP address.
- Changing DNS records without checking TTL.
- Confusing MX records for receiving email with SMTP settings for sending email.
