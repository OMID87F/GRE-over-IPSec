# GRE over IPSec (Cisco ↔ MikroTik)
## Overview
This project demonstrates a site-to-site VPN between Cisco IOS and MikroTik RouterOS using a GRE tunnel protected by IPSec.

The objective was to establish secure communication between two different vendors while gaining practical experience with tunnel configuration, routing, IPSec policies, and troubleshooting interoperability issues.


## Objectives
* Configure a GRE tunnel between Cisco and MikroTik routers.

* Protect the GRE tunnel using IPSec.

* Enable communication between remote LANs through the encrypted tunnel.

* Practice multi-vendor configuration and troubleshooting.


## Technologies Used
* Cisco IOS
* MikroTik RouterOS
* GNS3
* GRE Tunnel
* IPSec
* Static Routing


## Repository Structure
```
README.md
Documentation.md
Topology.png
Sources/
```


## Validation
The implementation was verified by:

* Establishing basic IP connectivity.
* Verifying GRE tunnel operation.
* Testing LAN-to-LAN communication.
* Confirming IPSec tunnel establishment.
* Validating encrypted traffic between both sites.


## Troubleshooting
One of the main challenges occurred during IPSec Phase 2 negotiation.

Although IKE Phase 1 completed successfully, the IPSec Security Association was not established, preventing GRE traffic from passing through the tunnel.

The issue was resolved by ensuring consistent IPSec policy parameters on both devices and initiating traffic across the GRE tunn
el to trigger SA establishment.


## Documentation
Detailed configuration steps, screenshots, verification, and troubleshooting notes are available in `Documentation.md`.

> **Note:** The detailed documentation is currently written in Persian (Farsi).


## Learning Outcomes
Through this project I gained hands-on experience with:

* Multi-vendor interoperability
* GRE tunnel deployment
* IPSec implementation
* Static routing across tunnels
* Network troubleshooting and verification
