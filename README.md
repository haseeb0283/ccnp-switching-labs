# ccnp-switching-labs

CCNP Switching Labs

This repository contains configuration files and Packet Tracer topologies from my hands-on CCNP Switching lab practice. I’m documenting each step to reinforce my understanding and share my learning journey.

Lab 1: VLAN Trunking & VTP Domain Setup

Devices Used:
- Cisco 3560-24PS Multilayer Switches (3 switches)
- Cisco Packet Tracer 8.x

Lab Objectives:
- Configure 802.1Q trunk ports between switches
- Set VTP domain name (CORVIT) and mode
- Use both static trunking and dynamic desirable mode
- Verify trunk formation and VLAN propagation

Commands Used:

Trunk Port Configuration:
Switch(config)# interface range fa0/1 - 2
Switch(config-if-range)# switchport trunk encapsulation dot1q
Switch(config-if-range)# switchport mode trunk
Switch(config-if-range)# switchport nonegotiate

VTP Configuration:
Switch(config)# vtp domain CORVIT
Switch(config)# vtp mode server

Verification:
Switch# show interfaces trunk
Switch# show vtp status

Files Included:
- CCNP_Switching_Lab1.pkt — Packet Tracer topology
- Switch1_Config.txt — Running config for Switch 1
- Switch2_Config.txt — Running config for Switch 2
- Switch3_Config.txt — Running config for Switch 3 (optional)

Results:
- Trunk ports successfully established
- VTP domain correctly set
- VLAN 1 active and forwarding
- show interfaces trunk confirms trunking status

About This Project:
This is part of my journey through CCNP Enterprise Switching (ENARSI). I'm using these labs to better understand VLANs, trunking, STP, and L3 switching using multilayer switches.

Next Lab Coming Soon:
Inter-VLAN Routing with SVI Interfaces

Feel free to fork or clone this repo and use the labs in your own CCNP studies.

Connect with Me:
- LinkedIn: https://www.linkedin.com
- Email: your.email@example.com
