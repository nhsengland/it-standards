---
title: Desktop Application Development
description: >
   Standards for the Development of Desktop Applications
stage: 3. Development Stage
created: 2021-06-10 09:06:00
lastUpdated: 2022-06-24 10:25:48
author: Julian Knight
---

In general, desktop applications SHOULD NOT be developed.

All applications for use on desktop operating systems should be developed as [**web applications**](/application-development/web-dev/readme).

Requests for the development of new desktop applications will generally be declined.

Desktop applications are mostly over-complex for the business requirements they are designed to meet.
In addition, they may need ongoing packaging and support, integration and testing on a wide variety of devices which adds significant cost and resource overheads that are not needed.

Should a desktop application be approved, there will need to be an agreed process and cost for ongoing maintenance and deployment/redeployment. Unmaintained apps will be removed.

## Java Runtime

!> No desktop applications may be developed for use in NHS England that make use of the Oracle Java Runtime Environment (JRE).

Not only does the JRE create unnecessary administrative and operation overheads, it also now has a commercial license and this is simply an unnecessary overhead.

Any desktop application presented for review that relies on Oracle JRE will be rejected. Failing that, the originator of the application will have to bear the ongoing costs.
