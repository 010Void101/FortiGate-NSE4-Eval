## Implementation for Source NAT/PAT
- Two IP Pools are created one for NAT and one for PAT
- NAT and PAT pools are put into the Central Source NAT policy (Firewall is in Central Source NAT mode)
- NAT does 1:1 mappings of LAN ip addresses to one of the ips from the NAT pools
- PAT does port mappings of LAN ip addresses to different ports of ips from the PAT pools

| ![fw1_ip_pools](/assets/screenshots/04/fw1_ip_pools.png) |
| :--: |
| **FW1 IP Pools** |

| ![central_snat](/assets/screenshots/04/central_snat_nat.png) |
| :--: |
| **FW1 Central SNAT for NAT** |

| ![nat_cli](/assets/screenshots/04/fw1_nat_cli.png) |
| :--: |
| **FW1 NAT Sessions** |

| ![central_snat](/assets/screenshots/04/central_snat_pat.png) |
| :--: |
| **FW1 Central SNAT for PAT** |

| ![pat_cli](/assets/screenshots/04/fw1_pat_cli.png) |
| :--: |
| **FW1 PAT Sessions** |

## Implementation for Destination NAT
- The Web server is present inside the 172.16.0.0/24 DMZ network
- Web server DNAT rule is made by mapping a public IP with private IP
- Lastly a firewall policy is made and then HQ's web server can be accessed from internet and remote site

| ![dnat](/assets/screenshots/04/dnat.png) |
| :--: |
| **FW1 DNAT for Web Server in DMZ** |

| ![dnat_policy](/assets/screenshots/04/dnat_policy.png) |
| :--: |
| **FW1 DNAT Policy** |

| ![web](/assets/screenshots/04/web_srv_access.png) |
| :--: |
| **Web Server Access from outside** |
