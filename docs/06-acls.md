# Access Control Lists (ACLs)

## Objective
Implement a security policy to restrict traffic between departments.

## Security Policy
| Source | Destination | Action |
|---|---|---|
| Sales (VLAN 10) | IT (VLAN 20) | Deny ❌ |
| Sales (VLAN 10) | Servers (VLAN 30) | Allow ✅ |
| Servers (VLAN 30) | Sales (VLAN 10) | Deny ❌ |
| Servers (VLAN 30) | IT (VLAN 20) | Deny ❌ |
| IT (VLAN 20) | Everywhere | Allow ✅ |

## What I configured
- Created extended ACLs on the L3 switch
- Applied ACLs inbound on VLAN 10 and VLAN 30 SVIs
- IT VLAN has no restrictions — full access

## Screenshot
<img width="944" height="276" alt="screenshotACL" src="https://github.com/user-attachments/assets/191a18fc-3201-4eee-aac3-5cfa451bac24" />

