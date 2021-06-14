---
title: Networking Standards
description: >
   Defines the standards for all digital networking including Local and Wide-Area Networks (LAN, WAN).
stage: 3. Development Stage
created: 2021-06-14 10:16:44
lastUpdated: 2021-06-14 17:30:39
reviewDate: 2022-05-01
---

Note that networking for NHSEI is subject to the requirements of the _DSP Toolkit_ and _Cyber Essentials Plus_ certification.

## General

- All changes to networking MUST be pre-approved by the CISW Infrastructure Team and the CISW Architecture Team.
- All networking hardware and software MUST be currently supported by vendors and manufacturers.
- All inter-network connections (LAN-LAN, LAN-WAN, etc.) MUST have a properly configured and actively managed firewall. (DSPT Assertion 9.7.1)
- All inbound connections from WAN to LAN MUST be disabled by default. Any inbound connections MUST be specifically defined with minimal connectivity.

## Wide-Area Networking

- WAN's should use software-defined networking to maximise flexibility and minimise cost

## Local-Area Networking

- 

### Corporately provisioned Wi-Fi

- MUST use WPA2 or better security.
- MUST not deliver more than 5 SSID's.
  
  Too many SSID's cause significant packet overheads that seriously impact Wi-Fi performance.

- Should use Azure Active Directory identity integration to the NHS England AAD if possible. Or at least AD Integration to the England domain.
- Should deliver GovWiFi in addition to corporate SSID's where possible.
- Should use device certificates where feasible (these may be required anyway for GovWiFi)

## Definitions

- LAN - Local Area Network. On-premise local networking that enables end user devices to communicate. LAN's have edge protection between themselves and WAN's.
- WAN - Wide Area Network. External inter-networking, provides interconnections between LAN's and cloud services. Includes but is not limited to the Internet.