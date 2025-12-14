## Implementation
- Dynamic routing is configured between all 3 HQ firewalls
- OSPF is used as the primary routing protocol because its administrative distance is lesser
- RIPv2 is used as the backup routing protocol as its administrative distance is greater 
- BGP is used between the edge firewalls of both the HQ and Site 1 (FW1 and FW4)
- The routing database shows all the activated routing protocols

| ![fw1_routing](/assets/screenshots/02/fw1_dynamic.png) |
| :--: |
| **FW1 routing table** |

| ![fw1_routing_d](/assets/screenshots/02/fw1_dynamic_cli.png) |
| :--: |
| **FW1 routing database** |

| ![fw2_routing](/assets/screenshots/02/fw2_dynamic.png) |
| :--: |
| **FW2 routing table** |

| ![fw3_routing](/assets/screenshots/02/fw3_dynamic.png) |
| :--: |
| **FW3 routing table** |

| ![fw4_routing](/assets/screenshots/02/fw4_dynamic.png) |
| :--: |
| **FW4 routing table** |

| ![fw4_routing_d](/assets/screenshots/02/fw4_dynamic_cli.png) |
| :--: |
| **FW4 routing database** |
