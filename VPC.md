 * VPC is
    - Create user defined virtual networks(IPv4/v6)
    - Can be connected to existing datacenters over VPN or Direct Connect
    - Can be peered with other VPCs in AWS
<br>

// TODO: VPC Architecture Image to come
<br>

* Subnets
    - Multiple subnets can be created inside a VPC.
    - Virtual private gateway helps to make a bridge between your datacenter or PC.
    - 
<br>

* Ip Addresses
    - IPv4 : Each IP address is made of four octets of 8 bits each.
    - IPv6 : 128 bits.
    - Within a VPC, certain IP Addresses are reserved so can;t be usable.
<br>

* IP CIDR Range :
    - Its a number that represent range of IP's in a network.
    - eg. 10.0.0.0/16 -> It represent first 16 bits are fixed.
    - So, the Ip ranges for above CIDR range -> 10.0.0.0 -> 10.0.255.255
    - CIDR ranges are immutable. If you want to change IP range add a new CIDR.
    - CIDR range of VPC is limited by AWS which is in range of /16 - /28
<br>

**VPC Components**

* Route Table/Router
    - Route table holds info where something should be send like 10.0.0.1 -> 10.0.0.15
    - Router Uses route table to move from one system to another system.
    - Router helps to connect all subnets.
    - If there is no route exist between two system that request will be timeout.
<br>

* Elastic Ip
    - is basically a static public IP.
    - When an EC2 instance is created, a dynamic ip is attached to it. If we want a permanent IP for EC2 instance we attach elastic IP to it. 

<br>

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

<br>

* Internet Gateway
    - A gateway that allows instance to connect to the internet.

<br>

* Customer Gateway/VPN Connection/Virtual Private Gateway
    - To establish a VPN connection all three mwntioned components need to be work together.
    - Customer Gateway is router in organization premises.
    - On AWS side private virtual gateway is used to establish connection.
    - So, to connect a VPN connection there will be two endpoints one is Customer gateway and another is virtual private gateway.
    - 

<br>

* VPC Peering
    - When we connect to VPC's togeather
<br>

* VPC Endpoints
    - Connectivity to talk to any AWS services privately.
    - Benefit is data don't travelled through internet.

<br>

* NAT gateway
    - Only allow outbound connection and reply on the same connection.

    
**References**
===============
* [AWS Networking Masterclass - VPC](https://www.youtube.com/watch?v=LX5lHYGFcnA)
* [Keep Your Network Traffic in AWS with VPC Endpoints | Overview and Tutorial](https://www.youtube.com/watch?v=jo3X_aay4Vs)




