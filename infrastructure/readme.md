---
title: Infrastructure Standards
description: >
   This section of the standards covers all infrastructure. Whether Cloud-based, data-centre or on-premise.
stage: 3. Development Stage
created: 2021-06-08 13:51:00
lastUpdated: 2022-06-24 10:42:11
---

## Common Standards

These standards apply to all types of infrastructure.

## Cloud First

NHS England's strategy and policy is to use Cloud over physical infrastructure.

Architectural approval MUST be sought before committing to any work that requires physical infrastructure.

When deploying cloud infrastructure, the following general approach must be followed: SaaS is preferred over PaaS over IaaS.

Cloud infrastructure MUST either belong to a vendor who will provide ongoing support and maintenance of the infrastructure for the whole life of the contract
_or_ it must use the NHS England Microsoft Azure cloud infrastructure.

Where NHS England cloud infrastructure is used, it will be subject to our development, support and documentation standards.

### All physical and virtual devices MUST be updatable

It will not be permitted to have infrastructure who's firmware, operating system or other key software elements cannot be updated no matter what the reason.

### All devices MUST have vendor or 3rd-party support

It will not be permitted to have infrastructure that has no support from the manufacturer, vendor or 3rd-party.

### Infrastructure definitions and deployment

The CISW Infrastructure Team along with the CISW Technical Design Authority (TDA) have responsibility over infrastructure change. Prior to live deployment, the Change Advisory Board must also be notified. Any proposed infrastructure changes that are different to the accepted architecture MUST also be reviewed and approved by the Architecture Review Board (ARB).

All infrastructure MUST have suitable design documentation that must be approved before hardware/software procurement and deployment. 

Wherever feasible, infrastructure MUST be defined using templating tools such as Azure Templates or Kubernetees. Consult with the CISW Infrastructure Team before deciding on the templating tool to use.

Note that Docker is NOT part of NHS England's standard toolchain and should not be used.

## Other Standards

* [Cloud Infrastructure](infrastructure/cloud/readme)
* [Physical Infrastructure (on-premise, data-centre)](infrastructure/physical/readme)
* [Network Infrastructure](infrastructure/networks)
