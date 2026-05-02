# OSPF

## Objective
Enable dynamic routing between R1 and the core L3 switch so all 
VLAN networks are reachable from the router.

## Design
OSPF Area 0 is configured on R1 and the L3 switch. The router 
advertises the default route to the L3 switch using 
default-information originate.

## OSPF Neighbors
| Device | Router ID | Neighbor |
|---|---|---|
| R1 | 203.0.113.2 | Core-SW |
| Core-SW | 192.168.0.2  | R1 |

## What I configured
- Enabled OSPF process 1 on R1 and L3 switch
- Advertised all networks in Area 0
- Used default-information originate on R1 to push default route

## Screenshot
OSPF neighbor
<img width="943" height="109" alt="screenshotospfneighbors" src="https://github.com/user-attachments/assets/562ced89-544e-42ec-a795-cc0f89c32d89" />

Routing table 
<img width="944" height="448" alt="screenshotiproute" src="https://github.com/user-attachments/assets/8fcb0c4d-b1e0-4a5a-9ff3-2c2cd812306b" />



