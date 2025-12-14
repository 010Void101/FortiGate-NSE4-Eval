## Implementation
- For LAN 1 DHCP server is made on FW1, DHCP reservations are also created for some IPs
- A windows server in 10.10.0.0/24 network (LAN 1) is configured as DHCP server
- For LAN 2 DHCP server is the windows server in LAN 1
- FW2 is configured as DHCP Relay Agent as pool is present on windows server

| ![fw1_dhcp](/assets/screenshots/03/fw1_dhcp.png) |
| :--: |
| **FW1 DHCP config** |

| ![fw1_dhcp_ips](/assets/screenshots/03/fw1_dhcp_ips.png) |
| :--: |
| **FW1 DHCP IPs** |

| ![dhcp_pool](/assets/screenshots/03/dhcp_pool_for_fw2.png) |
| :--: |
| **DHCP Pool on Windows Server** |

| ![fw2_relay](/assets/screenshots/03/fw2_dhcp_relay.png) |
| :--: |
| **FW2 DHCP Relay config** |
