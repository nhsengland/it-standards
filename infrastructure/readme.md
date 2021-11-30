---
title: Infrastructure Standards
description: >
   This section of the standards covers all infrastructure. Whether Cloud-based, data-centre or on-premise.
stage: 3. Development Stage
created: 2021-06-08 13:51:00
lastUpdated: 2021-11-24 18:06:30
---

## Common Standards

These standards apply to all types of infrastructure.

## Cloud First

NHSEI's strategy and policy is to use Cloud over physical infrastructure.

Architectural approval MUST be sought before committing to any work that requires physical infrastructure.

When deploying cloud infrastructure, the following general approach must be followed: SaaS is preferred over PaaS over IaaS.

Cloud infrastructure MUST either belong to a vendor who will provide ongoing support and maintenance of the infrastructure for the whole life of the contract
_or_ it must use the NHSEI Microsoft Azure cloud infrastructure.

Where NHSEI cloud infrastructure is used, it will be subject to our development, support and documentation standards.

### All physical and virtual devices MUST be updatable

It will not be permitted to have infrastructure who's firmware, operating system or other key software elements cannot be updated no matter what the reason.

### All devices MUST have vendor or 3rd-party support

It will not be permitted to have infrastructure that has no support from the manufacturer, vendor or 3rd-party.

## Other Standards

* [Cloud Infrastructure](infrastructure/cloud/readme)
* [Physical Infrastructure (on-premise, data-centre)](infrastructure/physical/readme)
* [Network Infrastructure](infrastructure/networks)
