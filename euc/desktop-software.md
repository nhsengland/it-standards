---
title: Desktop Software
description: >
   Selection and deployment processes for authorised desktop software
stage: 3. Development Stage
created: 2021-05-04 15:53:00
lastUpdated: 2023-01-27 11:39:34
---

For standard users, only two mechanisms exist for delivery of desktop software to a users desktop:
1) Centrally deployed.
2) Self-service from a controlled portal.

Standard users may not install or run arbitary desktop software.

It should be noted that **ALL** EUC devices issued by NHS England are subject to ongoing operational and security monitoring.
Compromised devices may be remotely locked and/or wiped.

## Specific User Classes

### "Power" Users

It is recognised that some users require more capabilities from their laptop. The NHS England Modern Desktop already accommodates most of these needs unlike the legacy builds. Power users will no longer be given local administration rights to their laptop in order to protect the integrity of the corporate devices and service.

Where local administrative access is required for specific reasons (such as a sponsored university course), a remote desktop environment can be provisioned.

Where users believe that they need a higher-than-average powered device, they can put in a request via the service management portal. However, they will be required to demonstrate a genuine need which will be reviewed by the Technical Design Authority (TDA). If approved, there will be a charge-back to the users local cost code for the additional cost.

### Data Scientists and Analysts

Many of the tools used have now been made available to all users via the NHS England Modern Desktop. Some specialist tools will not be made available on Modern Desktop and users will need to use a suitable remote desktop environment.

### Developers

Many developer tools have now been made available to all users via the NHS England Modern Desktop. However, there are some tools that are not compatible with a managed enterprise desktop. Most notably the full version of Microsoft Visual Studio. In those cases, users will need to use a suitable remote desktop environment.

## Legacy Services

Changes to any of the legacy managed desktops are no longer accepted except in a critical emergency.

## Modern Desktop Service

For the Modern Desktop, there are three tiers of application management, each of which carries a different level of cost and administrative overhead to the business while allowing maximum flexibility. The definitive list of Windows desktop applications is available in the [Modern Desktop Applications Catalogue](https://nhsengland.sharepoint.com/sites/ICTArchitectureDesign/SitePages/Modern-Desktop-Apps.aspx) which is available to all NHS England and related organisation staff and key partner vendors.

1) **Fully tested**
   
   Fully tested applications must be requested in advance via the IT request and triage process. They may also need to go
   through the Architecture Review Board for final sign-off. The triage process ensures that all aspects of architecture, techology,
   operations, delivery, service, security and IG are considered before an approval is given.
   
   Packaging and testing will follow a full process to ensure that such applications do not impact user or enterprise operations.
   The testing also ensures that collateral and scripts are available for service desk colleagues, operational issues are understood.
   
   Patching and upgrade schedules will also be agreed prior to deployment and will be enforced. Only versions that are still under
   active vendor support will be permitted to continue except under very specific circumstances where major enterprise disruption
   would result. In these cases, a full service, operational and business review will be needed in order to identify risks and
   mitigations. Senior business and IT managers will be asked to sign-off any resultant risks.
   
   Patches and upgrades will all be tested prior to deployment.
   
   Applications in this category are fully managed and supported (though specilist support may be outsourced).
   
2) **Minimally tested**

   Minimally tested applications must still go through the request and triage process and be approved.
   
   Once approved however, they will only be given and abbreviated packaging and cursory testing before being released to a self-service portal.
   
   Software updates will follow our standards which is that security patches will be rapidly applied but other updates will be kept at the minimum
   to keep the software in a currently supported version.
   
   Applications in this category will not be permitted to fall behind a currently supported version (at least recieving current security patches)
   even if this breaks user workflows.
   
   Users of these applications will recieve minimal support from the service desk. Any significant issues may result in removal of the software.

3) **Untested**

   Untested software applications may be ad-hoc requests from individuals or teams to support a localised business process.
   
   They will still be subject to the standard request and triage process and users will be encouraged to use existing standard
   software where appropriate.
   
   If approved, absolute minimal packaging and no testing will be applied before adding the application to a self-service portal.
   
   If reported problems arise from untested applications, they will be removed from the portal at short notice.
   
   Applications in this category will not be permitted to fall behind a currently supported version (at least recieving current security patches)
   even if this breaks user workflows.
   
   Users of these applications will not recieve support from the service desk. Any issues raised are likely to result in the application being removed from
   the users desktop.
   
   The purpose of this category is to provide a good level of business flexibility while maintaining control of costs and other overheads.

## Security & Privacy

Many desktop applications connect to external 3rd-party cloud services. Such applications MUST NOT be used without prior approval from both CISW and IG. Specifically, IT Security checks and Privacy checks will be required.

Local administrative elevated rights are no longer permitted on NHS England devices other than for approved administrators. This is to help ensure that the corporate services and users are protected. Alternative provisions are provided for the few exceptions.

NHS England actively monitor corporate end-user devices and services. This includes but is not limited to monitoring what applications have been used and what Internet endpoints people have accessed. Except for specifically identified threats and legal requests, this monitoring is mostly automated with threats and alerts surfaced in our Security Operations Centre and Service Management tools.

## Open Source & Free Software

It is UK Government and NHS policy that open source applications should be considered wherever feasible.

However, the following things should be considered:

- Open Source does not mean free - organisations and teams should consider investing in open source applications if they are relying on them.
- Free licenses may not be free for all uses - it is common for applications to have licenses that are free for personal and non-commercial use but charged for other use. It can be debatable as to whether an ALB such as NHS England would be eligable under non-commercial licensing.
- Free licenses do not mean that there is no cost - all IT comes with a cost. It costs money and resources to test, manage, deploy and support.
- Software suitable for domestic, non-professional use may be considered too risky for professional enterprise use. NHS England has in excess of 15,000 direct users to service and protect. It also has responsibilities across the NHS (2 million staff, 70 million patients) and the rest of Government along with suppliers and voluntary organisations. We cannot and will not put them at risk.
- Open source software may require significantly higher levels of administration than commercial software. This can make it uneconomic despite being "free".

