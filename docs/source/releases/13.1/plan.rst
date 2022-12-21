Build 13.1 Plan
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
    * - 03/02/2022
      - SCR Freeze Date
      - DDWG
      - Freeze date for identifying SCRs to be implemented in this release.
    * - 04/06/2023
      - Standards Documents Updates Due
      - Document Authoring Team
      - Updates to PDS4 standards documents due to EN for review.
    * - 04/18/2023 - 05/16/2023
      - Beta Testing Period
      - DNs, IPDA
      - Changes to PDS4 IM and system components available for beta testing.
    * - 04/18/2023 - 05/16/2023
      - dLDD Integration and Test
      - dLDD Stewards
      - Auto-generated dLDDs should be reviews by dLDD Stewards, and final updates to dLDDs should be completed during this time.
    * - 05/08/2023
      - Standards Documents Review Due
      - Document Review Team
      - Review updates to PDS4 standards documents.
    * - 06/02/2023
      - System Release
      - EN
      - PDS4 system is operationally deployed and website is updated accordingly.

.. list-table:: Key Dates for Engineering Node
    :widths: 20 40 40
    :header-rows: 1

    * - Date
      - Name
      - Description
    * - 03/21/2023
      - Delivery to I&T
      - The PDS4 IM and all software updated during this 
        build cycle are delivered to EN I&T.
    * - 04/03/2023
      - Test Readiness Review (TRR)
      - PDS EN internal review to verify readiness to enter I&T phase.
    * - 05/22/2023
      - Delivery and Deployment Review (DRR)
      - PDS internal review with PDS Software Working Group to verify readiness to deploy build system.
    * - 06/02/2023
      - Operational Deployment
      - PDS4 system is operationally deployed and website is updated accordingly.

For a more detailed schedule, see https://pds-engineering.jpl.nasa.gov/content/schedules.

Planned PDS4 Information Model Changes
+++++++++++++++++++++++++++++++++++++++

This section details the planned changes to the PDS4 Information Model for this build. These changes are deliverables by the PDS Data Design Working Group (DDWG) to the Engineering Node for implementation.

* `pds4-information-model#499 <https://github.com/NASA-PDS/pds4-information-model/issues/499>`_ **CCB-348: Add Units_of_Mass_Density as a unit of measure**
* `pds4-information-model#547 <https://github.com/NASA-PDS/pds4-information-model/issues/547>`_ **B13.1 Updates per CCB-Approved SCRs**



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
     - `Backlog <https://github.com/NASA-PDS/validate/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/validate/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/validate/releases>`_ 

* `validate#414 <https://github.com/NASA-PDS/validate/issues/414>`_ **Referential Integrity Checking with the Registry**
   * `validate#415 <https://github.com/NASA-PDS/validate/issues/415>`_ As a user, I want to perform referential integrity checking against a registry
   * `validate#462 <https://github.com/NASA-PDS/validate/issues/462>`_ As a user, I want validate to throw an error when the LID specified for secondary context product in a collection inventory is not valid
* `validate#498 <https://github.com/NASA-PDS/validate/issues/498>`_ **Improve Content Validation Performance through Spot Checking**
   * `validate#1 <https://github.com/NASA-PDS/validate/issues/1>`_ As a user, I want to execute content validation against every nth file
* `validate#534 <https://github.com/NASA-PDS/validate/issues/534>`_ **B13.1 Content Validation Improvements: Additional Table Types, Additional File Areas**
   * `validate#217 <https://github.com/NASA-PDS/validate/issues/217>`_ As a user, I want to validate content for all possible PDS4 table types
   * `validate#436 <https://github.com/NASA-PDS/validate/issues/436>`_ Improve error messages for overlapping objects in a label
   * `validate#480 <https://github.com/NASA-PDS/validate/issues/480>`_ Validate does not calculate overlaps correctly when Header is not first object in file
* `validate#557 <https://github.com/NASA-PDS/validate/issues/557>`_ **Dockerize Validate**
   * `validate#556 <https://github.com/NASA-PDS/validate/issues/556>`_ As a user, I want to be able to use validate from a docker container
* `validate#578 <https://github.com/NASA-PDS/validate/issues/578>`_ **B13.1 Fix Must-Have Priority Bugs**
   * `validate#444 <https://github.com/NASA-PDS/validate/issues/444>`_ pds4.bundle option seems to not travel through enough subdirectories
   * `validate#453 <https://github.com/NASA-PDS/validate/issues/453>`_ Validate should not check PDF/A validity if content validation is disabled
   * `validate#474 <https://github.com/NASA-PDS/validate/issues/474>`_ Validate can't find files in directory specified by <directory_path_name>
   * `validate#499 <https://github.com/NASA-PDS/validate/issues/499>`_ validate doesn't flag a data file with only LF
   * `validate#503 <https://github.com/NASA-PDS/validate/issues/503>`_ validate passes confusing message to the command window
   * `validate#511 <https://github.com/NASA-PDS/validate/issues/511>`_ Table_Character not accurately checking field formats
   * `validate#519 <https://github.com/NASA-PDS/validate/issues/519>`_ Validate should throw record length error when record delimiter does not occur in correct location
   * `validate#529 <https://github.com/NASA-PDS/validate/issues/529>`_  ERROR  [error.array.value_out_of_min_max_range] evaluation is not correct
   * `validate#531 <https://github.com/NASA-PDS/validate/issues/531>`_ ERROR  [error.table.bad_file_read] incorrectly reports that GroupFieldBinary group_length is larger than size of contained fields
   * `validate#544 <https://github.com/NASA-PDS/validate/issues/544>`_ validate gives a error.table.bad_field_read error
   * `validate#554 <https://github.com/NASA-PDS/validate/issues/554>`_ --spot-check-data flag throws IOException
   * `validate#564 <https://github.com/NASA-PDS/validate/issues/564>`_ Array object validation regression in v3.0.3
   * `validate#576 <https://github.com/NASA-PDS/validate/issues/576>`_ validate does not correctly handle field format checks for hex values

--------

pds4-information-model
######################

*The software tools and data necessary for generating the Information Model including PDS4 ontology, data, and information model.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-information-model/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-information-model>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-information-model/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds4-information-model/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-information-model/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-information-model/releases>`_ 

* `pds4-information-model#513 <https://github.com/NASA-PDS/pds4-information-model/issues/513>`_ **B13.1 Update LDDTool to support IM Version 1.19.0.0**
* `pds4-information-model#544 <https://github.com/NASA-PDS/pds4-information-model/issues/544>`_ **Test and Validate Term Mapping Implementation**
   * `pds4-information-model#545 <https://github.com/NASA-PDS/pds4-information-model/issues/545>`_ Implement Term Mapping Example for EPNCore Attributes
* `pds4-information-model#546 <https://github.com/NASA-PDS/pds4-information-model/issues/546>`_ **B13.1 Continue Refactoring the IMTool/LDDTool Code**
* `pds4-information-model#549 <https://github.com/NASA-PDS/pds4-information-model/issues/549>`_ **B13.1 Initial Support for Target Ontology Project**

--------

pds-api
#######

*PDS web APIs specifications and user's manual*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-api/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api/releases>`_ 

* `pds-api#181 <https://github.com/NASA-PDS/pds-api/issues/181>`_ **Search Improvements to Support Web Modernization**
   * `pds-api#104 <https://github.com/NASA-PDS/pds-api/issues/104>`_ Improvements to Keyword Search for Weighting and Suggested Searches
   * `pds-api#165 <https://github.com/NASA-PDS/pds-api/issues/165>`_ As a user, I want to search for PDS software tools and services
* `pds-api#182 <https://github.com/NASA-PDS/pds-api/issues/182>`_ **Implement Faceting**
   * `pds-api#70 <https://github.com/NASA-PDS/pds-api/issues/70>`_ As an API user, I want to know the unique values for a specific API field.
   * `pds-api#103 <https://github.com/NASA-PDS/pds-api/issues/103>`_ As a client developer, I want to facet on 1 or more fields in the registry
* `pds-api#230 <https://github.com/NASA-PDS/pds-api/issues/230>`_ **Support latest product search from API**
   * `pds-api#220 <https://github.com/NASA-PDS/pds-api/issues/220>`_ Past versions are being returned by API, by default
   * `pds-api#221 <https://github.com/NASA-PDS/pds-api/issues/221>`_ As a user, I want to query only the latest versions of products unless explicitly requested
   * `pds-api#236 <https://github.com/NASA-PDS/pds-api/issues/236>`_ Make the registry-api use the new latest index
   * `registry#140 <https://github.com/NASA-PDS/registry/issues/140>`_ Integrate new `provence.py` script into integration tests to tag products with Provenance information
   * `registry#141 <https://github.com/NASA-PDS/registry/issues/141>`_ Integrate new `provence.py` script into operational deployment to tag products with Provenance information
* `pds-api#235 <https://github.com/NASA-PDS/pds-api/issues/235>`_ **Enable Swagger Interface on pds.nasa.gov**
   * `pds-api#193 <https://github.com/NASA-PDS/pds-api/issues/193>`_ As a user, I want to be able to access the Search API Swagger interface from pds.nasa.gov
   * `pds-api#239 <https://github.com/NASA-PDS/pds-api/issues/239>`_ As a user, I want to get application/json response format by default if I request an API url in my browser
* `pds-api#237 <https://github.com/NASA-PDS/pds-api/issues/237>`_ **Support Searching for Past Versions of Products with Differing LIDs**
   * `pds-api#148 <https://github.com/NASA-PDS/pds-api/issues/148>`_ As a user, I want to search for past versions of a product where the LID changed during the product history

--------

wds-implementation
##################

*PDS Web Design System*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds>`_
     - `Github Repo <https://github.com/NASA-PDS/wds-implementation>`_
     - `Issue Tracking <https://github.com/NASA-PDS/wds-implementation/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/wds-implementation/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/wds-implementation/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/wds-implementation/releases>`_ 

* `wds-implementation#22 <https://github.com/NASA-PDS/wds-implementation/issues/22>`_ **Initial Data Search Journey Prototype**
   * `wds-implementation#23 <https://github.com/NASA-PDS/wds-implementation/issues/23>`_ Show Search Results With PDS Styles
   * `wds-implementation#24 <https://github.com/NASA-PDS/wds-implementation/issues/24>`_ Add Routing For Searches
   * `wds-implementation#25 <https://github.com/NASA-PDS/wds-implementation/issues/25>`_ Show Search Results From API
   * `wds-implementation#26 <https://github.com/NASA-PDS/wds-implementation/issues/26>`_ Integrate Search Results Feedback

--------

design-team
###########

*PDS.nasa.gov User Experience Task Issue and Prototype repository*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/design-team#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/design-team>`_
     - `Issue Tracking <https://github.com/NASA-PDS/design-team/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/design-team/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/design-team/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/design-team/releases>`_ 

* `design-team#161 <https://github.com/NASA-PDS/design-team/issues/161>`_ **B13.1 User Journey Figma Prototyping: Homepage & Search**

--------

cloud-tasks
###########

*PDS Cloud Migration documentation, issue, tracking and simple tools for assisting in the PDS hybrid cloud study and migration efforts.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/cloud-tasks#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/cloud-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/cloud-tasks/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/cloud-tasks/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/cloud-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/cloud-tasks/releases>`_ 

* `cloud-tasks#24 <https://github.com/NASA-PDS/cloud-tasks/issues/24>`_ **Re-imagine and Implement New Registry Architecture in AWS**
   * `cloud-tasks#36 <https://github.com/NASA-PDS/cloud-tasks/issues/36>`_ document the AWS infrastructure used by PDS
   * `cloud-tasks#51 <https://github.com/NASA-PDS/cloud-tasks/issues/51>`_ Create POC for registry multi-tenancy
   * `registry#133 <https://github.com/NASA-PDS/registry/issues/133>`_ Update Registry Loader Tools To Support New Registry Cloud Architecture
* `cloud-tasks#35 <https://github.com/NASA-PDS/cloud-tasks/issues/35>`_ **NGAP Pilot: Deploy Registries**
   * `cloud-tasks#40 <https://github.com/NASA-PDS/cloud-tasks/issues/40>`_ NGAP Onboarding
* `cloud-tasks#57 <https://github.com/NASA-PDS/cloud-tasks/issues/57>`_ **Prototype and Adapt ESDIS Thin Egresss App (TEA) for PDS**
   * `cloud-tasks#58 <https://github.com/NASA-PDS/cloud-tasks/issues/58>`_ Initial investigation of TEA and how/if it can be adapted for the PDS
* `cloud-tasks#60 <https://github.com/NASA-PDS/cloud-tasks/issues/60>`_ **Develop PDS Cloud Cost Model**

--------

planetarydata.org
#################

*Website and related services for the International Planetary Data Alliance, nominally run at https://planetarydata.org/*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/planetarydata.org#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/planetarydata.org>`_
     - `Issue Tracking <https://github.com/NASA-PDS/planetarydata.org/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/planetarydata.org/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/planetarydata.org/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/planetarydata.org/releases>`_ 

* `planetarydata.org#7 <https://github.com/NASA-PDS/planetarydata.org/issues/7>`_ **Migrate planetarydata.org to WordPress in AWS**
   * `planetarydata.org#8 <https://github.com/NASA-PDS/planetarydata.org/issues/8>`_ Deploy WordPress in an EC2 instance in JPL Cloud
   * `planetarydata.org#9 <https://github.com/NASA-PDS/planetarydata.org/issues/9>`_ Migrate existing content from Plone to Wordpress
   * `planetarydata.org#10 <https://github.com/NASA-PDS/planetarydata.org/issues/10>`_ Design / select skin for the new website
   * `planetarydata.org#11 <https://github.com/NASA-PDS/planetarydata.org/issues/11>`_ Complete review of website with IPDA Website Update team
   * `planetarydata.org#12 <https://github.com/NASA-PDS/planetarydata.org/issues/12>`_ Submit URS request for review of website for DNS switch
   * `planetarydata.org#13 <https://github.com/NASA-PDS/planetarydata.org/issues/13>`_ Finalize website migration with DNS switch 

--------

nucleus
#######

*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/nucleus#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/nucleus>`_
     - `Issue Tracking <https://github.com/NASA-PDS/nucleus/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/nucleus/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/nucleus/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/nucleus/releases>`_ 

* `nucleus#2 <https://github.com/NASA-PDS/nucleus/issues/2>`_ **Initial Implementation and Operationalize Nucleus**
* `nucleus#14 <https://github.com/NASA-PDS/nucleus/issues/14>`_ **B13.1 Technology Selection and Internal Review**
   * `nucleus#11 <https://github.com/NASA-PDS/nucleus/issues/11>`_ Proof-of-concept with Apache Airflow
   * `nucleus#13 <https://github.com/NASA-PDS/nucleus/issues/13>`_ Proof of concept with Cumulus on NGAP
   * `nucleus#15 <https://github.com/NASA-PDS/nucleus/issues/15>`_ Proof of concept for Nucleus in CWS
   * `nucleus#19 <https://github.com/NASA-PDS/nucleus/issues/19>`_ Complete JPL Internal Peer Review of Trade Study and Technology Selection
* `nucleus#16 <https://github.com/NASA-PDS/nucleus/issues/16>`_ **Develop Cost Model**
* `nucleus#17 <https://github.com/NASA-PDS/nucleus/issues/17>`_ **Pilot Nucleus with SBN-PSI Catalina Sky Survey Pipeline**
* `nucleus#18 <https://github.com/NASA-PDS/nucleus/issues/18>`_ **Develop Detailed Technical Architecture**

--------

registry
########

*PDS Registry provides service and software application necessary for tracking, searching, auditing, locating, and maintaining artifacts within the system. These artifacts can range from data files and label files, schemas, dictionary definitions for objects and elements, services, etc.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/registry>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/registry/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry/releases>`_ 

* `registry#85 <https://github.com/NASA-PDS/registry/issues/85>`_ **Enhance Registry Delete Functionality**
   * `registry-mgr#52 <https://github.com/NASA-PDS/registry-mgr/issues/52>`_ As a user I want to delete whole bundles at once
* `registry#99 <https://github.com/NASA-PDS/registry/issues/99>`_ **Populate EN Registry with PDS3 Data Sets**
   * `registry#62 <https://github.com/NASA-PDS/registry/issues/62>`_ As a user, I want to ingest legacy PDS3 data sets from EN legacy registry
   * `registry#63 <https://github.com/NASA-PDS/registry/issues/63>`_ Deploy harvest / registry-mgr as cron to regularly upload PDS EN data to registry
   * `operations#270 <https://github.com/NASA-PDS/operations/issues/270>`_ Deployment of Registry Loader Tools and Initial Ingestion of Engineering Node Registry on Latest AWS Deployment
* `registry#134 <https://github.com/NASA-PDS/registry/issues/134>`_ **Enhanced Query Support through Registry Tools**
   * `registry#100 <https://github.com/NASA-PDS/registry/issues/100>`_ Update documentation to include explicit example of how to query staged data
   * `registry-mgr#59 <https://github.com/NASA-PDS/registry-mgr/issues/59>`_ As a user, I want to query OpenSearch for staged data via a CLI command 


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