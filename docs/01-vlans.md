# VLANs & Trunking

## Objective
Segment the network into departments to improve security and traffic management.

## VLAN Table
| VLAN | Name | Subnet |
|---|---|---|
| 10 | Sales | 10.0.10.0/24 |
| 20 | IT | 10.0.20.0/24 |
| 30 | Servers | 10.0.30.0/24 |
| 99 | Management | 10.0.99.0/24 |

## What I configured
- Created VLANs on all switches
- Configured access ports per department
- Configured trunk ports between all switches

## Screenshot
<img width="945" height="364" alt="screenshotsvlans" src="https://github.com/user-attachments/assets/846e8ca1-da3c-404b-b0ea-f0235ec24110" />

