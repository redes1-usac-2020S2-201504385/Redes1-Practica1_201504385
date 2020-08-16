# Docs

### Topology

<img src="./img/topology.PNG" alt="Topology" style="zoom: 100%;" />

### Description

#### Router

| Interface | Network Address | IP Address     |
| --------- | --------------- | -------------- |
| f0/0      | 192.168.1X.0/24 | 192.168.1X.254 |
| f0/1      | 192.168.1Y.0/24 | 192.168.1Y.254 |

**where x = 8 and y = 5*



#### Hosts

| Type      | Name   | Connected To | IP Address    |
| --------- | ------ | ------------ | ------------- |
| TinyLinux | tiny-1 | Switch1      | 192.168.1X.30 |
| VPCS      | PC2    | Switch1      | 192.168.1X.15 |
| VPCS      | PC3    | Switch2      | 192.168.1Y.15 |
| VPCS      | PC4    | Switch2      | 192.168.1Y.30 |

**where x = 8 and y = 5*



