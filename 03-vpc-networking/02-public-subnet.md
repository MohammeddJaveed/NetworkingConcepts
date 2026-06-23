# Public Subnet

A subnet that has access to the internet.

Requirements:

- Route to Internet Gateway
- Public IP attached

Example:

Subnet:
10.0.1.0/24

Route Table:

0.0.0.0/0 → Internet Gateway

Resources:

- Web Servers
- Bastion Hosts
