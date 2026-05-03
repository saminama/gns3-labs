# STP & Rapid PVST+

## Objective
Establish a stable and predictable Layer 2 topology by configuring Spanning Tree Protocol with Rapid PVST+ across all active VLANs.

## Design
coreSW1 sits at the top of the hierarchy as the root bridge for all VLANs. Switch1 is designated as the secondary root to ensure predictable failover if coreSW1 goes down. Two additional links were added — one between coreSW1 and Switch1, and one between coreSW1 and Switch2 — to prepare the topology for EtherChannel.

## What I Configured
- Enabled Rapid PVST+ on all switches
- Set coreSW1 as the root bridge for VLANs 10, 20, 30, and 99
- Set Switch1 as the secondary root bridge for all active VLANs
- Added a second link between coreSW1↔Switch1 and coreSW1↔Switch2

## Troubleshooting
No issues encountered during this phase. Verification confirmed coreSW1 as root on all VLANs and Switch1 as secondary.

## Screenshot
Topology
<img width="355" height="168" alt="switchesSTPPVST" src="https://github.com/user-attachments/assets/bfa51142-a632-433e-80f2-8e72c289e1fb" />

Cli
<img width="959" height="408" alt="stpcoresw" src="https://github.com/user-attachments/assets/d768749b-ea27-497c-9cc3-f96e696f08da" />

<img width="945" height="452" alt="stpsswitch1" src="https://github.com/user-attachments/assets/4262da42-213f-4dc2-88c1-9607143ad6c4" />


