# Inter-VLAN Routing

## Objective
Enable communication between VLANs through a Layer 3 switch.

## Design
Traffic between VLANs is routed through SVIs (Switched Virtual Interfaces) 
on the core L3 switch. Each VLAN has a dedicated SVI acting as the 
default gateway for that department.

## SVI Configuration
| VLAN | SVI IP | Department |
|---|---|---|
| VLAN 10 | 10.0.10.254 | Sales |
| VLAN 20 | 10.0.20.254 | IT |
| VLAN 30 | 10.0.30.254 | Servers |
| VLAN 99 | 10.0.99.2 | Management |

## What I configured
- Enabled `ip routing` on the L3 switch
- Created SVIs for each VLAN with gateway IPs
- Configured trunk ports to carry all VLANs

## Screenshot
<img width="945" height="364" alt="screenshotsvlans" src="https://github.com/user-attachments/assets/64132230-457b-42ba-9e0f-5a8fd026ec6c" />

