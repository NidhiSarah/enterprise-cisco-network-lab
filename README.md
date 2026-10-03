\# Enterprise Cisco Network Lab



A hands-on simulated enterprise network built and configured using \*\*Cisco Packet Tracer\*\*.



\## Project Overview



This project demonstrates practical Cisco networking and network administration skills, including network segmentation, inter-VLAN routing, DHCP, access control, secure remote administration, troubleshooting, and configuration verification.



\## Network Topology



\*\*Devices:\*\*



\* Cisco 1941 Router

\* Cisco Catalyst 2960 Switch

\* 2 Employee PCs

\* 1 Guest PC

\* 1 Server



\*\*Network Design:\*\*



| VLAN | Name    | Network         | Gateway      |

| ---- | ------- | --------------- | ------------ |

| 10   | USERS   | 192.168.10.0/24 | 192.168.10.1 |

| 20   | SERVERS | 192.168.20.0/24 | 192.168.20.1 |

| 30   | GUEST   | 192.168.30.0/24 | 192.168.30.1 |



\## Technologies \& Configuration



\* Cisco IOS

\* Cisco Packet Tracer

\* VLAN segmentation

\* 802.1Q trunking

\* Router-on-a-stick

\* Inter-VLAN routing

\* DHCP

\* Extended ACLs

\* SSH version 2

\* TCP/IP

\* DNS

\* Network troubleshooting



\## Network Implementation



\### VLAN Segmentation



Three VLANs were created to separate:



\* Employee/user devices

\* Server resources

\* Guest devices



\### Inter-VLAN Routing



Router-on-a-stick was implemented using router subinterfaces:



\* G0/0.10 — Users

\* G0/0.20 — Servers

\* G0/0.30 — Guest



\### DHCP



The Cisco router provides DHCP services for the network segments.



DHCP address ranges were configured with reserved addresses for network infrastructure and static devices.



\### Guest Network Security



An extended ACL was implemented on the Guest VLAN to prevent guest devices from accessing the User and Server networks while allowing permitted traffic.



\### Secure Remote Administration



SSH version 2 was configured on the router using local authentication for secure remote management.



\## Verification \& Troubleshooting



Network functionality was verified using Cisco IOS commands including:



```text

show vlan brief

show interfaces trunk

show ip interface brief

show access-lists

show ip dhcp binding

show ip ssh

```



Connectivity was tested between devices and across VLANs.



A switchport connectivity issue affecting an employee workstation was also identified and corrected during troubleshooting.



\## Project Files



\* `enterprise-cisco-network-lab.pkt` — Cisco Packet Tracer project

\* `screenshots/` — Configuration and verification screenshots

\* `configs/` — Redacted device configurations

\* `troubleshooting/` — Troubleshooting documentation



\## Security Note



This repository contains a simulated lab environment.



\*\*Passwords, private keys, and other sensitive credentials should never be committed to the repository.\*\*



Any credentials shown in configuration examples should be replaced with `<REDACTED>`.



\## Skills Demonstrated



This project demonstrates hands-on practice with:



\*\*Cisco Routing \& Switching | VLANs | Trunking | Inter-VLAN Routing | DHCP | ACLs | SSH | Network Troubleshooting | Cisco IOS CLI | Network Documentation\*\*



\## Disclaimer



This is a \*\*simulated enterprise networking lab created in Cisco Packet Tracer\*\* for hands-on learning and portfolio development. It does not represent professional production-network administration experience.



