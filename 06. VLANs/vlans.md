## Implementation
- Created VLAN interfaces under the Trunk port (port 3)
- Making a group of VLANs and putting it in the policy and SNAT rule to activate VLANs
- As the server endpoint does not need to have internet access so its VLAN is not put into policy

| ![fw4_vlans](/assets/screenshots/06/fw4_vlans.png) |
| :--: |
| **FW4 VLANs** |

| ![vlan_policy](/assets/screenshots/06/vlan_policy.png) |
| :--: |
| **FW4 VLANs Policy** |

| ![vlan_snat](/assets/screenshots/06/vlan_snat.png) |
| :--: |
| **FW4 VLANs SNAT Rule** |

| ![vlan1](/assets/screenshots/06/vlan1.png) |
| :--: |
| **PC endpoints in VLAN 10 and 20** |

| ![vlan2](/assets/screenshots/06/vlan2.png) |
| :--: |
| **Server endpoint in VLAN 50** |
