---
# Infrastructure or Platform (PaaS), or Software (SaaS), as a Service (XaaS)
controls:
  - control: 'AWS (IAM) Account Management'
    boundary: IaaS
    poc: @AWS
    todo: 0
    doing: 0
    done: 100
  - control: 'AWS (EC2) Account Management'
    boundary: IaaS
    poc: @AWS
    todo: 0
    doing: 0
    done: 100
  - control: 'AWS (IAM) Account Management'
    boundary: IaaS
    poc: @AWS
    todo: 0
    doing: 0
    done: 100
  - control: 'AWS (S3) (Cloud Front) (EBS) Account Management'
    boundary: IaaS
    todo: 20
    doing: 30
    done: 50  
  - control: 'AWS (VPC) (Route 53) (ELB) Account Management'
    boundary: IaaS
    todo: 20
    doing: 30
    done: 50
  - control: 'Cloud Foundry (UAAC) PaaS Account Management'
    boundary: PaaS
    poc: @18F
    todo: 0
    doing: 10
    done: 90
  - control: 'Applications and Websites'
    boundary: SaaS
    poc: @datagov
    todo: 10
    doing: 0
    done: 90      
---

## AWS (IAM) Account Management:
[Inherit from](@AWS)
[Inherit from](@18F)

## AWS (EC2) Account Management:
[Inherit from](@AWS)
[Inherit from](@18F)

## AWS (S3) (Cloud Front) (EBS) Account Management:
[Inherit from](@AWS)
[Inherit from](@18F)

## AWS (RDS) Account Management:
[Inherit from](@AWS)
[Inherit from](@18F)

## AWS (VPC) (Route 53) (ELB) Account Management:
[Inherit from](@AWS)
[Inherit from](@18F)

## Cloud Foundry (UAAC) PaaS Account Management:
[Inherit from](@18F)

## Applications and Websites:
[Appended from](@18F)

```
The Application system owner (SO) should ensure its applications
provide a way to manage user’s access using identifiers
(i.e. individual, group, system, application, guest/anonymous, and temporary)
if required and not handled by the 18F DevOps team.
```
[Appended by](@datagov)
