# NAT Overload (PAT)

## Objective
Allow all internal VLANs to access the internet using a single 
public IP address on R1's outside interface.

## Design
NAT overload (PAT) is configured on R1. An ACL defines which 
internal networks are allowed to be translated. All traffic 
from VLANs 10, 20, and 30 is translated to R1's outside interface IP.

## NAT Configuration
| Direction | Interface |
|---|---|
| Inside | Gi1/0 (facing L3 switch) |
| Outside | Gi2/0 (facing ISP) |

## What I configured
- Defined inside and outside NAT interfaces
- Created ACL to permit internal subnets
- Configured NAT overload using the outside interface
- Added default route pointing to ISP

## Screenshot
<img width="943" height="170" alt="screenshotPAT" src="https://github.com/user-attachments/assets/6a8b9af6-de60-4ffa-8a84-9e16f727b59c" />

