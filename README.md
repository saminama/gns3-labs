# Small Enterprise Network Lab

## Objective
Design and implement a small enterprise network simulating a real-world 
company environment with multiple departments, secure access, 
and internet connectivity.

## Topology
<img width="699" height="411" alt="2026-05-02 09_47_54-Small entrprise network that actualy works final boss pro max - GNS3" src="https://github.com/user-attachments/assets/e65dc675-2a20-4ae2-9634-a85892b2fefe" />


## Network Design
| Department | VLAN | Subnet |
|---|---|---|
| Sales | VLAN 10 | 10.0.10.0/24 |
| IT | VLAN 20 | 10.0.20.0/24 |
| Servers | VLAN 30 | 10.0.30.0/24 |
| Management | VLAN 99 | 10.0.99.0/24 |

## Skills Demonstrated
- VLANs & Trunking
- Inter-VLAN Routing (L3 Switch)
- OSPF
- DHCP per VLAN (ip helper-address)
- NAT Overload (PAT)
- Extended ACLs (Security Policy)
- SSH Hardening (Management access restricted to IT VLAN)

## Tools Used
- GNS3
- Cisco IOS

## Author
[Sami Namane] — Aspiring Network Engineer
