# 🔀 Multi-Subnet Routing & NAT Configuration

> Cisco Packet Tracer lab configuring static and dynamic routing across three subnets, built as part of SNHU CYB-210 (Network Security).

## 📋 Overview

Built and configured a three-subnet network topology (Subnet 1, Subnet 2, and Network 3) in Cisco Packet Tracer for CYB-210, implementing both static routing and RIP dynamic routing, along with NAT/PAT for internet-bound traffic and DHCP/DNS services for host connectivity. Completed as two sequential labs: an initial routing build (Project One) followed by a more advanced multi-router scenario (Project Two, Scenario 2).

## 🎯 Objective

Establish full connectivity across three separate subnets using a mix of static and dynamic routing protocols, translate internal addressing to a public address via NAT/PAT, and verify end-to-end reachability.

## 🧰 Tools & Concepts

- Cisco Packet Tracer
- Static routing
- RIP (Routing Information Protocol) dynamic routing
- NAT / PAT (Network & Port Address Translation)
- DHCP scope configuration
- DNS resolution
- ICMP-based connectivity testing

## 🔍 Methodology

1. **Topology build** — laid out Subnet 1 (192.168.1.1) and Subnet 2 (192.168.5.1) behind a shared router, with Network 3 connected via a separate router over a serial link.
2. **Static + dynamic routing** — configured both static routes and RIP on the Server Router so Subnet 1, Subnet 2, and Network 3 could all reach each other, using both methods together since static routes alone can be unreliable.
3. **NAT/PAT configuration** — defined inside/outside interfaces (Fa0/0 external to Server Main, Se2/0 internal to the Subnet Router) and configured NAT/PAT so end devices could communicate correctly across the boundary.
4. **Device migration** — moved all PCs and printers from Subnet 2 into Subnet 1, then reconfigured gateways and static IPs to match the new addressing.
5. **Serial link to Network 3** — connected the Subnet Router to the Network 3 router via a (slower) serial cable and configured RIP alongside static routing for cross-network reachability.
6. **DHCP & DNS setup** — implemented DHCP and DNS on the Network 3 server to control IP allocation and limit user count.
7. **Verification** — confirmed connectivity with successful ping tests between PCs across Network 3 and Network A.

## ✅ Key Outcomes

- Fully functional multi-subnet topology with mixed static/dynamic (RIP) routing
- Verified NAT/PAT translation for outbound traffic across subnet boundaries
- Successfully migrated all devices from Subnet 2 to Subnet 1 with zero connectivity loss
- Confirmed end-to-end connectivity between Network 3 and Network A via successful ping tests

## 🧠 Skills Demonstrated

`Cisco Packet Tracer` `Static & Dynamic Routing` `RIP` `NAT/PAT` `DHCP` `DNS` `Network Troubleshooting`

## 📁 Files

- [`docs/7-2_Project_2_Submit.docx`](docs/7-2_Project_2_Submit.docx) — write-up and screenshots for Project Two, Scenario 2 (routing, NAT/PAT, DHCP/DNS, verification pings)
- [`docs/CYB_210_Project_Two_Scenario_2_Student_File_Submit.pkt`](docs/CYB_210_Project_Two_Scenario_2_Student_File_Submit.pkt) — Packet Tracer file for Project Two, Scenario 2
- [`docs/CYB_210_Project_One_Packet_Tracer_Student_File_Submit.pkt`](docs/CYB_210_Project_One_Packet_Tracer_Student_File_Submit.pkt) — Packet Tracer file for the preceding Project One routing lab

---
🔗 Part of my [cybersecurity portfolio](https://samuelroulstone.com) · [Back to profile](https://github.com/samuelroulstone)
