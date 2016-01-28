#AWS Customer Responsibility Requirement:

Customers are responsible for all aspects of this control related to user account access to their compute instances, virtual networks, and block stores. Details of each aspect of EC2, VPC, and EBS are outlined below.

## EC2
Virtual EC2 instances are completely controlled by the customer agency. Customers have full root access or administrative control over accounts, services, and applications. AWS does not have any access rights to customer instances and cannot log into the guest

## OS
AWS recommends a base set of security best practices to include disabling password-only access to their servers, and utilizing some form of multi-factor authentication to gain access to their instances (or at a minimum certificate-based SSH Version 2 access).
Additionally, customers should employ a privilege escalation mechanism with logging on a per-user basis. For example, if the guest OS is Linux, after hardening their instance, they should utilize certificate-based SSHv2 to access the virtual instance, disable remote root login, use command-line logging, and use ‘sudo’ for privilege escalation.
Customers should generate their own key pairs in order to guarantee that they are unique, and not shared with other customers or with AWS.

## EBS
Once a customer creates an Amazon EBS volume, the customer can attach it to an Amazon EC2 instance. Once attached, it will appear as a mounted device similar to any hard drive or other block device. At that point, the instance can interact with the volume just as it would with a local drive, formatting it with a file system or installing applications on it directly. The customer controls which EC2 instance an EBS volume may be attached to.

## VPC
Through the AWS Management Console, Amazon Virtual Private Cloud (Amazon VPC) lets customers provision a private, isolated section of the Amazon Web Services (AWS) Cloud where customers can launch AWS resources in the customer-defined virtual network. Customers can leverage multiple layers of security, including security groups and network access control lists, to help control access to Amazon EC2 instances in each subnet.
