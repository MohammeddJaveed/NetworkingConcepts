# Scenario-Based Networking Questions

Scenario questions test whether you can reason through real problems, not just define terms.

## Scenario 1: Website Is Not Loading

Question: A user says `app.example.com` is not loading. What do you check?

Answer:

1. Check DNS resolution for `app.example.com`.
2. Check whether the resolved IP is correct.
3. Check routing and reachability.
4. Check whether the expected port, usually `443`, is open.
5. Check TLS certificate validity.
6. Check load balancer health checks.
7. Check application logs.

## Scenario 2: EC2 Instance in Public Subnet Is Not Reachable

Question: An EC2 instance has a public IP but SSH does not work. What could be wrong?

Answer:

- Security group does not allow TCP port `22`.
- Network ACL blocks inbound or outbound traffic.
- Route table does not point `0.0.0.0/0` to an internet gateway.
- Internet gateway is not attached to the VPC.
- Operating system firewall blocks SSH.
- SSH service is not running.
- Wrong key pair or username is being used.

## Scenario 3: Private Instance Cannot Download Updates

Question: A private subnet instance cannot reach the internet. What do you check?

Answer:

- Private route table has `0.0.0.0/0` pointing to a NAT gateway.
- NAT gateway is in a public subnet.
- Public subnet route table points `0.0.0.0/0` to an internet gateway.
- NAT gateway has a public IP.
- Security group and network ACL allow outbound traffic and return traffic.
- DNS resolution works.

## Scenario 4: Database Should Not Be Public

Question: How do you design database access securely in a VPC?

Answer:

- Place the database in private subnets.
- Do not assign a public IP.
- Allow inbound database port only from application server security groups.
- Use private DNS or internal service discovery.
- Restrict administrative access through VPN, Session Manager, or bastion access.

## Scenario 5: DNS Record Was Updated but Users Still See Old IP

Question: Why might users still reach the old server?

Answer:

- DNS records are cached.
- TTL has not expired.
- Different resolvers may update at different times.
- Browser or operating system cache may still hold old data.
- The wrong authoritative zone may have been updated.
