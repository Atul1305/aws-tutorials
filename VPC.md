 VPC is
    - Create user defined virtual networks(IPv4/v6)
    - Can be connected to existing datacenters over VPN or Direct Connect
    - Can be peered with other VPCs in AWS

// TODO: VPC Architecture Image to come

Subnet
    - Multiple subnets can be created inside a VPC.
    - Virtual private gateway helps to make a bridge between your datacenter or PC.

**VPC Components**

* Route Table/Router
    - Route table holds info where something should be send like 10.0.0.1 -> 10.0.0.15
    - Router Uses route table to move from one system to another system.
    - Router helps to connect all subnets.
    - If there is no route exist between two system that request will be timeout.

* Elastic Ip
    - is basically a static public IP.
    - When an EC2 instance is created, a dynamic ip is attached to it. If we want a permanent IP for EC2 instance we attach elastic IP to it. 


* Elastic Network Interface
    An elastic network interface is a logical networking component in a VPC that represents a virtual network card. It can include the following attributes:

    - A primary private IPv4 address from the IPv4 address range of your VPC
    - One or more secondary private IPv4 addresses from the IPv4 address range of your VPC
    - One Elastic IP address (IPv4) per private IPv4 address
    - One public IPv4 address
    - One or more IPv6 addresses
    - One or more security groups
    - A MAC address
    - A source/destination check flag
    - A description

* Internet Gateway
    - A gateway that allows instance to connect to the internet.

* Customer Gateway/VPN Connection/Virtual Private Gateway
    - 

    





