# IP Addressing Table

| Device | Type | Interface | IP Address | Subnet Mask | VLAN | Gateway |
|---|---|---|---|---|---|---|
| R1 | Router | Gi1/0 | 192.168.0.1 | 255.255.255.252 | — | — |
| R1 | Router | Gi2/0 | 203.0.113.2 | 255.255.255.252 | — | — |
| ISP | Router | Gi0/0 | 203.0.113.1 | 255.255.255.252 | — | — |
| Core-SW | L3 Switch | Gi0/0 | 192.168.0.2 | 255.255.255.252 | — | — |
| Core-SW | L3 Switch | SVI VLAN 10 | 10.0.10.254 | 255.255.255.0 | VLAN 10 | — |
| Core-SW | L3 Switch | SVI VLAN 20 | 10.0.20.254 | 255.255.255.0 | VLAN 20 | — |
| Core-SW | L3 Switch | SVI VLAN 30 | 10.0.30.254 | 255.255.255.0 | VLAN 30 | — |
| Core-SW | L3 Switch | SVI VLAN 99 | 10.0.99.2 | 255.255.255.0 | VLAN 99 | — |
| SW1 | L2 Switch | SVI VLAN 99 | 10.0.99.4 | 255.255.255.0 | VLAN 99 | 10.0.99.2 |
| SW2 | L2 Switch | SVI VLAN 99 | 10.0.99.3 | 255.255.255.0 | VLAN 99 | 10.0.99.2 |
| PC1-PC2 | PC | NIC | DHCP | 255.255.255.0 | VLAN 10 | 10.0.10.254 |
| PC3-PC4 | PC | NIC | DHCP | 255.255.255.0 | VLAN 20 | 10.0.20.254 |
| PC5-PC6 | PC | NIC | DHCP | 255.255.255.0 | VLAN 30 | 10.0.30.254 |
