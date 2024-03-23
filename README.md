# OCI
Oracle Cloud Infrastructure Notes

```
Tenancy:

A tenancy is the highest level of administrative unit in OCI.
When you sign up for an OCI account, you are assigned a tenancy, which represents your entire cloud account.
A tenancy has its own separate identity, resources, policies, and administrative boundaries.
All resources within a tenancy belong to and are managed by the tenant organization or entity.
A tenancy encapsulates all the compartments and resources created within it.

Compartment:

A compartment is a logical container within a tenancy used to organize and isolate cloud resources.
Compartments help you organize resources based on business units, projects, environments, or any other organizational structure.
Each compartment can have its own set of policies, access controls, and resource management settings.
Compartments provide isolation and access control boundaries, allowing you to delegate administrative responsibilities and enforce security policies at a granular level.
Resources within a compartment inherit policies and permissions defined at the compartment level.
In summary, a tenancy represents your entire OCI account and serves as the top-level administrative boundary, while compartments are used to organize resources within the tenancy into logical groups for better management, isolation, and access control. Think of a tenancy as the overarching organization and compartments as the subdivisions within that organization for organizing resources.
```

# CIDR Notation
CIDR presentation: A.B.C.D/x

## Components of CIDR prefix:
```
Network Address - A.B.C.D
Network prefix or mask - /x

Subnetting allows dividing CIDR prefixes into smaller ones
CIDR notation: 192.168.1.0/24

8bits.8bits.8bits.8bits - 32 bits
192.168.1 - First 24bits - Network address
0 - Last bit host address

Network ID: 192.168.1.0
First Host: 192.168.1.1
Last Host: 192.168.1.254
Broadcast Address: 192.168.1.255

In IP addressing, when you have a subnet with 24 bits, it means that you have 24 bits for the network portion of the address,
leaving 32 - 24 = 8 bits for the host portion. 
With 8 bits for hosts, you can have 2^8 - 2 = 256 - 2 = 254 hosts. The "-2" accounts for the network address and the broadcast address, which cannot be assigned to individual hosts.
So, with 24 bits subnet mask, you can have up to 254 hosts on the subnet.
```
