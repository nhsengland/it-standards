---
title: Standards for new Service Procurements
description: >
   NHS England operates a cloud-first and SaaS-first approach to IT in line with UK Government guidelines.
   As such, it is much preferred for new IT to be procured as a managed _Service_ rather than as a system.

   This section provides some guidance on expected requirements for service procurements and should be included in ITT's.
stage: 3. Development Stage
created: 2021-11-29 12:05:40
lastUpdated: 2022-06-27 10:13:40
author: Julian Knight
---

In addition to these standards, all services procured by and for NHS England MUST adhere to the UK Government [Technology Code of Practice](https://www.gov.uk/guidance/the-technology-code-of-practice). Larger or public-facing systems will need to go through Cabinet Office approvals which are measured against the TCoP. This page provides some more NHS England specific standards but clearly overlaps with the larger TCoP.

!> These standards should be used by anyone in NHS England looking to procure IT services.<br>They should also be used by vendors providing services to NHS England. Any variation from these standards need to be explained.<br>There _can_ be exceptions as long as there are valid business reasons and as long as the risks and variations are manageable.

## Procure services not systems

Wherever feasible, NHS England should be procuring _services_ and not _systems_.

This means that the infrastructure, operating systems, and system software is all fully managed by a vendor.

The vendor is also responsible for keeping everything current in line with our security requirements.
Notably that all services and software MUST remain on in-support versions at all times and must be fully security patched.

## We are rarely unique

While organisations and teams often think of themselves as having unique needs, this is actually rarely the case.

As such, bespoking of services and software is strongly discouraged. It forms a tight coupling to the service, and
makes the general support and upgrade of the service harder.

Instead, as consumers of a service, NHS England should be looking to adopt general best-practice that has been formulated across multiple consumers over time.

Please see the [overview of this section](Services/readme.md) for more detailed reasoning.

## All IT services must have defined exit plans

Nothing lasts forever and it is critical that exit plans exist at the start so that the business have confidence
that services can be rehomed or transformed as needed.

## Platform vendor clouds should be used, not supplier clouds

For large-scale and global services in particular (e.g. SAP), it is much preferred to use the original platform vendor's cloud infrastructure
rather than a supplier/reseller infrastructure.

Ideally, that platform vendor should be operating a multi-tenanted platform and so have experience of on- and off-boarding organisations.

The purpose of this is to try and minimise supplier lockin. It is also to discourage bespoking of services and instead encourage multi-customer services
to be improved for all customers resulting in everyone benefitting from best practices.


## Services MUST have well defined integration architectures including API's, data schema's, timing and processes

When taking on off-the-shelf services, it is critical that those services have well-defined integration architectures. This enables easier offboarding where necessary
but also enables a more flexible approach whereby other services and systems can provide or consume information without expensive, bespoke integrations.

This is especially important for services that may be used by multiple NHS organisations. The NHS is a very complex collaboration of independent organisations and it
must not be assumed that they will all be able to operate in the same way, have the same budgets, or have the same requirements.

## IP, definitions, documentation of Data, interfaces, API's, data schema's, etc. BELONGS TO THE CROWN, not the vendor or supplier

In keeping with other standards and aligned to public spending, the intellectual property, definitions and documentation for all service data, interface and API definitions, and
data schema's belongs to the Crown.

Intellectual property for services provided on behalf of NHS England may belong to the Crown or to the supplier depending on which may make best use of the IP on behalf of the UK public.

Any data belongs to the Crown as do any backups.

This is to ensure that, upon service exit, sufficient knowledge is retained and that a new service can be created without significant disruption to users and interfaces.

It should also be noted that such open standards benefit the vendor as much as the consumers of a service.

## Integration points should use open standards wherever possible

Wherever possible, API's, data schema's, security and other interfaces must use open standards.

Open standards facilitate flexibility, minimise cost and complexity, and facilitate on-/off-boarding to and from services. They also benefit from external design and development input.

## Data and data backups must be transferable on service exit

It must always be acknowledged that all data belongs to the crown and must be made available at or before contract exit.

## Services must include business continuity plans

The project leading the delivery of a new IT service must define the business continuity requirements for use of the service.
However, the vendor and/or supplier are responsible for providing suitable evidence and documentation regarding business continuity
of a service and its underlying systems.

The NHS England BCDR team are available to support any area of the business standing up new services. They will help create a BCDR runbook and help to assess business criticality.

## New and changed IT services must be approved before procurement

It is important to engage IT before procuring services. See below for additional reasons.
As a minimum, it is needed to validate new services to ensure a good fit with the strategic technology and service management for NHS England and X.

There are three or four key governance processes that support this. 

### The _Architecture Review Board (ARB)_ 
Meets fortnightly and is made of of senior digital and IT staff across NHS England, HRA, Leadership Academy, and other supported bodies. It operates a rotating chair from amongst its members.

There is representation from service, infrastructure, security, IG, GDS assessors, data and analytics departments.

The ARB provides *technology approval* for business cases. It also assesses proposals for projects and services containing *architectures* that may differ from our existing ones.

### The _CISW Technical Design Authority board_ 
Meets weekly. It's purpose is to approve changes to IT and to ensure that the various technology areas are aware of strategic and operational changes. The Head of Architecture is the chair of the TDA.

It reviews design, development and infrastructure issues and proposals from across the business and provides technology approval for design change, especially as it impacts Core IT.
In addition, it reviews business cases against possible impact on core IT.

It contains representatives from all IT areas including security, service, architecture, and infrastructure. It also has representatives from other supported organisations and from key operational suppliers.

TDA will generally be able to make a rapid decision on a request and ensure that it moves on to the team best able to deal with the request. In addition, it will ensure that other approvers (e.g. IT Security, finance, commercial, service) are made aware and that they will respond accordingly.

### The _Digital Products Assurance Group (DPAG)_
This group pre-assesses proposals that need to be assessed under the Cabinet Office GDS standards (now CDDO).
This includes anything that is classed as a public digital service. It also includes any mobile app development and may include very large IT projects and services.
Business cases should generally be idenified as being "digital" so that DPAG are engaged early. However, if something misses that classification, 
it will be picked up during the ARB business case assessment. DPAG and the GDS assessors have seats on the ARB.

## IT Services must be centrally recorded

As new services are procured or existing services updated or renewed, a log of the details must be kept in the *Configuration Management Database* (CMDB)
which is maintained by IT in Service Now.

Commercial and product lifecycles must be tracked to enable look-ahead pipelines of work to be planned.
Records of business and vendor contacts are also kept along with summaries of key information such as numbers of licenses, dependencies, etc.

The CMDB supports various critical management and governance functions. It helps with cyber security and service incidents, ongoing license management, budgeting, support, strategic and architectural planning, etc.

## IT should have an Intelligent Client Function (ICF) role in IT services

It is important to get IT engaged early as they can help with standards, design, service management, security, procurement and more.
Early engagement helps avoid later pitfalls during procurement, design, implementation and running.

IT are also responsible for governance of IT services, systems, software, and infrastructure and will triage new requests and business cases and ensure that the right teams
and governance models are engaged.

IT can also provide ongoing help and support for IT services in these areas and more:

- Supplier and multi-supplier management
- Service monitoring
- Front-line service desk and incident management
- Cyber security incident management, governance, monitoring and support
- Commercial, procurement and financial support
- Financial monitoring (via open book charging)
- Standards
- Architecture & design governance and support
- Project and programme management
- Supplier integration with service desk
- Strategy and policy alignment

## Business cases for IT services must be approved by IT and the ARB

This is part of the technical, financial and commercial governance of NHS England.

New and significantly changed services will be assessed for fit to the NHS England policies and strategies.

Proposed services that overlap existing services will be questioned at the Architecture Review Board (ARB) and may not
be approved until evidence is provided that the existing service isn't viable for the new use.

The IT PMO team manage the governance processes both for business case approval and for the triage of requests and engagements with IT.

## Changes to live services must be put through the NHS England CAB

NHS England operate a Change Advisory Board (CAB) on a weekly basis.

All changes to live IT services must be submitted to CAB for approval prior to any live change.

For services running on vendor cloud infrastructure, only user- or interface-impacting changes need to go through the NHS England CAB.

## Technical standards

### No client dependencies

Procured services must not have dependencies on client apps (e.g. laptop/desktop applications or browser extensions).

NHS England operates a strategy that requires user-facing interfaces to be browser based.

Supported browsers must be kept "evergreen" and are restricted to *currently supported versions* of the following browsers:

* Microsoft Edge (the default browser for NHS England)
* Google Chrome
* Mozilla Firefox
* Apple Safari

Services must continue to support *current* versions of browsers as they evolve. Note that the development standards on this site have additional information about browser support.

**Specifically, no laptop/desktop applications will be approved that rely on the Oracle Java client.**

Services *may* specify local applications/extensions where those are not central to the use of the service. In other words, where they may provide some additional benefit to users. 
However, there is no guarentee that those will be accepted into live service. Any such software must not disadvanage the majority of users and all operation of the service must be
possible without such software.

### No private networks

The traditional use of private Wide Area Networks to add an additional layer of perceived security to a service is no longer sustainable and will not generally be accepted.

IT services should use a "Zero Trust" model of security. Access to services should be over public networks (the Internet).

### Accessibility

All user-facing services (both standard and administrative use) must meet the required levels of accessibility. This is both a legal as well as a moral requirement.

See the [accessibility development standards](application-development/common-dev/accessibility.md) page for more detail.

### Performance requirements

The business consumers of any service must define their core performance requirements for any IT service.

The IT service itself must document and communicate any performance requirements prior to procurement. 

Such requirements may include (but isn't limited to):

* Client memory, or storage
* Minimum CPU requirements
* Screen sizes
* Network bandwidth
* NHS England infrastructure required
* Maximum concurrent users
* ...

Anything that could constrain expected performance should be highlighted prior to procurement and ongoing throughout the live running period.

Note that NHS England maintains an *End User Compute (EUC) Hardware Baseline* which defines the current desktop and mobile hardware standards. This is available to projects and engaged vendors on request to CISW.

## Security, privacy and identity

Please see the pages under the common development standards section and the separate security section for details about standards covering security and identity & access management.
There are significant requirements in this area for any new IT service.

In summary:

* All suppliers and vendors must be at least Cyber Essentials Plus certified.

  Alternatively, they may be ISO28001 certified.
  
* Single sign-on (SSO) must always be an option.
  
  Internal NHS England users should not be subject to any other sign-on than their cloud identity sign-on.
  For systems that service the NHS or wider, our external identity store should generally be used.

  SSO must use open standards. Typically OAuth or SAML.

  Services not meeting these requirements will come under additional scrutiny and may be rejected.

  See the [Identity & Acess Management (IDAM)](idam/) sections of the standards for more detail.

* All actions and events requiring security must be logged and the individual making changes must be clearly identified.
  
* There are existing, strategic identity stores and processes for NHS England. Contact the NHS England Cyber Security team or the Head of Architecture for details.

  Proposals outside of these are unlikely to be accepted unless there are exceptional circumstances.

* All information is to be classified according to the UK Government data classification rules.
  
  Unless otherwise specified, all information is classified as at least *OFFICIAL*. Personally identifiable data (including patient data) is classified as *OFFICIAL-SENSITIVE:Personal*.
  Commercially sensitive data is classified as *OFFICIAL-SENSITIVE:Commercial*.

* All information relating to NHS England should generally be kept within England. Offshore data and offshore data access will be subject to additional scrutiny and governance.
  
* All services will be subject to the requirements to produce a Data Protection Impact Assessment (DPIA, IG) and a System Level Security Policy (SLSP, Cyber Security).
  
* All services accessible over the Internet must undertake at least a Penetration Test, undertaken using recognised processes by a certified and independent assessor. 
  Alternatively, suitable evidence of a current assessment may be provided.