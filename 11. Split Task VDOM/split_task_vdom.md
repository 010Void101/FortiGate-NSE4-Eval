## Implemetation
- Virtual Domains particularly Multi-VDOM mode partitions a physical firewall into multiple virtual firewalls but EVAL license does not support this
- Split Task VDOM is mainly used to seperate management traffic from network traffic
- Two domains are automatically made when switching to Split Task VDOM, one is "root" which is for management traffic and one is "FG-traffic" which is for network traffic

| ![split_task_vdom](/assets/screenshots/11/split_task_vdom.png) |
| :--: |
| **Split Task VDOM** |

| ![global](/assets/screenshots/11/global_int.png) |
| :--: |
| **Global view** |
