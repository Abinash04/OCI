# OCI
Oracle Cloud Infrastructure Notes

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

In IP addressing, when you have a subnet with 24 bits, it means that you have 24 bits for the network portion of the address, leaving 32 - 24 = 8 bits for the host portion.

With 8 bits for hosts, you can have 2^8 - 2 = 256 - 2 = 254 hosts. The "-2" accounts for the network address and the broadcast address, which cannot be assigned to individual hosts.

So, with 24 bits subnet mask, you can have up to 254 hosts on the subnet.
```
