# Cloud VPC Diagram

This diagram shows a common cloud VPC layout with public and private subnets.

```mermaid
flowchart TB
    Internet["Internet"] --> IGW["Internet Gateway"]

    subgraph VPC["VPC 10.0.0.0/16"]
        subgraph PublicA["Public Subnet A 10.0.1.0/24"]
            ALB["Public Load Balancer"]
            NATA["NAT Gateway"]
        end

        subgraph PrivateA["Private App Subnet A 10.0.2.0/24"]
            AppA["Application Server"]
        end

        subgraph DBA["Private DB Subnet A 10.0.3.0/24"]
            DB["Database"]
        end
    end

    IGW --> ALB
    AppA --> NATA
    NATA --> IGW
    ALB --> AppA
    AppA --> DB
```

The load balancer is public. Application servers and databases remain private. Private servers use the NAT gateway for outbound internet access.
