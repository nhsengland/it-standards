# IT People Database

The IT People Database is a collection of tables maintained by Corporate IT that bring together various information about staff and other internal system users
(e.g. contractors, embedded and seconded staff, and other organisations that we provide support for such as NHSX, Leadership Academy, etc).

Any IT system that needs data about internal users can use this database so that a consistent set of information is made available to all systems and services.

In summary, the IT People DB:

*	Provides a single, common, reusable dataset for people related data required for many different internal IT systems.
*	Has a single daily standardised HR data feed for all E&I staff. Processed in an agreed fashion to make sense of the complex data from the Electronic Staff Record system.
*	Removes the need for the many current ESR extracts that are sometimes ad-hoc and provide inconsistent data due to lack of understanding 
  of the ESR data complexities or simply because the author of the extract wrote it in a particular way based on the request.
*	Allows for recording of people who are not on ESR – e.g. NHSX, HEE embedded staff, manual entries.
*	Integrates additional data from systems with other identity keys (e.g. AD, AAD, Mobile Phones) that are not linked to ESR.
*	Provides **identity mapping** tables that link disparate electronic identities – required for Staff Directory, T2T migration, Open Service & 
  A365 exit work, HR Dashboards, Service Now. Additional future requirements already noted and will be developed.

While this database does not directly provide IDAM capability, it _is_ consumed by systems that do.

Systems and services that already consume data from this database:

* Joint Staff Directory
* NHS E&I electronic ID card
* E&I IT Service Management Toolkit (Service Now)
* HR Dashboards

Systems and services due to use this data:

* Active Directory
* Azure Active Directory/Office 365
* IT Forms
* Estates emergency notification system
* ORIS
