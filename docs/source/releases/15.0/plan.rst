Build 15.0 Plan
========================

..  toctree::
    :glob:
    :maxdepth: 3

    plan.rst

.. |br| raw:: html

  <br/>

The Planetary Data System (PDS) is a long-term archive of digital data products returned from NASA's planetary missions, and from other kinds of flight and ground-based data acquisitions, including laboratory experiments. But it is more than just a facility - the archive is actively managed by planetary scientists to help ensure its usefulness and usability by the world wide planetary science community.

The following page outlines the planned PDS software enhancements, bug fixes, and impacted requirements for the upcoming Build .

A more detailed breakdown of these tasks by date and priority can be found in our `Zenhub Roadmap <https://app.zenhub.com/workspaces/pdsen-workspace-5c87e859b7a0872dd10b87c5/roadmap>`_ (login required).

Key Dates
+++++++++

.. list-table:: Key Dates for Discipline Nodes
    :widths: 20 20 20 40
    :header-rows: 1

    * - Date
      - Name
      - Responsible Party
      - Description
    * - 08/13/24
      - SCR Freeze Date
      - DDWG
      - Freeze date for identifying SCRs to be implemented in this release.
    * - 08/22/24 - 10/03/24
      - Standards Documents Updates Due
      - Document Authoring Team
      - Updates to PDS4 standards documents due to EN for review.
    * - 10/24/24 - 11/14/24
      - Beta Testing Period
      - DNs, IPDA
      - Changes to PDS4 IM and system components available for beta testing.
    * - 10/24/24 - 11/14/24
      - dLDD Integration and Test
      - dLDD Stewards
      - Auto-generated dLDDs should be reviews by dLDD Stewards, and final updates to dLDDs should be completed during this time.
    * - 10/24/24 - 11/14/24
      - Standards Documents Review Due
      - Document Review Team
      - Review updates to PDS4 standards documents.
    * - 12/05/24
      - System Release
      - EN
      - PDS4 system is operationally deployed and website is updated accordingly.

.. list-table:: Key Dates for Engineering Node
    :widths: 20 40 40
    :header-rows: 1

    * - Date
      - Name
      - Description
    * - 09/12/24
      - Delivery to I&T
      - The PDS4 IM and all software updated during this
        build cycle are delivered to EN I&T.
    * - 10/03/24
      - Test Readiness Review (TRR)
      - PDS EN internal review to verify readiness to enter I&T phase.
    * - 12/03/24
      - Delivery and Deployment Review (DRR)
      - PDS internal review with PDS Software Working Group to verify readiness to deploy build system.
    * - 12/05/24
      - Operational Deployment
      - PDS4 system is operationally deployed and website is updated accordingly.

For a more detailed schedule, see https://pds-engineering.jpl.nasa.gov/content/schedules.

Planned PDS4 Information Model Changes
+++++++++++++++++++++++++++++++++++++++

This section details the planned changes to the PDS4 Information Model for this build. These changes are deliverables by the PDS Data Design Working Group (DDWG) to the Engineering Node for implementation.




Planned Software Changes
++++++++++++++++++++++++

This section details the planned software changes for this build.

Planned tasks for the next release cycle are grouped by software component, and sub-tasks are included where known at the time of this plan generation. Each section also includes additional information, such as:

* Software description
* Link to |:mag:| User Guide
* Link to |:computer:| Github Repo
* Link to |:ambulance:| Issue Tracking
* Link to |:ledger:| Backlog - future work not planned for this release cycle

**Don't see the tool you are looking for?** This means there is no active development planned for this build cycle. Head to the `PDS Tool Registry <https://pds.nasa.gov/tools/tool-registry/>`_ to see all possible tools available for PDS data.

**Have a new feature or tool you think we should be working on?** Create a ticket in the applicable Github repo or in our `PDS EN Operations repo <https://github.com/NASA-PDS/pdsen-operations/issues/new/choose>`_ and we will see how that can fit into our plans moving forward.


--------

validate
########

*Validates PDS4 product labels, data and PDS3 Volumes*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/validate/>`_
     - `Github Repo <https://github.com/NASA-PDS/validate>`_
     - `Issue Tracking <https://github.com/NASA-PDS/validate/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/validate/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/validate/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/validate/releases>`_ 

* `validate#696 <https://github.com/NASA-PDS/validate/issues/696>`_ **Use New Registry API for Context Product Validation**
   * `validate#592 <https://github.com/NASA-PDS/validate/issues/592>`_ As a user, I want to when a context product has been deprecated
   * `validate#675 <https://github.com/NASA-PDS/validate/issues/675>`_ Cutover to using new Registry API for generating context products json
* `validate#832 <https://github.com/NASA-PDS/validate/issues/832>`_ **Review Handling of Special Constants and Field Formats**
   * `validate#816 <https://github.com/NASA-PDS/validate/issues/816>`_ As a user, I want a WARNING to be thrown when a delimited or character table value does not match the expected `field_format`
   * `validate#817 <https://github.com/NASA-PDS/validate/issues/817>`_ As a user, I want an ERROR to be thrown when a character table value does not match the expected `validation_format`
   * `validate#831 <https://github.com/NASA-PDS/validate/issues/831>`_ validate incorrectly handles special constant high_instrument_saturation
   * `validate#837 <https://github.com/NASA-PDS/validate/issues/837>`_ In text tables, validate attempts to match pattern associated with `data_type` before checking `Special_Constants`
   * `validate#849 <https://github.com/NASA-PDS/validate/issues/849>`_ Validate stalls when validating collection inventory file with duplicates records

--------

pds4-information-model
######################

*The software tools and data necessary for generating the Information Model including PDS4 ontology, data, and information model.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-information-model/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-information-model>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-information-model/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds4-information-model/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-information-model/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-information-model/releases>`_ 

* `pds4-information-model#701 <https://github.com/NASA-PDS/pds4-information-model/issues/701>`_ **Initial Implementation of Cucumber Framework for PDS4 IM Repo**
   * `pds4-information-model#714 <https://github.com/NASA-PDS/pds4-information-model/issues/714>`_ Initial Implementation of Cucumber Framework for LDDTool Tests
   * `pds4-information-model#715 <https://github.com/NASA-PDS/pds4-information-model/issues/715>`_ Initial Implementation of Cucumber Framework for Information Model / SCRs
* `pds4-information-model#728 <https://github.com/NASA-PDS/pds4-information-model/issues/728>`_ **B15.0 SCR Freeze**
* `pds4-information-model#729 <https://github.com/NASA-PDS/pds4-information-model/issues/729>`_ **B15.0 Standards Documents Updates**
* `pds4-information-model#730 <https://github.com/NASA-PDS/pds4-information-model/issues/730>`_ **B15.0 Information Model Delivery to I&T**
* `pds4-information-model#731 <https://github.com/NASA-PDS/pds4-information-model/issues/731>`_ **B15.0 Information Model SCR Implementation**
* `pds4-information-model#732 <https://github.com/NASA-PDS/pds4-information-model/issues/732>`_ **B15.0 Planetary Systems Target Ontology: Rings, Satellites Small Bodies Phase 1**

--------

harvest
#######

*Standalone Harvest client application providing the functionality for capturing and indexing product metadata into the PDS Registry system (https://github.com/nasa-pds/registry).*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/harvest>`_
     - `Issue Tracking <https://github.com/NASA-PDS/harvest/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/harvest/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/harvest/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/harvest/releases>`_ 

* `harvest#131 <https://github.com/NASA-PDS/harvest/issues/131>`_ **Enhance support for searching lid/lidvid references**
   * `harvest#127 <https://github.com/NASA-PDS/harvest/issues/127>`_ ref_lid_* fields are not added to the Registry schema prior to load

--------

software-issues-repo
####################

*Issue tracking repository as a centralized entry point for general PDS software bugs and feature requests.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/software-issues-repo#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/software-issues-repo>`_
     - `Issue Tracking <https://github.com/NASA-PDS/software-issues-repo/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/software-issues-repo/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/software-issues-repo/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/software-issues-repo/releases>`_ 

* `software-issues-repo#97 <https://github.com/NASA-PDS/software-issues-repo/issues/97>`_ **B15.0 Bi-Annual Triage CodeQL Static Code Analysis Scan Results**

--------

portal-wp-tasks
###############

*PDS Web Design System*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds>`_
     - `Github Repo <https://github.com/NASA-PDS/portal-wp-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/portal-wp-tasks/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/portal-wp-tasks/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/portal-wp-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/portal-wp-tasks/releases>`_ 

* `portal-wp-tasks#57 <https://github.com/NASA-PDS/portal-wp-tasks/issues/57>`_ **Phase 1: Bundle/Collection Landing Pages Modules Implementation**
* `portal-wp-tasks#58 <https://github.com/NASA-PDS/portal-wp-tasks/issues/58>`_ **Phase 1: Search Results Page Module Implementation**
* `portal-wp-tasks#60 <https://github.com/NASA-PDS/portal-wp-tasks/issues/60>`_ **Phase 1: Investigation Landing Page Module Implementation**
   * `wds-react#1 <https://github.com/NASA-PDS/wds-react/issues/1>`_ Create Hero Component
   * `wds-react#3 <https://github.com/NASA-PDS/wds-react/issues/3>`_ Create spacecraft selection component
   * `wds-react#4 <https://github.com/NASA-PDS/wds-react/issues/4>`_ Create tab bar component
   * `wds-react#13 <https://github.com/NASA-PDS/wds-react/issues/13>`_ Keep Exploring, Card Variant
   * `wds-react#14 <https://github.com/NASA-PDS/wds-react/issues/14>`_ Landing Page Hero
   * `wds-react#15 <https://github.com/NASA-PDS/wds-react/issues/15>`_ Landing Page List Content
   * `wds-react#16 <https://github.com/NASA-PDS/wds-react/issues/16>`_ Landing Page Sort Table Content
   * `wds-react#17 <https://github.com/NASA-PDS/wds-react/issues/17>`_ Landing Page Tag List Content
   * `wds-react#18 <https://github.com/NASA-PDS/wds-react/issues/18>`_ Landing Page Text Content
   * `wds-react#19 <https://github.com/NASA-PDS/wds-react/issues/19>`_ Latest News and Data Releases
   * `wds-react#20 <https://github.com/NASA-PDS/wds-react/issues/20>`_ Local Nav ("Interior Page Jump Links")
   * `wds-react#21 <https://github.com/NASA-PDS/wds-react/issues/21>`_ Recent Publications
   * `wds-react#22 <https://github.com/NASA-PDS/wds-react/issues/22>`_ Spacecraft Breaker (formerly "Quick Actions")

--------

operations
##########

*Tickets for the PDSEN Operations Team*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/operations#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/operations>`_
     - `Issue Tracking <https://github.com/NASA-PDS/operations/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/operations/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/operations/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/operations/releases>`_ 

* `operations#424 <https://github.com/NASA-PDS/operations/issues/424>`_ **Add Data Registration Validation and Deep Archive Execution to Nominal Data Release Process**

--------

planetary-data-cloud
####################

*PDS Cloud Migration documentation, issue, tracking and simple tools for assisting in the PDS hybrid cloud study and migration efforts.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/planetary-data-cloud#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/planetary-data-cloud>`_
     - `Issue Tracking <https://github.com/NASA-PDS/planetary-data-cloud/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/planetary-data-cloud/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/planetary-data-cloud/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/planetary-data-cloud/releases>`_ 

* `planetary-data-cloud#73 <https://github.com/NASA-PDS/planetary-data-cloud/issues/73>`_ **ATLAS MVP: Support Development of Initial Migration Plan and Architecture for ATLAS Survey Data**
* `planetary-data-cloud#80 <https://github.com/NASA-PDS/planetary-data-cloud/issues/80>`_ **Develop PDC Tenant Roles and Shared Responsibility Model**
* `planetary-data-cloud#100 <https://github.com/NASA-PDS/planetary-data-cloud/issues/100>`_ **Phase 2 Migration of Existing Production JPL AWS Infra to MCP**
   * `planetary-data-cloud#95 <https://github.com/NASA-PDS/planetary-data-cloud/issues/95>`_ Create baseline IAM policies for AWS resources in MCP
   * `portal-tasks#89 <https://github.com/NASA-PDS/portal-tasks/issues/89>`_ Migrate pdscloud-* instances and pds.nasa.gov on MCP
   * `planetary-data-cloud#97 <https://github.com/NASA-PDS/planetary-data-cloud/issues/97>`_ Set up appropriate policies for Dev/Test/Prod environments
   * `planetary-data-cloud#98 <https://github.com/NASA-PDS/planetary-data-cloud/issues/98>`_ Migrate data and users from JPL AWS to MCP

--------

devops
######

*Parent repo for PDS DevOps activities*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/devops#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/devops>`_
     - `Issue Tracking <https://github.com/NASA-PDS/devops/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/devops/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/devops/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/devops/releases>`_ 

* `devops#69 <https://github.com/NASA-PDS/devops/issues/69>`_ **Phase 2: Develop CI/CD for NPM/React projects**
   * `wds-react-legacy#95 <https://github.com/NASA-PDS/wds-react-legacy/issues/95>`_ Setup NPM Audits as part of CI on React projects
   * `devops#62 <https://github.com/NASA-PDS/devops/issues/62>`_ Develop Branch Testing Github Action
   * `devops#64 <https://github.com/NASA-PDS/devops/issues/64>`_ Develop Stable GitHub Action CI/CD to I&T production venue
   * `devops#65 <https://github.com/NASA-PDS/devops/issues/65>`_ Develop PR Review GitHub Action CI/CD to Developer Staging venue
   * `devops#66 <https://github.com/NASA-PDS/devops/issues/66>`_ Develop Initial Architecture and Action Flow for React CI/CD Deployments

--------

nucleus
#######

*Nucleus is a software platform used to create workflows for the Planetary Data (PDS).*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/nucleus>`_
     - `Github Repo <https://github.com/NASA-PDS/nucleus>`_
     - `Issue Tracking <https://github.com/NASA-PDS/nucleus/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/nucleus/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/nucleus/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/nucleus/releases>`_ 

* `nucleus#54 <https://github.com/NASA-PDS/nucleus/issues/54>`_ **Validate and Load all PDS4 MESSENGER data products with Nucleus**
* `nucleus#91 <https://github.com/NASA-PDS/nucleus/issues/91>`_ **Implement Warm Backup Storage Solution (Data Backup Plan)**
   * `planetary-data-cloud#75 <https://github.com/NASA-PDS/planetary-data-cloud/issues/75>`_ As a user, I want a warm backup of my archive data to be available in the event of corruption of of primary archive data
   * `nucleus#73 <https://github.com/NASA-PDS/nucleus/issues/73>`_ As a user, I want to store a copy of my archive data in AWS Deep Archive / Glacier
* `nucleus#92 <https://github.com/NASA-PDS/nucleus/issues/92>`_ **Pilot project with IMG processing using Nucleus**
* `nucleus#93 <https://github.com/NASA-PDS/nucleus/issues/93>`_ **CSS MVP: Deploy Baseline Nucleus for Catalina Sky Survey in Test and Production Environments**
   * `nucleus#73 <https://github.com/NASA-PDS/nucleus/issues/73>`_ As a user, I want to store a copy of my archive data in AWS Deep Archive / Glacier
   * `nucleus#89 <https://github.com/NASA-PDS/nucleus/issues/89>`_ Deploy Nucleus in Test env
   * `nucleus#90 <https://github.com/NASA-PDS/nucleus/issues/90>`_ Deploy Nucleus in Production env
   * `nucleus#94 <https://github.com/NASA-PDS/nucleus/issues/94>`_ Remove data from staging S3 bucket at the end of PDS basic use case
   * `nucleus#95 <https://github.com/NASA-PDS/nucleus/issues/95>`_ Remove data from EFS at the end of PDS basic use case

--------

registry
########

*PDS Registry provides service and software application necessary for tracking, searching, auditing, locating, and maintaining artifacts within the system. These artifacts can range from data files and label files, schemas, dictionary definitions for objects and elements, services, etc.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/registry>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/registry/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry/releases>`_ 

* `registry#181 <https://github.com/NASA-PDS/registry/issues/181>`_ **Support Registration and Search of Products Replicated Across Archives**
   * `registry-api#306 <https://github.com/NASA-PDS/registry-api/issues/306>`_ If >1 products with the same LIDVID are registered by different nodes, we should respond with one of them
   * `registry#245 <https://github.com/NASA-PDS/registry/issues/245>`_ As a user, I want to register data product(s) that is mirrored across 2 or more organizations
* `registry#230 <https://github.com/NASA-PDS/registry/issues/230>`_ **Enable Support for Changing Field Types**
* `registry#266 <https://github.com/NASA-PDS/registry/issues/266>`_ **Implement design for alternate data file paths**
   * `registry#86 <https://github.com/NASA-PDS/registry/issues/86>`_ As a user, I want to harvest and register alternate data file paths
   * `registry#96 <https://github.com/NASA-PDS/registry/issues/96>`_ As a user I want to change the file paths of products in the registry
   * `harvest#123 <https://github.com/NASA-PDS/harvest/issues/123>`_ As a Node Operator, I want to specify an alternate file paths for 1 or more archive products
   * `registry-mgr#76 <https://github.com/NASA-PDS/registry-mgr/issues/76>`_ As a user, I want to manually update a product's file location (file_ref)

--------

registry-api
############

*Web API service for the PDS Registry, providing the implementation of the PDS Search API (https://github.com/nasa-pds/pds-api) for the PDS Registry.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-api/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/registry-api/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-api/releases>`_ 

* `registry-api#285 <https://github.com/NASA-PDS/registry-api/issues/285>`_ **Implement Faceting**
   * `registry-api#283 <https://github.com/NASA-PDS/registry-api/issues/283>`_ As a client developer, I want to facet on 1 or more fields in the registry
   * `registry-api#284 <https://github.com/NASA-PDS/registry-api/issues/284>`_ As an API user, I want to know the unique values for a specific API field.
   * `registry-api#323 <https://github.com/NASA-PDS/registry-api/issues/323>`_ As a user, I want the /properties endpoint to display counts for products having each property
   * `registry-api#324 <https://github.com/NASA-PDS/registry-api/issues/324>`_ As a user, I want the /properties endpoint to display range/enum type and values for each property
   * `registry-api#325 <https://github.com/NASA-PDS/registry-api/issues/325>`_ As a user, I want the /properties endpoint to include a link to explanatory documentation (i.e. DD or similar)

--------

data-upload-manager
###################

*Data Upload Manager (DUM) component for managing the interface for data uploads to the Planetary Data Cloud from Data Providers and PDS Nodes.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/data-upload-manager>`_
     - `Github Repo <https://github.com/NASA-PDS/data-upload-manager>`_
     - `Issue Tracking <https://github.com/NASA-PDS/data-upload-manager/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/data-upload-manager/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/data-upload-manager/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/data-upload-manager/releases>`_ 

* `data-upload-manager#51 <https://github.com/NASA-PDS/data-upload-manager/issues/51>`_ **Add User-Defined Object Metadata**
   * `data-upload-manager#50 <https://github.com/NASA-PDS/data-upload-manager/issues/50>`_ As a user, I want to include a MD5 checksum in the the user-defined object metadata being sent in the upload payload
   * `data-upload-manager#87 <https://github.com/NASA-PDS/data-upload-manager/issues/87>`_ As a user, I want to include the modification datetime in the the user-defined object metadata being sent in the upload payload


Other Information
+++++++++++++++++

Reference Documents
###################

This section details the controlling and applicable documents referenced for this release. The controlling documents are as follows:

* PDS Level 1, 2 and 3 Requirements, April 20, 2017.
* PDS4 Project Plan, July 17, 2013.
* PDS4 System Architecture Specification, Version 1.3, September 1, 2013.
* PDS4 Operations Concept, Version 1.0, September 1, 2013.
* PDS General System Software Requirements Document (SRD), Version 1.1, September 1, 2013.
* PDS Harvest Tool Software Requirements and Design Document (SRD/SDD), Version 1.2, September 1, 2013.
* PDS Preparation Tools Software Requirements and Design Document (SRD/SDD), Version 0.3, September 1, 2013.
* PDS Registry Service Software Requirements and Design Document (SRD/SDD), Version 1.1, September 1, 2013.
* PDS Report Service Software Requirements and Design Document (SRD/SDD), Version 1.1, September 1, 2013.
* PDS Search Service Software Requirements and Design Document (SRD/SDD), Version 1.0, September 1, 2013.
   * PDS Search Scenarios, Version 1.0, September 1, 2013.
   * PDS Search Protocol, Version 1.2, March 21, 2014.
   * PDAP Search Protocol, Version 1.0, March 21, 2014.
* PDS Security Service Software Requirements and Design Document (SRD/SDD), Version 1.1, September 1, 2013.
* PDS NSSDC Delivery Software Requirements and Design Document (SRD/SDD), Version 0.1, October 29, 2019.


System Requirements, Dependencies, and Assumptions
##################################################

See individual applications for specific dependencies and system requirements.
