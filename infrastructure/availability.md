---
title: Availability
description: >
   Availability is a measure of the percentage of time that a system is functioning and able to meet defined workloads.  

   It includes availability of **user interfaces** to support users complete tasks and also availability to respond to input on the **system interfaces**
stage: 3. Development Stage
created: 2021-08-23 15:32:00
lastUpdated: 2021-12-21 09:45:57
author: Ben Heap
---

!> This section has not yet been reviewed and is subject to change.

![image](https://user-images.githubusercontent.com/9471595/130458486-d1138b90-bf43-44c8-bf9c-9623458b9a72.png)

All services are to state their overall availability using the the following classification as seen in the above table. 

- **Platinum**: Service Level Agreement - 365 days 24x7 | 99.9% availability | Disaster Recovery - 2 hours
- **Gold**: Service Level Agreement - Mon-Sat including Bank Holidays, 08:00 to 18:00 | 99.9% availability | Disaster Recovery - 4 hours
- **Silver**: Service Level Agreement - Mon-Fri not including Bank Holidays, 08:00 to 18:00 | 99.5% availability | Disaster Recovery optional
- **Bronze**: Service Level Agreement - Mon-Fri not including Bank Holidays, 08:00 to 18:00 | 98.0% availability | Disaster Recovery optional

Services may break down their availability for different parts of their service as they deem appropriate.

## Example Availability Non Functional Requirements (NFR)

| Type | NFR | Evidence |
| --- | --- | --- |
| System | The SLA for availability of hosting and system components must be 99.5% or higher | By review: (1) The architectural design should include components with combined support availability calculated at 99.5% or better (2) This should be to support all front-end and back-end (batch) processing capabilities |
| System | a method for calculating system target availability must be documented. This may be broken down per component | By review: Document the method for estimating availability based on published availability of chosen system components |
| System | The availability of the system to support user activity must be monitored. An automated method for determining availability (actual) through periods of 1, 6, 12 months must be documented | By review: -	Document the approach for determining actual availability of front-end capabilities, for example based on: (1) successful responses compared to requests, or (2) a measure of available use time compared to elapsed time. By test: -	demonstrate the calculation over trial periods of 1 week and longer |
| User Interface | The interface should be available with an SLA of 99.5% or higher, offering reduced functional capability (graceful degradation). In the extreme this should be in the form of an advisory notice of no service when other components aren’t available making progress through the user interface impossible. | By review:	The architectural design should include front-end components with a combined availability calculated at 99.5% or better. By test: (1) One or more tests designed to artificially sever connection between key data and business logic components should cause the front end to provide a clarifying message to indicate the service is not available. (2) In this condition the front end should restrict the user and prevent them from accessing unavailable parts of the system. |
| User Interface | The service must remain available in the presence of a distributed denial of service attack, including infrastructure layer attacks and application layer attacks | By review: The architectural design should include measures to protect against directed DDoS attack, including: CDN, firewalls, scalable resources with correct resource capacity limits identified. By test: Vulnerability testing of the solution should provide evidence the service withstands typical denial of service attacks |
| Data | The core database must be available when other components of the system may not be available (SLA 99.9%). Investigations must be possible even if the user interface is down. | By review: Selected components should support an SLA of 99.9% |
| Data | Data repositories to hold current or historic reports must be available for direct access when other components of the system may not be available (SLA 99.9%) | By review: Selected components should support an SLA of 99.9% |
| Archiving | The system archive of records must be available when other components of the system may not be available (SLA 99.9%). This may be direct access through service interfaces (cloud management consoles etc). | By review: Selected components should support an SLA of 99.9% |
| Archiving | Reports generated must be retained with compliance to the updated [Records Management Code of Practice 2020](https://www.nhsx.nhs.uk/information-governance/guidance/records-management-code/) | By review: The retention period for reports should be documented. By test: Process to retrieve historic reports based on date both within and beyond the retention periods |
| Reporting | Reports must be timely and generated within the specified period of their validity (e.g. daily reports made available in good time each day) | By test: Scripted tests to time the generation of reports under a system load representative of maximum users and activity |
| Reporting | Reports must become available immediately upon completion of their creation (within 5 minutes). | By test: Scripted tests to time the retrieval of reports under a system load representative of maximum users and activity |
| Reporting | Reports up to 12 months must be available for immediate access. Any reports required to be retained for more than 12 months must be available but this may be with a period of delay which must be no longer than 1 working day) | By review: A tiered archiving approach for reports to support within month, within year, and longer periods. By test: -	Process to retrieve historic reports based on date both within and beyond the retention periods |
| System Administration | Administrative controls for managing system resources should be accessible through internet channels that are highly available, including one or more of html console, command line, and API.   | By test: Direct and scripted access to resource status information tested |
| System Administration | Information regarding live service status for resources used in the solution must be directly available to system administrators. (Only cloud service providers that publish live resource and service availability should be considered for solution components) | By review: -	Review the cloud service status for resources selected for solution components |





