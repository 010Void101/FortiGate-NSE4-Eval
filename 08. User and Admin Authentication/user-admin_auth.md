## Implemetation
- Users and Admins are created in Active Directory and mapped to groups in FortiGate
- Active Directory is integrated and a user is tested if the credentials are working fine which returns back all the information even nested groups information
- Users or Admins groups are put into firewall policies and when accessing the internet firewall asks for authentication
- While integrating AD an Administrator account is used however a service account should be used to decrease attack vector

| ![adsrv](/assets/screenshots/08/adsrv.png) |
| :--: |
| **Active Directory** |

| ![ldap_int](/assets/screenshots/08/ldap_int.png) |
| :--: |
| **Active Directory Integration** |

| ![test_user](/assets/screenshots/08/test_user.png) |
| :--: |
| **User Test** |

| ![groups](/assets/screenshots/08/groups.png) |
| :--: |
| **Firewall Groups** |

| ![admins](/assets/screenshots/08/admins.png) |
| :--: |
| **Firewall Admins** |

| ![ad_auth](/assets/screenshots/08/ad_auth.png) |
| :--: |
| **AD User Authentication** |

| ![ad_logs](/assets/screenshots/08/ad_logs.png) |
| :--: |
| **AD Logs** |

