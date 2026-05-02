# SSH Hardening

## Objective
Secure remote management access by enabling SSH and restricting 
access to IT VLAN only.

## Security Policy
- Telnet is disabled on all devices
- SSH version 2 is enabled on all devices
- Only VLAN 20 (IT) can SSH into network devices

## Devices Configured
| Device | Management IP |
|---|---|
| R1 | 192.168.0.1 |
| Core-SW | 10.0.99.2 |
| SW1 | 10.0.99.4 |
| SW2 | 10.0.99.3 |

## What I configured
- Set hostname and domain name on all devices
- Generated RSA keys on all devices
- Configured SSH version 2
- Restricted VTY lines to SSH only
- Applied access-class to allow only VLAN 20

## Screenshot
<img width="944" height="111" alt="screenshotSSH" src="https://github.com/user-attachments/assets/b7816dd3-c267-46c1-87e0-95eba6f30349" />

