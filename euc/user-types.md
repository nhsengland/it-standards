---
title: EUC User Types
description: >
   Defines the different user types that are used to indicate what type of device that user requires.
stage: 3. Development Stage
created: 2021-05-04 15:53:00
lastUpdated: 2024-03-19 10:20:08
---

This document outlines the different types of users, the software and configuration they can expect, and the device types that they will be allocated as standard.

The currently identified types are:

1) Standard User
2) Power/Developer User
3) Highly Mobile User
4) User requiring Reasonable Adjustments

Device types are detailed in [Desktop Devices](./desktop-devices.md).

## 1) Standard User

This covers 80-90% of all users across NHS England.

### Device Allocation

Standard users will recieve a [standard laptop device](./desktop-devices.md#standard-device).

### Configuration

The standard configuration is a tightly locked-down desktop with no local administrive rights. The provides the greatest safety and security for the majority of the organisation.

Under the legacy services, the following restrictions apply:
* No local administrative rights
* No ability to install software
* Can self-install a limited set of optional applications from an Open Service software maintenance app and from the Microsoft Business Store.
* Cannot run arbitary software - this prevents downloaded executables from being run and protects against the majority of malware.

For the Modern Desktop design, the following restrictions apply:
* No local administrative rights
* No ability to install software
* Can self-install a pre-defined set of applications from the Microsoft Business Store and InTune self-service portal.
* Arbitary software _may_ be executable subject to dynamic restrictions by Microsoft Defender.

Adding new applications to the self-service portals will be a lot quicker and simpler under the Modern Desktop design. 

## 2) Power/Developer User

Users in this category are required by their roles to be handling large, complex documents or working with very large datasets or may be developing software or undertaking complex analytical analysis of data.

As such, they typically need more powerful devices and more flexibility over software.

A user who considers themselves in this category may ask their line-manager to put in a request for a "developer account".

Developer Accounts on the legacy services are separate to a users standard account (where they have access to standard corporate services).

Developer accounts have the following benefits:
* Local administrative rights - allowing local installation of desktop software and running of arbitary applications (subject to the dynamic
  protection of Microsoft Defender)
  
They have the following restrictions:
* They **MUST** still meet the minimum security standards. They must retain strong login credentials, encrypted drives, and centrally configured Microsoft Defender (inlcuding all of the "guard" services). Users deliberately configuring devices to avoid these restrictions will have their increased rights removed without warning and may be subject to disciplinary procedings.
* The device **MUST NOT** be shared with another person - whether that person is an employee of NHS England or not. 
  
  Note that it is possible to have a developer _device_ that could be shared. That would be a bespoke request to IT PMO and would be subject to different restrictions.
  
* Devices with developer accounts will have reduced support. 
  
  Should any local configuration changes or locally installed software be deemed to have caused issues, the user will be responsible for resolving those issues,
  the standard service desk will only be able to offer a device reset.

Developer accounts also come with the following user responsibilities:
* The _user takes full responsibility_ for the safety and security of the device, their account and any information accessed via the device.

  In particular, the user must be certain of the security and privacy issues arising from the installation and use of both local and cloud software and services.

* The user or their team/department takes responsibility for the support of any locally installed software or configuration changes. They may, of course have access to
  local specialist support or support from colleagues or vendors.
* The user or their team/department takes responsibility for the licensing of any locally installed software.

## 3) Highly Mobile User

Highly mobile users are presumed not to be required to author large, complex documents. Instead being more focused on reading/commenting-on documents, involved with online meetings, and using email.

Such users may choose to have an iPad Pro device _instead of_ a laptop. Users must agree with their line managers that such a device is suitable for their workload. Users may not choose to have both types of device.

## 4) User requiring Reasonable Adjustments

Reasonable adjustments are assessed by a standard processes. A specific laptop type is available that has a larger screen and may be suitable for some people with eyesight issues.
