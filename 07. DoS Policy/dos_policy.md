## Implementation
- A DoS policy is created to block ICMP and TCP floods, also blocking NMAP scans
- Quarantine is configured so that the ip address from which the attack is originated is logged and quarantined for a certain period of time
- Attackers can still spoof the ip address and attack again

| ![dos_policy](/assets/screenshots/07/dos_policy.png) |
| :--: |
| **DoS Policy** |

| ![dos](/assets/screenshots/07/dos.png) |
| :--: |
| **DoS Attack** |

| ![dos_scan](/assets/screenshots/07/dos_scan.png) |
| :--: |
| **NMAP Scan** |

| ![dos_logs](/assets/screenshots/07/dos_logs.png) |
| :--: |
| **DoS Logs** |

| ![quarantine](/assets/screenshots/07/quarantine_cli.png) |
| :--: |
| **Quarantine config** |

| ![quarantine](/assets/screenshots/07/quarantine.png) |
| :--: |
| **IP Quarantined** |

