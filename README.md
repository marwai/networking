Subnet is a subnet inside a network that makes traffic in the IP directs exactly where it needs to go

Submasks - hides the IP addresss, allows different traffic to be picked up

# Submask/Cidr block
 Submask works at the end of the IP address
	- Represents the submask as a block at the end of the an IP
	- It represents by the submask by adding the bits
IPV4 you can have a maximum of 32 bit, when adding the 8 bits inside the 4 octets

# N-Tier Architecture
	- Monliths

## Monoliths
	- Big, solid single point of failure because it is one big block
	- Monolith architecture - describes an application that has everything working on the same server.
	- Everything running on machine/server:
		○ DB/Logic/Presentation

### Example
	- Database on top
	- NodeJS running on server


# Networking

192.65.63.1

VPC with public and private subnet (NAT)

The configuration of this scenario includes a virtual private cloud (VPC) with a public subnet and a private subnet.

• A VPC with a size /16 IPv4 CIDR block (example: 10.0.0.0/16). This provides 65,536 private IPv4 addresses.
• A public subnet with a size /24 IPv4 CIDR block (example: 10.0.0.0/24). This provides 256 private IPv4 addresses. A public subnet is a subnet that's associated with a route table that has a route to an Internet gateway.
• A private subnet with a size /24 IPv4 CIDR block (example: 10.0.1.0/24). This provides 256 private IPv4 addresses.

Implementing Scenario 2
You can use the VPC wizard to create the VPC, subnets, NAT gateway and optionally, an egress-only internet gateway.

Implementing Scenario 2 with a NAT instance

2-Tier Infrastructure
A two-tier architecture is a software architecture in which a presentation layer or interface runs on a client, and a data layer or data structure gets stored on a server. Separating these two components into different locations represents a two-tier architecture, as opposed to a single-tier architecture. Other kinds of multi-tier architectures add additional layers in distributed software design


test

3-Tier Infrastructure
	1. Public Layer
	2. Application Layer
Database Layer

Cloud service (AWS) there is Virtual Private Cloud (database servers and web servers)
 DB:
-  2 tier architecture

 Within VPC we can allow for multiple IP addresses to connect, multiple users have 16IPv4 cidr block

