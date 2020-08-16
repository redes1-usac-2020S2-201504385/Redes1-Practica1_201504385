# Docs

You are asked to configure and manage the devices of a network infrastructure for a company which is starting to grow and want to implement a network, a network architect provides them with the **[design of the topology](#Topology)** that will be used by said company, but they must configure it to provide communication according to the needs indicated.

You must configure and manage the equipment of a network infrastructure for a company which has **[4 hosts](#Hosts)** which are connected to 2 different switches and these are connected to each other through a **[router](#Router)** which will be the main communication center.

- [Topology](#Topology)
- [Description](#Description)
- [Vocabulary](#Vocabulary)



## Topology

<img src="./img/topology.PNG" alt="Topology" style="zoom: 100%;" />

## Description

### Router

| Interface | Network Address | IP Address     |
| --------- | --------------- | -------------- |
| f0/0      | 192.168.1X.0/24 | 192.168.1X.254 |
| f0/1      | 192.168.1Y.0/24 | 192.168.1Y.254 |

**where x = 8 and y = 5*



### Hosts

| Type      | Name   | Connected To | IP Address    |
| --------- | ------ | ------------ | ------------- |
| TinyLinux | tiny-1 | Switch1      | 192.168.1X.30 |
| VPCS      | PC2    | Switch1      | 192.168.1X.15 |
| VPCS      | PC3    | Switch2      | 192.168.1Y.15 |
| VPCS      | PC4    | Switch2      | 192.168.1Y.30 |

**where x = 8 and y = 5*





## Vocabulary

#### **Router**

A **router**[[a\]](https://en.wikipedia.org/wiki/Router_(computing)#cite_note-2) is a [networking device](https://en.wikipedia.org/wiki/Networking_device) that forwards [data packets](https://en.wikipedia.org/wiki/Data_packet) between [computer networks](https://en.wikipedia.org/wiki/Computer_network). Routers perform the traffic directing functions on the [Internet](https://en.wikipedia.org/wiki/Internet). Data sent through the internet, such as a [web page](https://en.wikipedia.org/wiki/Web_page) or [email](https://en.wikipedia.org/wiki/Email), is in the form of data packets. A packet is typically [forwarded](https://en.wikipedia.org/wiki/Packet_forwarding) from one router to another router through the networks that constitute an [internetwork](https://en.wikipedia.org/wiki/Internetwork) (e.g. the Internet) until it reaches its destination [node](https://en.wikipedia.org/wiki/Node_(networking)).[[2\]](https://en.wikipedia.org/wiki/Router_(computing)#cite_note-3)

A router is connected to two or more data lines from different [IP networks](https://en.wikipedia.org/wiki/IP_network).[[b\]](https://en.wikipedia.org/wiki/Router_(computing)#cite_note-4) When a data packet comes in on one of the lines, the router reads the [network address](https://en.wikipedia.org/wiki/Network_address) information in the packet header to determine the ultimate destination. Then, using information in its [routing table](https://en.wikipedia.org/wiki/Routing_table) or [routing policy](https://en.wikipedia.org/wiki/Routing_policy), it directs the packet to the next network on its journey.

The most familiar type of IP routers are [home and small office routers](https://en.wikipedia.org/wiki/Residential_gateway) that simply forward [IP packets](https://en.wikipedia.org/wiki/IP_packet_(disambiguation)) between the home computers and the Internet. More sophisticated routers, such as enterprise routers, connect large business or ISP networks up to the powerful [core routers](https://en.wikipedia.org/wiki/Core_router) that forward data at high speed along the [optical fiber](https://en.wikipedia.org/wiki/Optical_fiber) lines of the [Internet backbone](https://en.wikipedia.org/wiki/Internet_backbone). 

*[Wikipedia](https://en.wikipedia.org/wiki/Router_(computing))*

#### Host

A **network host** is a [computer](https://en.wikipedia.org/wiki/Computer) or other device connected to a [computer network](https://en.wikipedia.org/wiki/Computer_network). A host may work as a [server](https://en.wikipedia.org/wiki/Server_(computing)) offering information resources, services, and applications to users or other hosts on the network. Hosts are assigned at least one [network address](https://en.wikipedia.org/wiki/Network_address).

A computer participating in networks that use the [Internet protocol suite](https://en.wikipedia.org/wiki/Internet_protocol_suite) may also be called an **IP host**. Specifically, computers participating in the [Internet](https://en.wikipedia.org/wiki/Internet) are called **Internet hosts**. Internet hosts and other IP hosts have one or more [IP addresses](https://en.wikipedia.org/wiki/IP_address) assigned to their network interfaces. The addresses are configured either manually by an administrator, automatically at startup by means of the [Dynamic Host Configuration Protocol](https://en.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol) (DHCP), or by [stateless address autoconfiguration](https://en.wikipedia.org/wiki/Stateless_address_autoconfiguration) methods.

Network hosts that participate in applications that use the [client–server model](https://en.wikipedia.org/wiki/Client–server_model) of computing, are classified as [server](https://en.wikipedia.org/wiki/Server_(computing)) or [client](https://en.wikipedia.org/wiki/Client_(computing)) systems. Network hosts may also function as nodes in [peer-to-peer](https://en.wikipedia.org/wiki/Peer-to-peer) applications, in which all nodes share and consume resources in an equipotent manner.

[*Wikipedia*](https://en.wikipedia.org/wiki/Host_(network))