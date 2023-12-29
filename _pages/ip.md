---
layout: page
permalink: /ip/
title: IP
description: Protocols and equipments test
nav: true
nav_order: 6
---

**Service Provider Networks:**
I implemnted and tested a Seamless MPLS IPv4 network design:
Access Node(DSLAM/OLT/CE/BTS)->Metro Network-> Core Network-> Peering/Transit.
* Router used:Cisco ASR 9k, Juniper PTX and MX , Huawei NE40E, Nokia SR 7700
* IS-IS and OSPFv3 to redistribute loopbacks.
* On the top of that MP-BGP with redundant and virtualized Route Reflectors was implemented.
* MPLS labels distributed with BGP LU.

Service succefully deployed and tested:
* MPLS L3VPN, VPWS, VPLS, 6PE, Multicast VPN (to deliver IPv6 to customers and PE), 6VPE

VPLS was implemented using RFC4761, using BGP both for autodiscovery and signaling

**Datacenter Networks:**

* Switches:Cisco Nexus 7000, 9000, QFX 5100 series
* Virtual Switches:  Vmware Distributed Switch

I swapped deployments from plain Ethernet, Spanning Tree and VLAN to VxLAN and Routing, building the so called "IP Swtiched Fabric", this technology enables streaching of VLANs across geographically different places and not to speare link capacity using the ECMP routing techinque.
On the same IP fabric it's running the iSCSI storage

**Enterprise Networks:**
LAN mainly with Cisco Switch 3850/9300 stacks, both for Data and IP Voice with QoS.
Firewall: Cisco ASA, Juniper SRX, Fortinet, Checkpoint and PaloAlto (managed Policies, IPsec VPN, SSL VPN, etc..)


