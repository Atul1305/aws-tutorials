 VPC is
    - Create user defined virtual networks(IPv4/v6)
    - Can be connected to existing datacenters over VPN or Direct Connect
    - Can be peered with other VPCs in AWS

// TODO: VPC Architecture Image to come

Subnet
    - Multiple subnets can be created inside a VPC.
    - Router helps to connect all subnets.
    - Virtual private gateway helps to make a bridge between your datacenter or PC.

**VPC Components**

* Route Table/ Router
    Route table holds info where something should be send like 10.0.0.1 -> 10.0.0.15
    Router Uses route table to move from one system to another system.
    If there is no route exist between two system that request will be timeout.

* Elastic Ip
    is basically a static public IP
    





