# Intro to Gateway Redundancy Protocols Overview Guide

**Description/Overview:** *Gateway redundancy* is an essential implementation for network reliability: it provides continuous network availability as a result of having (potentially multiple) alternative/backup gateways configured in the event of failure. These gateways are automatically chosen to transmit data in the event of the primary gateways failing, which keeps connectivity active between internal and external network segments.

#### Table of Contents

1. [Gateway Redundancy](#redundancy)
2. [Hot Standby Router Protocol (HSRP)](#hsrp)
3. [Virtual Router Redundancy Protocol (VRRP)](#vrrp)
4. [Gateway Load Balancing Protocol (GLBP)](#glbp)
5. [Redundancy Protocols Comparison Table](#comparison)
6. [Supplemental Resources](#supplemental)

<hr />

## 1. <a name="redundancy">Gateway Redundancy</a>

(TODO)

<hr />

## 2. <a name="hsrp">Hot Standby Router Protocol (HSRP)</a>

(TODO)

<hr />

## 3. <a name="vrrp">Virtual Router Redundancy Protocol (VRRP)</a>

(TODO)

<hr />

## 4. <a name="glbp">Gateway Load Balancing Protocol (GLBP)</a>

(TODO)

<hr />

## 5. <a name="comparison">Redundancy Protocols Comparison Table</a>

| Characteristic | Hot Standby Router Protocol (HSRP) | Virtual Router Redundancy Protocol (VRRP) | Gateway Load Balancing Protocol (GLBP) |
| :---: | :---: | :---: | :---: | 
| Developer/Ownership | Cisco Proprietary | Open-Standard (Defined by Internet Engineering Task Force (IETF))| Cisco Proprietary |
| What It Does | Enables several layer-three switches or routers to show up as belonging to one gateway IP address (or virtual router). | Declares a virtual router in which a single elected router serves as the 'master', with other routers serving as backups. | Enables the concurrent usage and automatic selecting of more than one available gateway router, therefore also providing load balancing. |
| Failover | In the event that the active router fails, the next-highest priority standby router automatically becomes the active router. | If the master router fails, then the highest priority backup router automatically becomes the master router. | If an Active Virtual Forwarder (AVF) fails, then the Active Virtual Gateway (AVG) will automatically redirect traffic toward the still-functional AVFs. |
| RFC | [2281](https://datatracker.ietf.org/doc/html/rfc2281) | [2338](https://www.rfc-editor.org/rfc/rfc2338.html) (with others for more recent versions) | N/A |

<hr />

## 6. <a name="supplemental">Supplemental Resources</a>

* *[Official Cisco Documentation on HSRP](https://www.cisco.com/c/en/us/support/docs/ip/hot-standby-router-protocol-hsrp/9234-hsrpguidetoc.html)*
* *[Official Cisco Documentation on VRRP](https://www.cisco.com/c/en/us/support/docs/security/vpn-3000-series-concentrators/7210-vrrp.html)*
* *[Official Cisco Documentation on GLBP](https://www.cisco.com/en/US/docs/ios/12_2t/12_2t15/feature/guide/ft_glbp.html)*
