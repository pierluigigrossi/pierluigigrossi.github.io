---
layout: page
permalink: /ip/
title: IP
description: Some of the stuff I did
nav: true
nav_order: 2
---

#### Service Provider Networks

**Core and Metro IP**

Seamless MPLS IPv4 network design:
Access Node(DSLAM/OLT/CE/BTS)->Metro Network-> Core Network-> Peering/Transit.
* IGP Protocols: IS-IS and OSPFv3 to redistribute loopbacks.
* MP-BGP with redundant and virtualized Route Reflectors 
* ECMP for loadbalacing 
* MPLS labels distributed via BGP LU.
* Loadbalacing via MPLS Entropy Label and Deep Packet Inspection on the EdgeLSR 
* PCEP controller
* BGP Link State to signal network topology to the controller

BGP/MPLS services:
* MPLS L3VPN, VPWS, VPLS, 6PE(to deliver IPv6 to customers and PE), 6VPE
* BGP FlowSpec


VPLS was implemented using EVPN , using BGP both for autodiscovery and signaling. 

* Routers used:Cisco ASR 9k and NCS 55xx, Juniper PTX and MX , Huawei NE40E, Nokia SR 7700

* Cisco Network Service Orchestrator

**IP Edge**

Python scripts to automate service delivery:
* CE-PE Business customers with BGP Session
* Residential and small business BNG: terminating Pseudowires. AAA of CPEs conncted with DHCP or PPPoE, CGNAT 
* IP management


**NGAN  Fixed Access**
* ULL/VULA/NGA Access Troubleshooting and design
* OLT and DSLAM Nokia and Huawei 


#### Datacenter Networks

* Switches:Cisco Nexus 7000, 9000, QFX 5100 series
* Virtual Switches:  Vmware Distributed Switch

I swapped deployments from plain Ethernet, Spanning Tree and VLAN to VxLAN and Routing, building the so called "IP Switched Fabric".This technology enables stretching VLANs across geographically different places and saves links capacity, using the ECMP routing techinque.
All DC services relay on the same IP fabric, iSCSI too.

#### Enterprise Networks
LAN mainly with Cisco Switch 3850/9300 stacks, both for Data and IP Voice with QoS.
Firewall: Cisco ASA, Juniper SRX, Fortinet, Checkpoint and PaloAlto (Policies, IPsec VPN, SSL VPN, etc..)


