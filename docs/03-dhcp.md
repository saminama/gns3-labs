# DHCP per VLAN

## Objective
Automatically assign IP addresses to end devices in each VLAN.

## Design
DHCP pools are configured on R1. Since the DHCP server is on a different 
subnet than the clients, ip helper-address is configured on each SVI 
to forward DHCP requests to R1.

## DHCP Pools
| Pool | Network | Gateway | DNS |
|---|---|---|---|
| pool1 | 10.0.10.0/24 | 10.0.10.254 | 8.8.8.8 |
| pool2 | 10.0.20.0/24 | 10.0.20.254 | 8.8.8.8 |
| pool3 | 10.0.30.0/24 | 10.0.30.254 | 8.8.8.8 |

## What I configured
- Created DHCP pools on R1 for each VLAN
- Excluded gateway IPs from DHCP pools
- Configured ip helper-address on each SVI pointing to R1

## Screenshot
<img width="947" height="266" alt="screenshotdhcp" src="https://github.com/user-attachments/assets/64e1bb2c-0740-4f85-a53a-4ccdb2cb4cda" />

