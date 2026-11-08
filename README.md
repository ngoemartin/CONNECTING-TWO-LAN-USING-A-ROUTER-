# CONNECTING-TWO-LAN-USING-A-ROUTER-
1. Objectives

The main objective of this project is to establish communication between two separate Local Area Networks (LANs) using a router in Cisco Packet Tracer.

The specific objectives are:

1. To design and configure two independent LANs.
2. To assign appropriate IP addresses to all computers and router interfaces.
3. To configure a router to enable communication between the two networks.
4. To connect computers to switches using copper straight-through cables.
5. To test connectivity between devices on different LANs using the ICMP ping command.
6. To understand how routers facilitate communication between different IP networks.

2. IP Address Configuration

The project consists of two separate networks, each using a different IP address range.

LAN CONNECTION 1 (Network 1)

Network Address: 10.1.1.0/24
Subnet Mask: 255.255.255.0

Device| IP Address| Subnet Mask| Default Gateway
Computer 1| 10.1.1.1| 255.255.255.0| 10.1.1.3
Computer 2| 10.1.1.2| 255.255.255.0| 10.1.1.3
Router Interface| 10.1.1.3| 255.255.255.0| N/A

LAN CONNECTION 2 (Network 2)

Network Address: 192.168.1.0/24
Subnet Mask: 255.255.255.0

Device| IP Address| Subnet Mask| Default Gateway
Computer 3| 192.168.1.1| 255.255.255.0| 192.168.1.3
Computer 4| 192.168.1.2| 255.255.255.0| 192.168.1.3
Router Interface| 192.168.1.3| 255.255.255.0| N/A

The router serves as the default gateway for both networks, allowing computers in one LAN to communicate with computers in the other LAN.

3. Tools Used

The following devices and software were used to implement the network topology:

1. Cisco Packet Tracer: Network simulation software used to design, configure, and test the network.
2. Cisco 1941 Router: Used to connect the two different LANs and facilitate communication between them.
3. Cisco 2960 Switches (2): Used to connect computers within each LAN.
4. PC-PT Computers (4): Used as end devices to send and receive data across the network.
5. Copper Straight-Through Cables: Used to establish physical connections between the computers and switches, as well as between the switches and router.
6. ICMP Ping Command: Used to test connectivity between computers on the two different networks.

4. Project Overview

This project involves the design and implementation of two separate Local Area Networks (LANs) connected through a Cisco 1941 router using Cisco Packet Tracer.

The first LAN consists of two computers (Computer 1 and Computer 2) connected to a Cisco 2960 switch. The second LAN also consists of two computers (Computer 3 and Computer 4) connected to another Cisco 2960 switch.

Both switches are connected to different interfaces of the Cisco 1941 router. Each LAN is assigned a unique network address. The first LAN uses the 10.1.1.0/24 network, while the second LAN uses the 192.168.1.0/24 network.

The router is configured with an IP address for each network interface, allowing it to forward packets between the two networks. Each computer is assigned an IP address, subnet mask, and default gateway corresponding to its respective LAN.

After configuring the network devices, connectivity was tested using ICMP packets in Simulation Mode. The simulation showed successful communication between devices across the two LANs, demonstrating that the router was correctly facilitating communication between the separate networks.

5. Network Topology

The network uses a star topology within each LAN, with a router connecting the two LANs.

The topology consists of:

- One Cisco 1941 router at the centre connecting the two networks.
- Two Cisco 2960 switches, with one switch assigned to each LAN.
- Four computers, with two computers connected to each switch.
- Copper straight-through cables connecting the network devices.

Network Structure:

LAN 1 (10.1.1.0/24)

- Computer 1: 10.1.1.1
- Computer 2: 10.1.1.2
- Switch 0
- Router Interface: 10.1.1.3

LAN 2 (192.168.1.0/24)

- Computer 3: 192.168.1.1
- Computer 4: 192.168.1.2
- Switch 1
- Router Interface: 192.168.1.3

The two switches are connected to the router, which acts as the intermediary device responsible for forwarding data packets between the two LANs.

This topology demonstrates how multiple independent local networks can be interconnected to form a larger network while maintaining separate IP address ranges.