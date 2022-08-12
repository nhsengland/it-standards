---
title: Networking Standards
description: >
   Defines the standards for all digital networking including Local and Wide-Area Networks (LAN, WAN).
stage: 3. Development Stage
created: 2021-06-14 10:16:44
lastUpdated: 2022-08-12 11:54:06
reviewDate: 2023-01-02
---

Note that networking for NHS England is subject to the requirements of the _[DSP Toolkit](https://www.dsptoolkit.nhs.uk/)_ and _[Cyber Essentials Plus](https://www.ncsc.gov.uk/cyberessentials/overview)_ certification.

## General

- All changes to networking MUST be pre-approved by the *CISW Infrastructure Team* and the *CISW Technical Design Authority* (TDA).
- All networking hardware and software MUST be currently supported by vendors and manufacturers. This MUST continue to be true for its contracted life. Once hardware or software is no longer under active support, it MUST be retired.
- All inter-network connections (LAN-LAN, LAN-WAN, etc.) MUST have a properly configured and actively managed firewall. (DSPT Assertion 9.7.1).
- All inbound connections from WAN to LAN MUST be disabled by default. Any inbound connections MUST be specifically defined with minimal connectivity.

## Wide-Area Networking

- WAN's should use software-defined networking to maximise flexibility and minimise cost.
- Use of private WAN's SHOULD be minimised. Justification must be provided if proposing the use of private networking rather than the Internet.

## Local-Area Networking

- All network wiring and switches MUST be at least 100Mbps and SHOULD be 1Gbps.
- All LAN hardware should use SD-LAN technology.
- All sites MUST have an edge firewall. This MUST be a centrally managed, SD-network device.
- Site firewalls MUST NOT be individually configured. A single, central configuration must be used.
- IoT devices, door controls, and consumer-grade devices (such as smart-TV's) MUST all go on at least separate VLANs and preferably on physically isolated LAN segments.
- Network-connected devices MUST be firmware and software updatable and MUST have access ids/passwords that can be changed.

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
