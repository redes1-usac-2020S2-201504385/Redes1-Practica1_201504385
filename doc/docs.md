# Docs

You are asked to configure and manage the devices of a network infrastructure for a company which is starting to grow and want to implement a network, a network architect provides them with the **[design of the topology](#Topology)** that will be used by said company, but they must configure it to provide communication according to the needs indicated.

You must configure and manage the equipment of a network infrastructure for a company which has **[4 hosts](#Hosts)** which are connected to 2 different switches and these are connected to each other through a **[router](#Router)** which will be the main communication center.



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



