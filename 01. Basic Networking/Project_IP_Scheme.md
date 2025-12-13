## Management/Internet Network = 192.168.149.0/24

| Port                     | IP address             |
|--------------------------|------------------------|
| FW1 port1                | 192.168.149.91         |
| FW2 port1                | 192.168.149.92         |
| FW3 port1                | 192.168.149.93         |
| FW4 port1                | 192.168.149.94         |
| FW5-HA1 port1            | 192.168.149.95         |
| FW5-HA2 port1            | 192.168.149.95 (sync)  |
| Router-ISP-1 e0/0        | 192.168.149.60         |
| Router-ISP-2 e0/0        | 192.168.149.65         |
| FW-Transparent port1     | 192.168.149.80         |
| FW5-HA1 port1 (mgmt-ip)  | 192.168.149.75         |
| FW5-HA2 port1 (mgmt-ip)  | 192.168.149.76         |


## ISP-1 Network = 203.0.113.0/24 (RFC 5737)

| Port                     | IP address             |
|--------------------------|------------------------|
| Router-ISP-1 e0/1        | 203.0.113.60           |
| FW1 port4                | 203.0.113.91           |
| FW4 port4                | 203.0.113.94           |
| Kali Outside             | 203.0.113.50           |
| Linux Outside            | 203.0.113.55           |
| Web Server VIP           | 203.0.113.200          |
| PAT Pool                 | 203.0.113.181-182      |
| NAT Pool                 | 203.0.113.185-187      |


## ISP-2 Network = 198.51.100.0/24 (RFC 5737)

| Port                     | IP address             |
|--------------------------|------------------------|
| Router-ISP-2 e0/1        | 198.51.100.65          |
| FW1 port5                | 198.51.100.91          |


## FW1 Lan1 Network = 10.10.0.0/24

| Port                     | IP address             |
|--------------------------|------------------------|
| FW1 port2                | 10.10.0.91             |
| FW2 port4                | 10.10.0.92             |
| FW3 port4                | 10.10.0.93             |
| Windows Server DHCP      | 10.10.0.100            |
| LAN1 PCs                 | 10.10.0.151-160 (dhcp) |


## FW2 Lan2 Network = 10.20.0.0/24

| Port                     | IP address             |
|--------------------------|------------------------|
| FW2 port2                | 10.20.0.92             |
| LAN2 PCs                 | 10.20.0.201-220 (relay)|


## FW3 Lan3 Network = 10.30.0.0/24

| Port                     | IP address             |
|--------------------------|------------------------|
| FW3 port2                | 10.30.0.93             |
| LAN3 PCs                 | 10.30.0.151-160        |


## DMZ Network = 172.16.0.0/24

| Port                     | IP address             |
|--------------------------|------------------------|
| FW1 port3                | 172.16.0.91            |
| Active Directory Server  | 172.16.0.110           |
| Web Server (Ubuntu)      | 172.16.0.100           |


## FW4 Lan4 Network = 10.40.0.0/24

| Port                     | IP address             |
|--------------------------|------------------------|
| FW4 port2                | 10.40.0.94             |
| LAN4 PCs                 | 10.40.0.151-160 (dhcp) |
| FW4 port3 (VLAN 10)      | 10.40.10.94            |
| FW4 port3 (VLAN 20)      | 10.40.20.94            |
| VLAN 10 PCs              | 10.40.10.141-150 (dhcp)|
| VLAN 20 PCs              | 10.40.20.141-150 (dhcp)|
| FW5-HA1 port4            | 10.40.0.95             |
| FW5-HA2 port4            | 10.40.0.95 (sync)      |
| FW4 port3 (VLAN 50)      | 10.40.50.94            |
| VLAN 50 Devices          | 10.40.50.191-200 (dhcp)|


## HA Network = 10.50.0.0/24

| Port                     | IP address             |
|--------------------------|------------------------|
| FW5-HA1 port3            | Heartbeat              |
| FW5-HA2 port3            | Heartbeat              |
| FW5-HA1 port2            | 10.50.0.95             |
| FW5-HA2 port2            | 10.50.0.95 (sync)      |
| HA-LAN PCs               | 10.50.0.50             |

