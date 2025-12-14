## Implementation
- Firewall policies are most crucial aspect of an NGFW
- The security profiles used are Web, DNS, Application Control, IPS and WAF (available on evaluation license)
- SSL inspection is also used but the already available "custom-deep-inspection" profile is modified as EVAL license only allows that
- Anti Virus profile is not available along with few settings in the Web and IPS profiles
- Most of security profiles work when the firewall policy is set into proxy based mode instead of flow based mode
- Secondly security profiles would require the SSL inspection already set for them to work properly

| ![fw1_policies](/assets/screenshots/05/fw1_policies.png) |
| :--: |
| **FW1 Policies** |

| ![fw3_policies](/assets/screenshots/05/fw3_policies.png) |
| :--: |
| **FW3 Policies** |

| ![fw4_policies](/assets/screenshots/05/fw4_policies.png) |
| :--: |
| **FW4 Policies** |

## Web Profile Implementation
- Static URL filter is used to block sites
- Options related to FortiGuard or FortiSandbox are not allowed in EVAL license

| ![web](/assets/screenshots/05/web/web.png) |
| :--: |
| **Web Profile** |

| ![web_logs](/assets/screenshots/05/web/web_logs.png) |
| :--: |
| **Web Profile Logs** |

## DNS Profile Implementation
- Safe Search, Static Domain Filter, DNS Translations are used
- External IP Blocklist is created on the web server in DMZ and integrated with firewall

| ![dns](/assets/screenshots/05/dns/dns.png) |
| :--: |
| **DNS Profile** |

| ![dns1](/assets/screenshots/05/dns/dns1.png) |
| :--: |
| **DNS Working** |

| ![dns2](/assets/screenshots/05/dns/dns2.png) |
| :--: |
| **DNS Working** |

| ![dns_logs](/assets/screenshots/05/dns/dns_logs.png) |
| :--: |
| **DNS Profile Logs** |

## Application Control Profile Implementation
- As an example Filter Overrrides is made to block Whatsapp and Facebook in social media category while letting Instagram pass
- Similar tuning of profile can be done for other categories like the P2P or Proxies 

| ![app](/assets/screenshots/05/appcontrol/app.png) |
| :--: |
| **Application Control Profile** |

| ![app1](/assets/screenshots/05/appcontrol/app1.png) |
| :--: |
| **Application Control Working** |

| ![app_logs](/assets/screenshots/05/appcontrol/app_logs.png) |
| :--: |
| **Application Control Profile Logs** |

## IPS Profile Implementation
- A simple Intrusion Prevention signature is made to block brute force alongside medium to high severity attacks
- For IPS to work Inbound SSL inpection should be configured as the attack traffic would be inbound towards the web server
- A very important feature the Botnet C&C settings is not allowed in the EVAL license

| ![ips](/assets/screenshots/05/ips/ips.png) |
| :--: |
| **IPS Profile** |

| ![ips1](/assets/screenshots/05/ips/ips1.png) |
| :--: |
| **IPS Working** |

| ![ips_logs](/assets/screenshots/05/ips/ips_logs.png) |
| :--: |
| **IPS Profile Logs** |

## WAF Profile Implementation
- A simple profile is made to block SQL injection and Extended SQL injection
- Web Application Firewall profile is very detailed and can be tuned a lot

| ![waf](/assets/screenshots/05/waf/waf.png) |
| :--: |
| **WAF Profile** |

| ![waf1](/assets/screenshots/05/waf/waf1.png) |
| :--: |
| **WAF Working** |

| ![waf_logs](/assets/screenshots/05/waf/waf_logs.png) |
| :--: |
| **WAF Profile Logs** |

