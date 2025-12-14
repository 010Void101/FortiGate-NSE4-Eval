## Implementation
- Vlan 50 server in Remote Site is protected by a transparent firewall
- Virtual Wire Pair is made on firewall which gives the advantage of a firewall in Transparent mode without actually switching the firewall from NAT to Transparent mode
- A Virtual Wire Pair policy is created and when server asks for DHCP it gets one from FW4 but logs are generated in Transparent Firewall too
- Transparent firewalls are hidden on the network as they dont have ip addresses and they give full security through security profiles

| ![vwire](/assets/screenshots/10/vwire.png) |
| :--: |
| **Virtual Wire Pair** |

| ![vwire_policy](/assets/screenshots/10/vwire_policy.png) |
| :--: |
| **Virtual Wire Pair Policy** |

| ![vwire_logs](/assets/screenshots/10/vwire_logs.png) |
| :--: |
| **Virtual Wire Pair Logs** |

