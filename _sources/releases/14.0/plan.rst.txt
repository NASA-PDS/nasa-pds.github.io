Build 14.0 Plan
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
    * - 08/14/2023
      - SCR Freeze Date
      - DDWG
      - Freeze date for identifying SCRs to be implemented in this release.
    * - 08/15/2023 - 09/16/2023
      - Standards Documents Updates Due
      - Document Authoring Team
      - Updates to PDS4 standards documents due to EN for review.
    * - 10/17/2023 - 11/07/2023
      - Beta Testing Period
      - DNs, IPDA
      - Changes to PDS4 IM and system components available for beta testing.
    * - 10/17/2023 - 11/07/2023
      - dLDD Integration and Test
      - dLDD Stewards
      - Auto-generated dLDDs should be reviews by dLDD Stewards, and final updates to dLDDs should be completed during this time.
    * - 09/28/2023 - 10/26/2023
      - Standards Documents Review Due
      - Document Review Team
      - Review updates to PDS4 standards documents.
    * - 12/01/2023
      - System Release
      - EN
      - PDS4 system is operationally deployed and website is updated accordingly.

.. list-table:: Key Dates for Engineering Node
    :widths: 20 40 40
    :header-rows: 1

    * - Date
      - Name
      - Description
    * - 09/12/2023
      - Delivery to I&T
      - The PDS4 IM and all software updated during this 
        build cycle are delivered to EN I&T.
    * - 09/25/2023
      - Test Readiness Review (TRR)
      - PDS EN internal review to verify readiness to enter I&T phase.
    * - 11/20/2023
      - Delivery and Deployment Review (DRR)
      - PDS internal review with PDS Software Working Group to verify readiness to deploy build system.
    * - 12/01/2023
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

* `validate#534 <https://github.com/NASA-PDS/validate/issues/534>`_ **B14.0 Content Validation Improvements: Additional Table Types, Additional File Areas**
   * `validate#7 <https://github.com/NASA-PDS/validate/issues/7>`_ Update to support ComplexLSB8 data types and investigate Floating point exception
   * `validate#190 <https://github.com/NASA-PDS/validate/issues/190>`_ Validation fails to catch real value in ASCII_NonNegative_Integer field (Table_Delimited)
   * `validate#211 <https://github.com/NASA-PDS/validate/issues/211>`_ Update validate with additional data type support for image transformations
   * `validate#217 <https://github.com/NASA-PDS/validate/issues/217>`_ As a user, I want to validate content for all possible PDS4 table types
   * `validate#343 <https://github.com/NASA-PDS/validate/issues/343>`_ As a user I want to see the name of a table/array in errors, if one is specified
   * `validate#431 <https://github.com/NASA-PDS/validate/issues/431>`_ warning.table.characters_between_fields missing for last record in table
   * `validate#436 <https://github.com/NASA-PDS/validate/issues/436>`_ Improve error messages for overlapping objects in a label
   * `validate#476 <https://github.com/NASA-PDS/validate/issues/476>`_ Check for duplicate LIDVIDs in collection inventory
   * `validate#480 <https://github.com/NASA-PDS/validate/issues/480>`_ Validate does not calculate overlaps correctly when Header is not first object in file
   * `validate#508 <https://github.com/NASA-PDS/validate/issues/508>`_ CRLF/LF checks do not seem to be working as expected for Table_Character
* `validate#606 <https://github.com/NASA-PDS/validate/issues/606>`_ **Support for Encoded Video and Encoded Audio**
   * `validate#604 <https://github.com/NASA-PDS/validate/issues/604>`_ As a user, I want to validate MP4/H.264 encoded video as observational data
   * `validate#605 <https://github.com/NASA-PDS/validate/issues/605>`_ As a user, I want to validate MP4/H.264/AAC encoded audio as observational data
* `validate#607 <https://github.com/NASA-PDS/validate/issues/607>`_ **Support for Improved Datetime Checks**
   * `validate#520 <https://github.com/NASA-PDS/validate/issues/520>`_ Refactor regex handling to use Google's RE2J library and compile
   * `validate#608 <https://github.com/NASA-PDS/validate/issues/608>`_ Update datetime regex for content validation
* `validate#610 <https://github.com/NASA-PDS/validate/issues/610>`_ **B14.0 Enhancements to Initial Version of Registry Referential Integrity Validator**
   * `validate#619 <https://github.com/NASA-PDS/validate/issues/619>`_ Improve new referential integrity checker timeout tolerance
   * `validate#620 <https://github.com/NASA-PDS/validate/issues/620>`_ verbosity flag does not appear to output INFO messages
   * `validate#622 <https://github.com/NASA-PDS/validate/issues/622>`_ Update to use non-zero exit code if any ERROR in execution
   * `validate#643 <https://github.com/NASA-PDS/validate/issues/643>`_ Document how to use validate-refs tool in Validate Operation User Guide
* `validate#629 <https://github.com/NASA-PDS/validate/issues/629>`_ **Add Check for Schematron/Schema Version Mismatch**
   * `validate#628 <https://github.com/NASA-PDS/validate/issues/628>`_ As a user, I want to throw a WARNING when a product's schematron version does not match the schema version

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

* `pds4-information-model#627 <https://github.com/NASA-PDS/pds4-information-model/issues/627>`_ **Support LBLX label file extension**
   * `pds4-information-model#554 <https://github.com/NASA-PDS/pds4-information-model/issues/554>`_ As a user, I want to output a dictionary label with the .lblx extension.
* `pds4-information-model#635 <https://github.com/NASA-PDS/pds4-information-model/issues/635>`_ **B14.0 Develop Planetary Systems Target Ontology**
   * `pds4-information-model#634 <https://github.com/NASA-PDS/pds4-information-model/issues/634>`_ Iterate and improve planetary systems target ontology
* `pds4-information-model#652 <https://github.com/NASA-PDS/pds4-information-model/issues/652>`_ **B14.0 LDDTool/IMTool Code Refactoring**
   * `pds4-information-model#651 <https://github.com/NASA-PDS/pds4-information-model/issues/651>`_ Add TermMaps to default output JSON

--------

pds-github-util
###############

*github utility functions to enforce the PDS engineering node software life cycle.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-github-util>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-github-util>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-github-util/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-github-util/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-github-util/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-github-util/releases>`_ 

* `pds-github-util#72 <https://github.com/NASA-PDS/pds-github-util/issues/72>`_ **Refactor github-util Into Smaller Subpackages**
   * `pds-github-util#73 <https://github.com/NASA-PDS/pds-github-util/issues/73>`_ Define the pds-github-util subpackages

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

* `software-issues-repo#63 <https://github.com/NASA-PDS/software-issues-repo/issues/63>`_ **B14.0 Release Planning**

--------

pds-api
#######

*PDS web APIs specifications and user's manual*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-api/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api/releases>`_ 

* `pds-api#237 <https://github.com/NASA-PDS/pds-api/issues/237>`_ **Support Searching for Past Versions of Products with Differing LIDs**
   * `pds-api#148 <https://github.com/NASA-PDS/pds-api/issues/148>`_ As a user, I want to search for past versions of a product where the LID changed during the product history
* `pds-api#255 <https://github.com/NASA-PDS/pds-api/issues/255>`_ **Enable Authorized Access to Restricted Data**

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

* `operations#379 <https://github.com/NASA-PDS/operations/issues/379>`_ **Phase 2: Wordpress migration for pds-engineering website**
   * `operations#338 <https://github.com/NASA-PDS/operations/issues/338>`_ Request last re-sync of most recent files then verify
   * `operations#339 <https://github.com/NASA-PDS/operations/issues/339>`_ Test redirects
   * `operations#343 <https://github.com/NASA-PDS/operations/issues/343>`_ Install Feedback widget in WordPress PDS Engineering site
   * `operations#362 <https://github.com/NASA-PDS/operations/issues/362>`_ update information file for Metrics' Multi-Selection Visualization Chart
   * `operations#391 <https://github.com/NASA-PDS/operations/issues/391>`_ Migrate and verify latest content for PDS Eng WP
   * `operations#392 <https://github.com/NASA-PDS/operations/issues/392>`_ Incorporate JPL logo into header for PDS Eng WP

--------

doi-ui
######

*The web interface for the PDS DOI Service providing the ability management PDS archive DOIs. See the DOI Service for more details on the available capabilities. https://nasa-pds.github.io/doi-service/*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/doi-ui#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/doi-ui>`_
     - `Issue Tracking <https://github.com/NASA-PDS/doi-ui/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/doi-ui/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/doi-ui/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/doi-ui/releases>`_ 

* `doi-ui#184 <https://github.com/NASA-PDS/doi-ui/issues/184>`_ **Develop DOI Service User Guide and Training**

--------

cloud-tasks
###########

*PDS Cloud Migration documentation, issue, tracking and simple tools for assisting in the PDS hybrid cloud study and migration efforts.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/cloud-tasks#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/cloud-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/cloud-tasks/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/cloud-tasks/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/cloud-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/cloud-tasks/releases>`_ 

* `cloud-tasks#29 <https://github.com/NASA-PDS/cloud-tasks/issues/29>`_ **Migrate Web Analytics prototype to PDS Cloud**
   * `cloud-tasks#30 <https://github.com/NASA-PDS/cloud-tasks/issues/30>`_ Work with Web Unification team to define system architecture for migration
   * `web-analytics#2 <https://github.com/NASA-PDS/web-analytics/issues/2>`_ As a data engineer, I want to sync logs from PDS website in an automated fashion
   * `web-analytics#3 <https://github.com/NASA-PDS/web-analytics/issues/3>`_ Migrate PDS Web Analytics dashboards in PDS-managed AWS environment
* `cloud-tasks#35 <https://github.com/NASA-PDS/cloud-tasks/issues/35>`_ **MCP Pilot: Deploy Registry**
* `cloud-tasks#61 <https://github.com/NASA-PDS/cloud-tasks/issues/61>`_ **Design and Implement Initial File System Viewer**
* `cloud-tasks#64 <https://github.com/NASA-PDS/cloud-tasks/issues/64>`_ **MCP Pilot: Deploy Nucleus**
* `cloud-tasks#65 <https://github.com/NASA-PDS/cloud-tasks/issues/65>`_ **Initial NGAP-to-MCP Migration Research**

--------

planetarydata.org
#################

*Website and related services for the International Planetary Data Alliance, nominally run at https://planetarydata.org/*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/planetarydata.org#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/planetarydata.org>`_
     - `Issue Tracking <https://github.com/NASA-PDS/planetarydata.org/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/planetarydata.org/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/planetarydata.org/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/planetarydata.org/releases>`_ 

* `planetarydata.org#7 <https://github.com/NASA-PDS/planetarydata.org/issues/7>`_ **Operational Deployment of new planetarydata.org WordPress site**
   * `planetarydata.org#8 <https://github.com/NASA-PDS/planetarydata.org/issues/8>`_ Deploy WordPress in an EC2 instance in JPL Cloud
   * `planetarydata.org#9 <https://github.com/NASA-PDS/planetarydata.org/issues/9>`_ Migrate existing content from Plone to Wordpress
   * `planetarydata.org#10 <https://github.com/NASA-PDS/planetarydata.org/issues/10>`_ Design / select skin for the new website
   * `planetarydata.org#11 <https://github.com/NASA-PDS/planetarydata.org/issues/11>`_ Complete review of website with IPDA Website Update team
   * `planetarydata.org#12 <https://github.com/NASA-PDS/planetarydata.org/issues/12>`_ Complete URS request for review of website for DNS switch
   * `planetarydata.org#13 <https://github.com/NASA-PDS/planetarydata.org/issues/13>`_ Finalize website migration with DNS switch 
   * `planetarydata.org#15 <https://github.com/NASA-PDS/planetarydata.org/issues/15>`_ Iterate on new planetarydata.org updates per feedback
   * `planetarydata.org#16 <https://github.com/NASA-PDS/planetarydata.org/issues/16>`_ planetarydata.org accessibility scan part 2
   * `planetarydata.org#18 <https://github.com/NASA-PDS/planetarydata.org/issues/18>`_ Enable public access to Wordpress site for external review

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

* `devops#37 <https://github.com/NASA-PDS/devops/issues/37>`_ **Automatically deploy an up to date I&T platform where all software can be tested**
   * `devops#36 <https://github.com/NASA-PDS/devops/issues/36>`_ For registry components, add a github action which runs the integration test when something is pushed on a dev branch
   * `registry-sweepers#6 <https://github.com/NASA-PDS/registry-sweepers/issues/6>`_ Create the docker image and push it to docker hub as part of the CICD
   * `devops#41 <https://github.com/NASA-PDS/devops/issues/41>`_ Push docker image on AWS ECR in github-actions, in addition to docker hub
   * `devops#44 <https://github.com/NASA-PDS/devops/issues/44>`_ Ask new Application developer profile on JPL AWS
   * `devops#45 <https://github.com/NASA-PDS/devops/issues/45>`_ Have a github action self-hosted runner on NGAP
   * `devops#46 <https://github.com/NASA-PDS/devops/issues/46>`_ Fully terraform the registry application

--------

nucleus
#######

*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/nucleus#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/nucleus>`_
     - `Issue Tracking <https://github.com/NASA-PDS/nucleus/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/nucleus/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/nucleus/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/nucleus/releases>`_ 

* `nucleus#17 <https://github.com/NASA-PDS/nucleus/issues/17>`_ **Deploy Baseline Nucleus for SBN-PSI Catalina Sky Survey Pilot**
* `nucleus#38 <https://github.com/NASA-PDS/nucleus/issues/38>`_ **Develop Logging and Monitoring Strategy**
* `nucleus#41 <https://github.com/NASA-PDS/nucleus/issues/41>`_ **Determine DAG definition standard**

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

* `registry#47 <https://github.com/NASA-PDS/registry/issues/47>`_ **Support LBLX extension in Registry Loader tools**
* `registry#99 <https://github.com/NASA-PDS/registry/issues/99>`_ **Populate EN Registry with PDS3 Data Sets**
   * `registry#62 <https://github.com/NASA-PDS/registry/issues/62>`_ As a user, I want to ingest legacy PDS3 data sets from EN legacy registry
   * `registry#63 <https://github.com/NASA-PDS/registry/issues/63>`_ Deploy harvest / registry-mgr as cron to regularly upload PDS EN data to registry
   * `operations#270 <https://github.com/NASA-PDS/operations/issues/270>`_ Deployment of Registry Loader Tools and Initial Ingestion of Engineering Node Registry on Latest AWS Deployment
   * `registry#168 <https://github.com/NASA-PDS/registry/issues/168>`_ As a manager, I want to see the progress of data sets ingested into registry vs. legacy registry
* `registry#178 <https://github.com/NASA-PDS/registry/issues/178>`_ **Improved Fault Tolerance for Registry and Registry API**
   * `registry-common#26 <https://github.com/NASA-PDS/registry-common/issues/26>`_ [SECURITY] Fix code scanning alert - `TrustManager` that accepts all certificates
   * `registry-api#292 <https://github.com/NASA-PDS/registry-api/issues/292>`_ Queries for data products with lots of metadata attributes crash in browser
   * `registry-api#297 <https://github.com/NASA-PDS/registry-api/issues/297>`_ As a EN Operator, I want to the registry API to be fault tolerant
   * `registry#176 <https://github.com/NASA-PDS/registry/issues/176>`_ As a EN Operator, I want to the registry to be fault tolerant
   * `registry-api#300 <https://github.com/NASA-PDS/registry-api/issues/300>`_ Update Java params and Docker image to expand JVM memory beyond 50%
   * `harvest#119 <https://github.com/NASA-PDS/harvest/issues/119>`_ As a developer, I want to know what version of Harvest was used to load a product
* `registry#181 <https://github.com/NASA-PDS/registry/issues/181>`_ **Support Registration and Search of Products Replicated Across Archives**
   * `registry#93 <https://github.com/NASA-PDS/registry/issues/93>`_ As a user, I want to be able to ingest mirrored archive data
   * `registry-api#306 <https://github.com/NASA-PDS/registry-api/issues/306>`_ If >1 products with the same LIDVID are registered by different nodes, we should respond with one of them
* `registry#185 <https://github.com/NASA-PDS/registry/issues/185>`_ **Implement Registry Multi-tenancy**
   * `registry-mgr#66 <https://github.com/NASA-PDS/registry-mgr/issues/66>`_ Update to utilize new multi-tenancy approach
   * `registry#179 <https://github.com/NASA-PDS/registry/issues/179>`_ Implement authorization handshake with API Gateway and Lambda for multi-tenancy approach
   * `harvest#118 <https://github.com/NASA-PDS/harvest/issues/118>`_ Update to utilize new multi-tenancy approach
   * `registry-api#304 <https://github.com/NASA-PDS/registry-api/issues/304>`_ Update to utilize new multi-tenancy approach
   * `validate#621 <https://github.com/NASA-PDS/validate/issues/621>`_ Re-test validate-refs using populated multi-tenant registry
   * `registry#188 <https://github.com/NASA-PDS/registry/issues/188>`_ Update Terraform scripts to support multi-tenancy
* `registry#186 <https://github.com/NASA-PDS/registry/issues/186>`_ **Enhance Terraform Scripts for Continuous Deployment and MCP**

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

   * - `User Guide <https://github.com/NASA-PDS/data-upload-manager#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/data-upload-manager>`_
     - `Issue Tracking <https://github.com/NASA-PDS/data-upload-manager/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/data-upload-manager/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/data-upload-manager/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/data-upload-manager/releases>`_ 

* `data-upload-manager#4 <https://github.com/NASA-PDS/data-upload-manager/issues/4>`_ **Develop Cost Model**
* `data-upload-manager#11 <https://github.com/NASA-PDS/data-upload-manager/issues/11>`_ **Refine Design and Prototype**
   * `data-upload-manager#3 <https://github.com/NASA-PDS/data-upload-manager/issues/3>`_ Develop initial design doc
   * `data-upload-manager#5 <https://github.com/NASA-PDS/data-upload-manager/issues/5>`_ Develop Ingress Service Routing Logic
   * `data-upload-manager#6 <https://github.com/NASA-PDS/data-upload-manager/issues/6>`_ Develop Ingress Lambda Logging Conventions
   * `data-upload-manager#8 <https://github.com/NASA-PDS/data-upload-manager/issues/8>`_ Develop Ingress Client Interface
* `data-upload-manager#12 <https://github.com/NASA-PDS/data-upload-manager/issues/12>`_ **Develop IaC for Deployment**
* `data-upload-manager#13 <https://github.com/NASA-PDS/data-upload-manager/issues/13>`_ **Test and Iterate with SBN and CSS**


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