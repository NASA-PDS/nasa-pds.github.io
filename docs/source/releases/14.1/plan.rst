Build 14.1 Plan
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
    * - 02/12/24
      - SCR Freeze Date
      - DDWG
      - Freeze date for identifying SCRs to be implemented in this release.
    * - 02/13/24 - 04/12/24
      - Standards Documents Updates Due
      - Document Authoring Team
      - Updates to PDS4 standards documents due to EN for review.
    * - 04/23/24 - 05/21/24
      - Beta Testing Period
      - DNs, IPDA
      - Changes to PDS4 IM and system components available for beta testing.
    * - 04/23/24 - 05/21/24
      - dLDD Integration and Test
      - dLDD Stewards
      - Auto-generated dLDDs should be reviews by dLDD Stewards, and final updates to dLDDs should be completed during this time.
    * - 04/12/24 - 05/22/24
      - Standards Documents Review Due
      - Document Review Team
      - Review updates to PDS4 standards documents.
    * - 06/07/24
      - System Release
      - EN
      - PDS4 system is operationally deployed and website is updated accordingly.

.. list-table:: Key Dates for Engineering Node
    :widths: 20 40 40
    :header-rows: 1

    * - Date
      - Name
      - Description
    * - 03/21/24
      - Delivery to I&T
      - The PDS4 IM and all software updated during this
        build cycle are delivered to EN I&T.
    * - 04/8/24
      - Test Readiness Review (TRR)
      - PDS EN internal review to verify readiness to enter I&T phase.
    * - 05/30/24
      - Delivery and Deployment Review (DRR)
      - PDS internal review with PDS Software Working Group to verify readiness to deploy build system.
    * - 06/07/24
      - Operational Deployment
      - PDS4 system is operationally deployed and website is updated accordingly.

For a more detailed schedule, see https://pds-engineering.jpl.nasa.gov/content/schedules.

Planned PDS4 Information Model Changes
+++++++++++++++++++++++++++++++++++++++

This section details the planned changes to the PDS4 Information Model for this build. These changes are deliverables by the PDS Data Design Working Group (DDWG) to the Engineering Node for implementation.

* `pds4-information-model#663 <https://github.com/NASA-PDS/pds4-information-model/issues/663>`_ **CCB-367: Superseded_by / Supersedes reference type**



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

* `validate#695 <https://github.com/NASA-PDS/validate/issues/695>`_ **Update Validate Test Suite to Support Larger Data Sets**
   * `validate#633 <https://github.com/NASA-PDS/validate/issues/633>`_ Reintegrate cucumber test for ticket #599
   * `validate#659 <https://github.com/NASA-PDS/validate/issues/659>`_ move test data to git large file storage repo
* `validate#696 <https://github.com/NASA-PDS/validate/issues/696>`_ **Use New Registry API for Context Product Validation**
   * `validate#592 <https://github.com/NASA-PDS/validate/issues/592>`_ As a user, I want to when a context product has been deprecated
   * `validate#675 <https://github.com/NASA-PDS/validate/issues/675>`_ Cutover to using new Registry API for generating context products json

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

* `pds4-information-model#700 <https://github.com/NASA-PDS/pds4-information-model/issues/700>`_ **Document Nuances for Reusability of Generic LDD Classes/Attributes**
   * `pds4-information-model#469 <https://github.com/NASA-PDS/pds4-information-model/issues/469>`_ As a namespace steward, I want to provide a more specific definition/nuance for a generic attribute
* `pds4-information-model#701 <https://github.com/NASA-PDS/pds4-information-model/issues/701>`_ **Implement Cucumber Framework for LDDTool**
* `pds4-information-model#703 <https://github.com/NASA-PDS/pds4-information-model/issues/703>`_ **B14.1 Information Model SCR Implementation**
   * `pds4-information-model#663 <https://github.com/NASA-PDS/pds4-information-model/issues/663>`_ CCB-367: Superseded_by / Supersedes reference type
* `pds4-information-model#704 <https://github.com/NASA-PDS/pds4-information-model/issues/704>`_ **B14.1 Information Model Delivery to I&T**
* `pds4-information-model#705 <https://github.com/NASA-PDS/pds4-information-model/issues/705>`_ **B14.1 Standards Documents Updates**

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

* `harvest#129 <https://github.com/NASA-PDS/harvest/issues/129>`_ **Add Support for LBLX File Extension**
   * `harvest#130 <https://github.com/NASA-PDS/harvest/issues/130>`_ As a user, I want to ingest data products with labels having `.lblx` file extension
* `harvest#131 <https://github.com/NASA-PDS/harvest/issues/131>`_ **Enhance support for searching lid/lidvid references**
   * `registry#215 <https://github.com/NASA-PDS/registry/issues/215>`_ Verify fields types are changed when LDD fields are reloaded

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

* `software-issues-repo#67 <https://github.com/NASA-PDS/software-issues-repo/issues/67>`_ **Migrate PDS JIRA to Atlassian Cloud JIRA**
   * `software-issues-repo#68 <https://github.com/NASA-PDS/software-issues-repo/issues/68>`_ Complete URS request for pds-jira.jpl.nasa.gov
   * `software-issues-repo#69 <https://github.com/NASA-PDS/software-issues-repo/issues/69>`_ Complete JIRA Open Source form for PDS JIRA
   * `software-issues-repo#70 <https://github.com/NASA-PDS/software-issues-repo/issues/70>`_ Export and Migrate JIRA to Atlassian Cloud
* `software-issues-repo#80 <https://github.com/NASA-PDS/software-issues-repo/issues/80>`_ **Upgrade Legacy Registry Tools and Services to Fix Vulnerability**
   * `operations#431 <https://github.com/NASA-PDS/operations/issues/431>`_ Deploy and Test legacy registry components on OL8
   * `registry-pds3-catalog#4 <https://github.com/NASA-PDS/registry-pds3-catalog/issues/4>`_ Upgrade Catalog Tool and dependencies to support Harvest/Registry upgrades
   * `ds-view#3 <https://github.com/NASA-PDS/ds-view/issues/3>`_ Upgrade Dataset View and dependencies to support Harvest/Registry upgrades
   * `search-ui-legacy#1 <https://github.com/NASA-PDS/search-ui-legacy/issues/1>`_ Upgrade Keyword Search and dependencies to support Harvest/Registry upgrades
   * `registry-mgr-legacy#3 <https://github.com/NASA-PDS/registry-mgr-legacy/issues/3>`_ Upgrade legacy registry mgr with upgraded log4j libraries and Solr 8.11.2
* `software-issues-repo#86 <https://github.com/NASA-PDS/software-issues-repo/issues/86>`_ **Complete Tasks and Artifacts Supporting NASA A&A Process**
   * `software-issues-repo#54 <https://github.com/NASA-PDS/software-issues-repo/issues/54>`_ As a user, I want to ensure no passwords/secrets are committed to a PDS repo
   * `software-issues-repo#87 <https://github.com/NASA-PDS/software-issues-repo/issues/87>`_ Develop Contingency Plans
   * `software-issues-repo#88 <https://github.com/NASA-PDS/software-issues-repo/issues/88>`_ Develop Disaster Recovery Plan
   * `software-issues-repo#89 <https://github.com/NASA-PDS/software-issues-repo/issues/89>`_ Develop Incident Response Plan
   * `software-issues-repo#90 <https://github.com/NASA-PDS/software-issues-repo/issues/90>`_ Update Software Management / Configuration Management Plans
   * `software-issues-repo#91 <https://github.com/NASA-PDS/software-issues-repo/issues/91>`_ Complete Contingency Plan Test
   * `software-issues-repo#92 <https://github.com/NASA-PDS/software-issues-repo/issues/92>`_ Develop Boundary Diagram for PDS-managed systems
   * `software-issues-repo#95 <https://github.com/NASA-PDS/software-issues-repo/issues/95>`_ Develop Continuous Monitoring Plan
* `software-issues-repo#93 <https://github.com/NASA-PDS/software-issues-repo/issues/93>`_ **B14.1 Bi-Annual Triage CodeQL Static Code Analysis Scan Results**
* `software-issues-repo#94 <https://github.com/NASA-PDS/software-issues-repo/issues/94>`_ **B14.1 Prep for I&T**

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

* `portal-wp-tasks#42 <https://github.com/NASA-PDS/portal-wp-tasks/issues/42>`_ **Deploy Dev Wordpress Environment in MCP**
* `portal-wp-tasks#44 <https://github.com/NASA-PDS/portal-wp-tasks/issues/44>`_ **Develop Initial Headless Wordpress Docker Deployment**
   * `portal-wp-tasks#43 <https://github.com/NASA-PDS/portal-wp-tasks/issues/43>`_ As a developer, I want to deploy a local instance of headless wordpress and latest code using Docker
   * `portal-wp-tasks#45 <https://github.com/NASA-PDS/portal-wp-tasks/issues/45>`_ Why headless over vanilla Wordpress?
* `portal-wp-tasks#49 <https://github.com/NASA-PDS/portal-wp-tasks/issues/49>`_ **Implement Header**
   * `portal-wp-tasks#50 <https://github.com/NASA-PDS/portal-wp-tasks/issues/50>`_ Implement Navbar
   * `portal-wp-tasks#51 <https://github.com/NASA-PDS/portal-wp-tasks/issues/51>`_ Implement Titlebar (logo, node navigation, search)
   * `portal-wp-tasks#55 <https://github.com/NASA-PDS/portal-wp-tasks/issues/55>`_ Updated header components
* `portal-wp-tasks#56 <https://github.com/NASA-PDS/portal-wp-tasks/issues/56>`_ **Implement Initial Investigation Landing Page Template and Associated Components**
* `portal-wp-tasks#57 <https://github.com/NASA-PDS/portal-wp-tasks/issues/57>`_ **Implement Initial Bundle/Collection Landing Pages and Associated Components**
* `portal-wp-tasks#58 <https://github.com/NASA-PDS/portal-wp-tasks/issues/58>`_ **Implement Initial Search Results Page and Associated Components**

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
   * `operations#399 <https://github.com/NASA-PDS/operations/issues/399>`_ Submit new URS request
* `operations#424 <https://github.com/NASA-PDS/operations/issues/424>`_ **Add Data Registration Validation and Deep Archive Execution to Nominal Data Release Process**
* `operations#460 <https://github.com/NASA-PDS/operations/issues/460>`_ **B14.1 dLDD Build and I&T**
* `operations#456 <https://github.com/NASA-PDS/operations/issues/456>`_ **B14.1 EN Deployment & Release**

--------

roundup-action
##############

*Do a "roundup", a/k/a PDS-style continuous integration and delivery*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/roundup-action#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/roundup-action>`_
     - `Issue Tracking <https://github.com/NASA-PDS/roundup-action/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/roundup-action/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/roundup-action/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/roundup-action/releases>`_ 

* `roundup-action#114 <https://github.com/NASA-PDS/roundup-action/issues/114>`_ **Develop CI/CD for React Projects**
   * `wds-react-legacy#95 <https://github.com/NASA-PDS/wds-react-legacy/issues/95>`_ Setup NPM Audits as part of CI on React projects
   * `roundup-action#118 <https://github.com/NASA-PDS/roundup-action/issues/118>`_ Develop React template repo
   * `roundup-action#119 <https://github.com/NASA-PDS/roundup-action/issues/119>`_ Develop Branch Testing Github Action
   * `roundup-action#120 <https://github.com/NASA-PDS/roundup-action/issues/120>`_ Develop Unstable GitHub Action CI/CD to I&T Staging venue
   * `roundup-action#121 <https://github.com/NASA-PDS/roundup-action/issues/121>`_ Develop Stable GitHub Action CI/CD to I&T production venue
   * `roundup-action#122 <https://github.com/NASA-PDS/roundup-action/issues/122>`_ Develop PR Review GitHub Action CI/CD to Developer Staging venue
   * `roundup-action#123 <https://github.com/NASA-PDS/roundup-action/issues/123>`_ Develop Initial Architecture and Action Flow for React CI/CD Deployments

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

search-api-notebook
###################

*Jupyter notebooks for demonstrating and utilizing the Planetary Data System (PDS) Search API*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/search-api-notebook#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/search-api-notebook>`_
     - `Issue Tracking <https://github.com/NASA-PDS/search-api-notebook/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/search-api-notebook/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/search-api-notebook/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/search-api-notebook/releases>`_ 

* `search-api-notebook#24 <https://github.com/NASA-PDS/search-api-notebook/issues/24>`_ **Geographic data extraction and visualization**
   * `search-api-notebook#12 <https://github.com/NASA-PDS/search-api-notebook/issues/12>`_ Test extracting lat/long bounding box info from python component with STAC API
   * `search-api-notebook#14 <https://github.com/NASA-PDS/search-api-notebook/issues/14>`_ Connect leaflet-cartocosmos component to the TBD data bounding box attributes in the registry-api
   * `search-api-notebook#25 <https://github.com/NASA-PDS/search-api-notebook/issues/25>`_ Use GDAL Digital Elevation Model visualization features

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

* `planetary-data-cloud#35 <https://github.com/NASA-PDS/planetary-data-cloud/issues/35>`_ **MCP Pilot: Deploy Registry**
   * `registry#218 <https://github.com/NASA-PDS/registry/issues/218>`_ Add registry costs to the PDS EN Cloud spreadsheet
   * `registry#222 <https://github.com/NASA-PDS/registry/issues/222>`_ Setup OIDC Authentication for MCP
   * `registry#223 <https://github.com/NASA-PDS/registry/issues/223>`_ OpenSearch Serverless Setup in MCP
* `planetary-data-cloud#61 <https://github.com/NASA-PDS/planetary-data-cloud/issues/61>`_ **Design and Implement Initial Archive Browser Beta**
* `planetary-data-cloud#69 <https://github.com/NASA-PDS/planetary-data-cloud/issues/69>`_ **Design and Implement Minor Planet Center Cloud Backup Solution**
* `planetary-data-cloud#71 <https://github.com/NASA-PDS/planetary-data-cloud/issues/71>`_ **CSS MVP: Identify Requirements and Prep for CSS in AWS Open Data Registry**
* `planetary-data-cloud#76 <https://github.com/NASA-PDS/planetary-data-cloud/issues/76>`_ **Design and Implement Warm Storage Data Backup Solution**
   * `planetary-data-cloud#75 <https://github.com/NASA-PDS/planetary-data-cloud/issues/75>`_ As a user, I want a warm backup of my archive data to be available in the event of corruption of of primary archive data
   * `nucleus#73 <https://github.com/NASA-PDS/nucleus/issues/73>`_ As a user, I want to store a copy of my archive data in AWS Deep Archive / Glacier in another region from the primary copy
* `planetary-data-cloud#77 <https://github.com/NASA-PDS/planetary-data-cloud/issues/77>`_ **B14.1 Bi-Annual Cost Model Review**
* `planetary-data-cloud#79 <https://github.com/NASA-PDS/planetary-data-cloud/issues/79>`_ **Migrate Existing JPL AWS Infra to MCP**
   * `planetary-data-cloud#81 <https://github.com/NASA-PDS/planetary-data-cloud/issues/81>`_ Migrate PDS EC2 instances from JPL AWS to MCP

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

* `devops#37 <https://github.com/NASA-PDS/devops/issues/37>`_ **Automatically deploy an up to date I&T platform where all software can be tested (Part 2)**
   * `registry-api#269 <https://github.com/NASA-PDS/registry-api/issues/269>`_ Add registry/docker compose integration tests to github action on dev branches
   * `devops#36 <https://github.com/NASA-PDS/devops/issues/36>`_ For registry components, add a github action which runs the integration test when something is pushed on a dev branch
   * `registry-sweepers#6 <https://github.com/NASA-PDS/registry-sweepers/issues/6>`_ Create the docker image and push it to docker hub as part of the CICD
   * `devops#41 <https://github.com/NASA-PDS/devops/issues/41>`_ Push docker image on AWS ECR in github-actions, in addition to docker hub
   * `devops#44 <https://github.com/NASA-PDS/devops/issues/44>`_ Ask new Application developer profile on JPL AWS
   * `devops#45 <https://github.com/NASA-PDS/devops/issues/45>`_ Use Github Actions Github-Hosted Runner to deploy to NGAP
   * `devops#46 <https://github.com/NASA-PDS/devops/issues/46>`_ Fully terraform the registry application
   * `devops#47 <https://github.com/NASA-PDS/devops/issues/47>`_ Other CICD improvements
   * `devops#48 <https://github.com/NASA-PDS/devops/issues/48>`_ Use JPL AWS jenkins to launch terraform scripts

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

* `nucleus#17 <https://github.com/NASA-PDS/nucleus/issues/17>`_ **CSS MVP: Deploy Baseline Nucleus for Catalina Sky Survey**
* `nucleus#66 <https://github.com/NASA-PDS/nucleus/issues/66>`_ **MCP Pilot: Pilot Nucleus Deployment for CSS and MESSENGER MDIS Data**
   * `nucleus#52 <https://github.com/NASA-PDS/nucleus/issues/52>`_ Work with IMG to connect to S3 Bucket with MESSENGER data
   * `nucleus#53 <https://github.com/NASA-PDS/nucleus/issues/53>`_ Deploy and Test Nucleus DAG for MESSENGER processing
   * `nucleus#54 <https://github.com/NASA-PDS/nucleus/issues/54>`_ Validate and Load all PDS4 MESSENGER data products with Nucleus
   * `nucleus#61 <https://github.com/NASA-PDS/nucleus/issues/61>`_ Manually validate and load MESSENGER MSGRMDS_4001 and MESSDEM_1001 data
   * `nucleus#68 <https://github.com/NASA-PDS/nucleus/issues/68>`_ Setting-up MWAA Environment on MCP
   * `nucleus#74 <https://github.com/NASA-PDS/nucleus/issues/74>`_ Support processing of PDS products with fitz file format in Nucleus
* `nucleus#62 <https://github.com/NASA-PDS/nucleus/issues/62>`_ **Develop Support For Off-Nominal Data Loads**

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

* `registry#155 <https://github.com/NASA-PDS/registry/issues/155>`_ **Registry Multi-tenancy Design and implementation with Cognito**
   * `registry#179 <https://github.com/NASA-PDS/registry/issues/179>`_ Implement authorization handshake with API Gateway and Lambda for multi-tenancy approach
* `registry#178 <https://github.com/NASA-PDS/registry/issues/178>`_ **Improved Fault Tolerance for Registry and Registry API**
   * `registry-common#26 <https://github.com/NASA-PDS/registry-common/issues/26>`_ [SECURITY] Fix code scanning alert - `TrustManager` that accepts all certificates
   * `harvest#101 <https://github.com/NASA-PDS/harvest/issues/101>`_ Unexpected WARNINGs related to http requests
   * `registry-api#292 <https://github.com/NASA-PDS/registry-api/issues/292>`_ Queries for data products with lots of metadata attributes crash in browser
   * `registry-api#300 <https://github.com/NASA-PDS/registry-api/issues/300>`_ Update Java params and Docker image to expand JVM memory beyond 50%
   * `harvest#119 <https://github.com/NASA-PDS/harvest/issues/119>`_ As a developer, I want to know what version of Harvest was used to load a product
   * `registry-api#337 <https://github.com/NASA-PDS/registry-api/issues/337>`_ Enhance robustness of API Monitoring
   * `registry-sweepers#25 <https://github.com/NASA-PDS/registry-sweepers/issues/25>`_ Enhance provenance sweeper with more graceful failure when registry contains zero documents
   * `harvest#125 <https://github.com/NASA-PDS/harvest/issues/125>`_ Improve Fault Tolerance of Harvest for Forbidden Access error and Timeout
   * `registry#211 <https://github.com/NASA-PDS/registry/issues/211>`_ As an operator, I want to be notified of when Registry storage capacity exceeds 75% capacity.
   * `registry-api#361 <https://github.com/NASA-PDS/registry-api/issues/361>`_ As a user, I want my API request to execute successfully even when the registry contains corrupted documents
   * `registry#224 <https://github.com/NASA-PDS/registry/issues/224>`_ Write documentation and Training for Registry monitoring
   * `registry#225 <https://github.com/NASA-PDS/registry/issues/225>`_ Registry-Sweepers Multiple Updates Detected
   * `registry-sweepers#69 <https://github.com/NASA-PDS/registry-sweepers/issues/69>`_ Registry-Sweepers Error: contained no hits when hits were expected
   * `registry-api#378 <https://github.com/NASA-PDS/registry-api/issues/378>`_ Investigate and fix intermittent Registry-API Errors
   * `harvest#133 <https://github.com/NASA-PDS/harvest/issues/133>`_ `Data too large` error from very large data products
   * `harvest#134 <https://github.com/NASA-PDS/harvest/issues/134>`_ `Too many requests` error to OpenSearch
* `registry#181 <https://github.com/NASA-PDS/registry/issues/181>`_ **Support Registration and Search of Products Replicated Across Archives**
   * `registry-api#306 <https://github.com/NASA-PDS/registry-api/issues/306>`_ If >1 products with the same LIDVID are registered by different nodes, we should respond with one of them
   * `registry#245 <https://github.com/NASA-PDS/registry/issues/245>`_ As a user, I want to register data product(s) that is mirrored across 2 or more organizations
* `registry#185 <https://github.com/NASA-PDS/registry/issues/185>`_ **Implement Registry Multi-tenancy without Cognito in the loop**
   * `registry-mgr#66 <https://github.com/NASA-PDS/registry-mgr/issues/66>`_ Update to utilize new multi-tenancy approach
   * `harvest#118 <https://github.com/NASA-PDS/harvest/issues/118>`_ Update to utilize new multi-tenancy approach
   * `registry-api#304 <https://github.com/NASA-PDS/registry-api/issues/304>`_ Update to utilize new multi-tenancy approach
   * `validate#621 <https://github.com/NASA-PDS/validate/issues/621>`_ Re-test validate-refs using populated multi-tenant registry
   * `registry#188 <https://github.com/NASA-PDS/registry/issues/188>`_ Update Terraform scripts to support multi-tenancy
   * `registry#212 <https://github.com/NASA-PDS/registry/issues/212>`_ Design scalable, multi-tenant opensearch
   * `registry#217 <https://github.com/NASA-PDS/registry/issues/217>`_ Write a migration plan to multitenant registry
   * `registry-sweepers#60 <https://github.com/NASA-PDS/registry-sweepers/issues/60>`_ Registry-Sweeper ECS Enchancements (Post Multi-Tenancy)
   * `registry#223 <https://github.com/NASA-PDS/registry/issues/223>`_ OpenSearch Serverless Setup in MCP
* `registry#230 <https://github.com/NASA-PDS/registry/issues/230>`_ **Enable Support for Changing Field Types**
* `registry#231 <https://github.com/NASA-PDS/registry/issues/231>`_ **Design and Implement Support for Alternate Data File Paths**
   * `registry#96 <https://github.com/NASA-PDS/registry/issues/96>`_ As a user I want to change the file paths of products in the registry
   * `harvest#123 <https://github.com/NASA-PDS/harvest/issues/123>`_ As a Node Operator, I want to specify an alternate file paths for 1 or more archive products
   * `registry#209 <https://github.com/NASA-PDS/registry/issues/209>`_ As a user, I want to manually update a product's file location (file_ref)

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

planetary-data-engine
#####################

*Free-text search capability for planetary data, services, tools, and information*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/planetary-data-engine#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/planetary-data-engine>`_
     - `Issue Tracking <https://github.com/NASA-PDS/planetary-data-engine/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/planetary-data-engine/issues?q=is%3Aopen+is%3Aissue+label%icebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/planetary-data-engine/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/planetary-data-engine/releases>`_ 

* `planetary-data-engine#5 <https://github.com/NASA-PDS/planetary-data-engine/issues/5>`_ **Complete Sinequa Useability Analysis**
   * `planetary-data-engine#9 <https://github.com/NASA-PDS/planetary-data-engine/issues/9>`_ Make requirement analysis & trade study for PDS Web Search
   * `planetary-data-engine#8 <https://github.com/NASA-PDS/planetary-data-engine/issues/8>`_ Working with Jupyter Notebook to show various features to be used by UI team
* `planetary-data-engine#7 <https://github.com/NASA-PDS/planetary-data-engine/issues/7>`_ **Develop Query Test Suite and Success Criteria**
   * `planetary-data-engine#14 <https://github.com/NASA-PDS/planetary-data-engine/issues/14>`_ Create test cases for evaluation of PDS search quality
   * `planetary-data-engine#15 <https://github.com/NASA-PDS/planetary-data-engine/issues/15>`_ Design and develop a new tool to evaluate the quality of a set of search results

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

* `data-upload-manager#4 <https://github.com/NASA-PDS/data-upload-manager/issues/4>`_ **Develop Cost Model**
* `data-upload-manager#13 <https://github.com/NASA-PDS/data-upload-manager/issues/13>`_ **CSS MVP: Deploy to MCP and Test Uploads to Nucleus**
   * `data-upload-manager#31 <https://github.com/NASA-PDS/data-upload-manager/issues/31>`_ Upload test data set with manual trigger of Nucleus
   * `data-upload-manager#32 <https://github.com/NASA-PDS/data-upload-manager/issues/32>`_ Test upload subset of CSS with manual trigger of Nucleus
   * `registry#238 <https://github.com/NASA-PDS/registry/issues/238>`_ Assist with DUM infra setup in MCP
   * `nucleus#71 <https://github.com/NASA-PDS/nucleus/issues/71>`_ Support CSS demo 
* `data-upload-manager#29 <https://github.com/NASA-PDS/data-upload-manager/issues/29>`_ **Develop Directory Write Locking Mechanism**


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