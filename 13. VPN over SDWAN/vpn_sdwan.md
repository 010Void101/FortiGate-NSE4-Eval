## Implementation
- Normal creation of VPNs using wizard cannot be created over SD-WAN
- For VPN over SDWAN, SDWAN Zone is created with VPN options
- Then manual creation of Local and Remote subnets, VPN policies and routes alongwith IP addresses on tunnel interfaces
- Ping from Local (FW1) to Remote (FW4) subnet and FW1 will show as initiator in VPN network while FW4 is the responder
- IPSEC VPN is made in this part, the SSL VPN is not allowed in EVAL license

| ![vpn_over_sdwan](/assets/screenshots/13/vpn_over_sdwan.png) |
| :--: |
| **VPN option in SDWAN** |

| ![vpn_over_sdwan_2](/assets/screenshots/13/vpn_over_sdwan_2.png) |
| :--: |
| **VPN over SDWAN Zone** |

| ![addresses_vpn](/assets/screenshots/13/addresses_vpn.png) |
| :--: |
| **Address groups** |

| ![edit_vpn](/assets/screenshots/13/edit_vpn.png) |
| :--: |
| **Address groups in VPN** |

| ![vpn_policy](/assets/screenshots/13/vpn_policy.png) |
| :--: |
| **VPN Policies** |

| ![vpn_route](/assets/screenshots/13/vpn_route.png) |
| :--: |
| **VPN Route** |

| ![tunnel_int_ips](/assets/screenshots/13/tunnel_int_ips.png) |
| :--: |
| **Tunnel interface IPs** |

| ![vpn_ping](/assets/screenshots/13/vpn_ping.png) |
| :--: |
| **Ping from Local to Remote** |

| ![fw1_tunnel_status](/assets/screenshots/13/fw1_tunnel_status.png) |
| :--: |
| **FW1 Tunnel Status** |

| ![fw4_tunnel_status](/assets/screenshots/13/fw4_tunnel_status.png) |
| :--: |
| **FW4 Tunnel Status** |

| ![fw1_vpn_logs](/assets/screenshots/13/fw1_vpn_logs.png) |
| :--: |
| **FW1 VPN Logs** |

