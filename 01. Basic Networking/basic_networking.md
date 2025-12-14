## Overview
A FortiGate Firewalls based architecture with multiple vendors between headquarters and remote site number 1. The goal is to explore, learn and implement every possible
functionality available in the evaluation license of FortiGate firewall version 7.0.17.
FW1, FW2 and FW3 are placed inside HeadQuarters while FW4 and both FW5 (HA cluster) is in Remote Site, HQ also support the shared web server and other servers e.g AD
and DHCP etc. RFC 5737 IP addresses are used as pseudu internet which are non routable on the internet for conformability of connection while actual internet access is
also present.

![architecture](/assets/screenshots/01/topology.png)

## Implementation
- Bootstrapping the firewalls
- Assigning IP addresses and names on ports, DNS and default routes
- Checking connectivity between all 3 firewalls in HQ 

| ![fw1_interfaces](/assets/screenshots/01/fw1_interfaces.png) |
| :--: |
| **FW1 interfaces** |
