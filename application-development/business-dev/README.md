---
title: Business Applications Development Standards
description: >
   Defines the standards for the development of bespoke business applications.
stage: 3. Development Stage
created: 2021-06-08 17:21:47
lastUpdated: 2021-06-08 18:07:23
---

# Business Applications Development Standards

Business applications are bespoke applications developed on corporate/business platforms and will typically use C#, C++, Visual Basic.net, SQL Server, etc. 

They may be hosted on-premise or in the cloud. However, please read the [Infrastructure Standards](/infrastructure) for requirements regarding hosting.

See also the [standards common to all development activities](../common-dev).

## Core

All business application development:

* MUST follow the [common standards](../common-dev)
* MUST use the common development stack defined by NHSEI

## Development Stack

The development stack for business applications is comprised of:

* **Microsoft .net** - for core business logic on the server (back-end).
* **Microsoft SQL Server** - for standard relational data management.
* **Browser Client** - for front-end client (user) interactions (using HTML, CSS and JavaScript).
* **REACT** - front-end library supporting client UI development.
* **JavaScript v6 (ECMA2015)** - front-end code MUST target this version of JS or be transpiled to it.
* **Azure DevOps Pipeline** - for Continuous Integration, project management, etc.
* **GitHub NHS England** - NHS England's organisation on GitHub. For code management.

Note that exceptions to the use of REACT and JS v6 will be considered but pre-approval must be sought before committing to them.