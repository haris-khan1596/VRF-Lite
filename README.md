# VRF-Lite HLD
Table of content



<!-- /TOC -->

## Document History

| Version | Date       | Author       | Description                                      |
|---------|------------|--------------|--------------------------------------------------|
| v1.0    | 01/09/2022 |Khubaib Ahmad Qureshy, Muhammad Haris Azaz Khan  | VRF-lite      |

## Abbreviations

| **Term** | **Definition**                                                                                                                                  |
|----------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| VRF      | Virtual routing forwarding                                                                                                                      |
| MPLS     | Multi-Protocol Labelling System|
| SVI | Switch virtual Interface|
| PE | Provider Edge|
| P| Provider|
| LAN | Local Area Network|
| WAN | Wide Area Network|
| VPN | Virtual Private Network|
| VLAN | Virtual Local Area Network|
| L3 | Layer-3|

## Overview
  This document provides information about working of vrf-lite in sonic
## Introduction
  VRF (Virtual Routing and Forwarding) is associated with IP MPLS technology whereby an ISP 
creates Layer3 (or Layer2) VPNs for customers using VRF. Each VRF is like a separate virtual router 
with its own routing table on the same physical router.
  
  VRF-lite is a feature that enables a service provider to support two or more VPNs, where IP 
addresses can be overlapped among the VPNs. VRF-lite uses interfaces to distinguish routes for 
different VPNs and forms virtual packet-forwarding tables by associating one or more Layer 3 
interfaces with each VRF. Interfaces in a VRF can be either physical, such as Ethernet ports, or 
logical, such as VLAN SVIs, but a Layer 3 interface cannot belong to more than one VRF at any 
time.

## Architecture
