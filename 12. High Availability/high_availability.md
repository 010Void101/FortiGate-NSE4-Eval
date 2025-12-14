## Implementation
- High Availability cluster of two firewalls is made in Active-Passive mode
- If active firewall goes down or either of the two monitor interfaces goes down the passive firewall will become active and traffic will not be disrupted
- Once in Active-Passive cluster both firewalls will sync all configurations using the Heartbeat interface and passive firewall's web GUI could not open
- A dedicated management ip is configured that will help opening the firewalls web GUI even after the sync

| ![ha](/assets/screenshots/12/ha.png) |
| :--: |
| **HA config** |

| ![ha1](/assets/screenshots/12/ha1.png) |
| :--: |
| **HA1 as Primary** |

| ![ha2](/assets/screenshots/12/ha2.png) |
| :--: |
| **HA2 as Primary** |

| ![ha1_cli](/assets/screenshots/12/ha1_cli.png) |
| :--: |
| **HA1 MGMT IP** |

| ![ha2_manage](/assets/screenshots/12/ha1_to_ha2_manage.png) |
| :--: |
| **HA2 MGMT IP** |

