Build 12.0 Plan
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
    * - 08/24/2021
      - SCR Freeze Date
      - DDWG
      - Freeze date for identifying SCRs to be implemented in this release.
    * - 08/24/2021
      - Standards Documents Updates Due
      - Document Authoring Team
      - Updates to PDS4 standards documents due to EN for review.
    * - 10/15/2021 - 11/12/2021
      - Beta Testing Period
      - DNs, IPDA
      - Changes to PDS4 IM and system components available for beta testing.
    * - 10/15/2021 - 11/12/2021
      - dLDD Integration and Test
      - dLDD Stewards
      - Auto-generated dLDDs should be reviews by dLDD Stewards, and final updates to dLDDs should be completed during this time.
    * - 11/12/2021
      - Standards Documents Review Due
      - Document Review Team
      - Review updates to PDS4 standards documents.
    * - 12/03/2021
      - System Release
      - EN
      - PDS4 system is operationally deployed and website is updated accordingly.

.. list-table:: Key Dates for Engineering Node
    :widths: 15 10 30
    :header-rows: 1

    * - Date
      - Name
      - Description
    * - 09/17/2021
      - Delivery to I&T
      - The PDS4 IM and all software updated during this 
        build cycle are delivered to EN I&T.
    * - 09/30/2021
      - Test Readiness Review (TRR)
      - PDS EN internal review to verify readiness to enter I&T phase.
    * - 11/17/2021
      - Delivery and Deployment Review (DRR)
      - PDS internal review with PDS Software Working Group to verify readiness to deploy build system.
    * - 12/03/2021
      - Operational Deployment
      - PDS4 system is operationally deployed and website is updated accordingly.

For a more detailed schedule, see https://pds-engineering.jpl.nasa.gov/content/schedules.

Planned PDS4 Information Model Changes
+++++++++++++++++++++++++++++++++++++++

This section details the planned changes to the PDS4 Information Model for this build. These changes are deliverables by the PDS Data Design Working Group (DDWG) to the Engineering Node for implementation.

* `validate#310 <https://github.com/NASA-PDS/validate/issues/310>`_ **Validate missing collections in bundle after CCB-282 updates**



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

* `validate#319 <https://github.com/NASA-PDS/validate/issues/319>`_ **B12.0 Configuration Improvements**
   * `validate#150 <https://github.com/NASA-PDS/validate/issues/150>`_ Update software to handle catalog files the same fashion when specified via command-line versus config file
* `validate#318 <https://github.com/NASA-PDS/validate/issues/318>`_ **B12.0 Content Validation Improvements**
   * `validate#57 <https://github.com/NASA-PDS/validate/issues/57>`_ As a user, I want to be warned when there are alphanumeric characters between fields in Table_Character
   * `validate#164 <https://github.com/NASA-PDS/validate/issues/164>`_ As a user, I want to validate PDF files are PDF/A
   * `validate#303 <https://github.com/NASA-PDS/validate/issues/303>`_ As a user, I want to the raise a WARNING if the object-defined size in the label does not match the file_size value
   * `validate#314 <https://github.com/NASA-PDS/validate/issues/314>`_ Revert #9: Do not throw ERROR message when ASCII Numeric field consists of only white space
* `validate#317 <https://github.com/NASA-PDS/validate/issues/317>`_ **B12.0 Referential Integrity Improvements**
   * `validate#69 <https://github.com/NASA-PDS/validate/issues/69>`_ As a user, I want to validate that all context objects specified in observational products are referenced in the parent bundle/collection Reference_List
   * `validate#307 <https://github.com/NASA-PDS/validate/issues/307>`_ As a user, I want to validate that all XML Schema collections in NASA PDS archives are secondary collections
   * `validate#308 <https://github.com/NASA-PDS/validate/issues/308>`_ As a user, I want to check that all Internal References are valid references to other PDS4 products within the current validating bundle

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

* `pds4-information-model#350 <https://github.com/NASA-PDS/pds4-information-model/issues/350>`_ **B12.0 PDS4 Information Model SCR Implementation**
* `pds4-information-model#349 <https://github.com/NASA-PDS/pds4-information-model/issues/349>`_ **Establish LDD Management Teams and Processes**
   * `pds4-information-model#347 <https://github.com/NASA-PDS/pds4-information-model/issues/347>`_ Create dLDD CCB
   * `pds4-information-model#348 <https://github.com/NASA-PDS/pds4-information-model/issues/348>`_ Create dLDD Stewardship Teams
* `pds4-information-model#326 <https://github.com/NASA-PDS/pds4-information-model/issues/326>`_ **B12.0 LDDTool Improvements**
   * `pds4-information-model#240 <https://github.com/NASA-PDS/pds4-information-model/issues/240>`_ Improve argument handling using argument parsing library
   * `pds4-information-model#269 <https://github.com/NASA-PDS/pds4-information-model/issues/269>`_ The PDS4 IM Specification Document is not consistent in the ordering of Permissible Values
   * `pds4-information-model#330 <https://github.com/NASA-PDS/pds4-information-model/issues/330>`_ As a user I want to know the output of the tool after it completes execution.
   * `pds4-information-model#338 <https://github.com/NASA-PDS/pds4-information-model/issues/338>`_ As a developer, I want to know the dLDD version from the output JSON data
   * `pds4-information-model#341 <https://github.com/NASA-PDS/pds4-information-model/issues/341>`_ As a user, I want to specify an IngestLDD using a relative path
   * `pds4-information-model#346 <https://github.com/NASA-PDS/pds4-information-model/issues/346>`_ lddtool's doc directory is not in tgz file
* `pds4-information-model#306 <https://github.com/NASA-PDS/pds4-information-model/issues/306>`_ **B12.0 Refactoring of IMTool**
   * `pds4-information-model#239 <https://github.com/NASA-PDS/pds4-information-model/issues/239>`_ Refactor Class information from config to Data Dictionary Protege ontology
   * `pds4-information-model#281 <https://github.com/NASA-PDS/pds4-information-model/issues/281>`_ Tag ops classes/attributes in IM so they are easily identifiable by users

--------

pds-deep-archive
################

*PDS Open Archival Information System (OAIS) utilities, including Submission Information Package (SIP) and Archive Information Package (AIP) generators*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-deep-archive/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-deep-archive>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-deep-archive/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-deep-archive/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-deep-archive/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-deep-archive/releases>`_ 

* `pds-deep-archive#105 <https://github.com/NASA-PDS/pds-deep-archive/issues/105>`_ **Integrate PDS Deep Archive with Registry**
   * `pds-deep-archive#7 <https://github.com/NASA-PDS/pds-deep-archive/issues/7>`_ As a user, I want to generate AIPs and SIPs using Registry
   * `pds-deep-archive#106 <https://github.com/NASA-PDS/pds-deep-archive/issues/106>`_ Improvements per API updates to remove workarounds from code
   * `pds-deep-archive#107 <https://github.com/NASA-PDS/pds-deep-archive/issues/107>`_ Improvements in API for "performance" workarounds in PDS Deep "Registry" Archive

--------

pds-doi-service
###############

*Service and tools for generating DOIs for PDS bundles, collections, and data sets*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-doi-service>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-doi-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-doi-service/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-doi-service/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-doi-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-doi-service/releases>`_ 

* `pds-doi-service#179 <https://github.com/NASA-PDS/pds-doi-service/issues/179>`_ **Develop DataCite Interface**
   * `pds-doi-service#103 <https://github.com/NASA-PDS/pds-doi-service/issues/103>`_ As the PDS, I want to mint DOIs through DataCite
* `pds-doi-service#178 <https://github.com/NASA-PDS/pds-doi-service/issues/178>`_ **B12.0 Refinements to DOI Service and UI for Initial Release**
   * `pds-doi-ui#13 <https://github.com/NASA-PDS/pds-doi-ui/issues/13>`_ Enable to remind previously used value in submitter and node for reserve
   * `pds-doi-ui#20 <https://github.com/NASA-PDS/pds-doi-ui/issues/20>`_ Autocompletion for doi or lidvid selection in release form
   * `pds-doi-ui#22 <https://github.com/NASA-PDS/pds-doi-ui/issues/22>`_ After reserve one file successfully, resubmit a new file
   * `pds-doi-service#153 <https://github.com/NASA-PDS/pds-doi-service/issues/153>`_ Prepare API and UI for production deployment
   * `pds-doi-service#163 <https://github.com/NASA-PDS/pds-doi-service/issues/163>`_ Dockerize API Service
   * `pds-doi-ui#34 <https://github.com/NASA-PDS/pds-doi-ui/issues/34>`_ As a user, I want to see the error/warnings messages on the same page from where they were raised
   * `pds-doi-service#176 <https://github.com/NASA-PDS/pds-doi-service/issues/176>`_ As an API user, I want to have pagination that is consistent with the PDS API.
   * `pds-doi-service#177 <https://github.com/NASA-PDS/pds-doi-service/issues/177>`_ As an API user I want to filter on lidvids with wildcards
   * `pds-doi-service#180 <https://github.com/NASA-PDS/pds-doi-service/issues/180>`_ As an API user I want to filter on PDS3 Data Set IDs with wildcards
   * `pds-doi-service#188 <https://github.com/NASA-PDS/pds-doi-service/issues/188>`_ As a user, I want to make sure I can not override existing DOI with new LIDVID
   * `pds-doi-service#192 <https://github.com/NASA-PDS/pds-doi-service/issues/192>`_ As a user, I want the application to support the history of PDS's DOIs, especially the one created for PDS3 products
* `pds-doi-service#86 <https://github.com/NASA-PDS/pds-doi-service/issues/86>`_ **Deploy DOI API and UI**
   * `pds-doi-service#87 <https://github.com/NASA-PDS/pds-doi-service/issues/87>`_ Dev beta testing with API
   * `pds-doi-service#88 <https://github.com/NASA-PDS/pds-doi-service/issues/88>`_ Operations team test interface with DOI Service
   * `pds-doi-service#89 <https://github.com/NASA-PDS/pds-doi-service/issues/89>`_ Update procedures to use DOI web interface submission
   * `pds-doi-service#90 <https://github.com/NASA-PDS/pds-doi-service/issues/90>`_ Deploy point build of DOI service and UI
   * `pds-doi-service#145 <https://github.com/NASA-PDS/pds-doi-service/issues/145>`_ review the full doi workflow and make it smooth for eng operators/users
   * `pds-doi-ui#35 <https://github.com/NASA-PDS/pds-doi-ui/issues/35>`_ As a SA, I don't want security vulnerabilities in the public UI
   * `pds-doi-service#187 <https://github.com/NASA-PDS/pds-doi-service/issues/187>`_ As a SA, I want the application to be deployed without security risks

--------

pds-registry-app
################

*Registry application enabling a PDS node to register all its data products for long term preservation and sharing with the rest of the PDS system.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-registry-app>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-registry-app/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-registry-app/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-registry-app/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-registry-app/releases>`_ 

* `pds-registry-app#155 <https://github.com/NASA-PDS/pds-registry-app/issues/155>`_ **[registry] Registry Regression Test and Documentation**
   * `pds-registry-app#153 <https://github.com/NASA-PDS/pds-registry-app/issues/153>`_ As a developer, I want to extend the registry-mgr and harvest using the Java API
   * `pds-registry-app#154 <https://github.com/NASA-PDS/pds-registry-app/issues/154>`_ As a manager, I want the registry to have regression tests included in CI
   * `pds-registry-app#156 <https://github.com/NASA-PDS/pds-registry-app/issues/156>`_ As a user, I want to uninstall the Registry and all its components
   * `pds-registry-app#157 <https://github.com/NASA-PDS/pds-registry-app/issues/157>`_ As a user, I want to upgrade the Registry and all its components
   * `pds-registry-app#158 <https://github.com/NASA-PDS/pds-registry-app/issues/158>`_ Update Registry App landing page to divert data users to separate landing page for using the PDS API
* `pds-registry-app#152 <https://github.com/NASA-PDS/pds-registry-app/issues/152>`_ **Pilot DN Registry + API AWS Deployments**
   * `pds-registry-app#90 <https://github.com/NASA-PDS/pds-registry-app/issues/90>`_ Develop cost model and reporting for Registry deployments

--------

pds-api
#######

*PDS API Application with client and server integrated into one package*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-api/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api/releases>`_ 

* `pds-api#24 <https://github.com/NASA-PDS/pds-api/issues/24>`_ **[registry] Handle PDS Supplemental Metadata**
   * `pds-registry-app#12 <https://github.com/NASA-PDS/pds-registry-app/issues/12>`_ As a user,  I want to ingest supplemental metadata for PDS products.
   * `pds-api#67 <https://github.com/NASA-PDS/pds-api/issues/67>`_ As an API user, I want to access supplemental metadata for PDS products.
* `pds-api#81 <https://github.com/NASA-PDS/pds-api/issues/81>`_ **[pds-api] B12.0 Improve API query handling**
   * `pds-api#71 <https://github.com/NASA-PDS/pds-api/issues/71>`_ As a user, I want to do a complex query to the API without being limited by the length of the url request
   * `pds-api#72 <https://github.com/NASA-PDS/pds-api/issues/72>`_ As an API user, I want to search by a temporal range as an ISO-8601 time interval.
   * `pds-api#83 <https://github.com/NASA-PDS/pds-api/issues/83>`_ As an API user, I want to search using URL parameters
* `pds-api#84 <https://github.com/NASA-PDS/pds-api/issues/84>`_ **[pds-api] Initial Google-like Search**
   * `pds-registry-app#49 <https://github.com/NASA-PDS/pds-registry-app/issues/49>`_ Enhance weighting and expected search results
* `pds-api#75 <https://github.com/NASA-PDS/pds-api/issues/75>`_ **[pds-api] B12.0 API Response Improvements**
   * `pds-api#65 <https://github.com/NASA-PDS/pds-api/issues/65>`_ As an API user, I want to get only the properties I explicitly requested.
   * `pds-api#66 <https://github.com/NASA-PDS/pds-api/issues/66>`_ As an API user, I want to get 'application/xml' content which matches the json structure
   * `pds-api#68 <https://github.com/NASA-PDS/pds-api/issues/68>`_ As an API user, I want to know in the response how many hits are returned for an API query.
   * `pds-api#70 <https://github.com/NASA-PDS/pds-api/issues/70>`_ As an API user, I want to know the unique values for a specific API field.
   * `registry-api-service#26 <https://github.com/NASA-PDS/registry-api-service/issues/26>`_ As a user, I want to know why my query syntax is invalid
* `pds-api#76 <https://github.com/NASA-PDS/pds-api/issues/76>`_ **[pds-api] Improve API Performance**
   * `registry-api-service#13 <https://github.com/NASA-PDS/registry-api-service/issues/13>`_ As a developer, I want to utilize ElasticSearch performance robustness for API response time requirements.
   * `registry-api-service#18 <https://github.com/NASA-PDS/registry-api-service/issues/18>`_ As an API user, I want an average query response time of 1 second.
   * `registry-api-service#19 <https://github.com/NASA-PDS/registry-api-service/issues/19>`_ As an API user, I want to handle long-running queries that take >10 seconds.
   * `pds-api#80 <https://github.com/NASA-PDS/pds-api/issues/80>`_ As a developer, I never want the label blob to be returned
* `pds-api#77 <https://github.com/NASA-PDS/pds-api/issues/77>`_ **[pds-api] PDS4 Product Relationships**
   * `pds-api#56 <https://github.com/NASA-PDS/pds-api/issues/56>`_ As an API user, I want to know the children and ancestors of bundle, collections, and products
   * `pds-api#59 <https://github.com/NASA-PDS/pds-api/issues/59>`_ As an API user, I want to know the Product(s) that belong to a given Bundle.
   * `pds-api#60 <https://github.com/NASA-PDS/pds-api/issues/60>`_ As an API user, I want to know the Bundle for a given Product.
   * `pds-api#61 <https://github.com/NASA-PDS/pds-api/issues/61>`_ As an API user, I want to know the Collection(s) for a given Product.
   * `pds-api#62 <https://github.com/NASA-PDS/pds-api/issues/62>`_ As an API user, I want to know the Bundle for a given Collection.
* `pds-api#79 <https://github.com/NASA-PDS/pds-api/issues/79>`_ **[pds-api] PDS Core Registry**
   * `pds-registry-app#150 <https://github.com/NASA-PDS/pds-registry-app/issues/150>`_ Develop plan for instituting AWS ES Cross Cluster Search 

--------

pdsen-corral
############

*umbrella project to manage the build cycle (continuous integration and stable release) for the PDS EN tools. *

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pdsen-corral>`_
     - `Github Repo <https://github.com/NASA-PDS/pdsen-corral>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pdsen-corral/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pdsen-corral/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pdsen-corral/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pdsen-corral/releases>`_ 

* `pdsen-corral#28 <https://github.com/NASA-PDS/pdsen-corral/issues/28>`_ **B12.0 Release Doc Improvements**
   * `pdsen-corral#19 <https://github.com/NASA-PDS/pdsen-corral/issues/19>`_ Propose a good management of requirements for parent/child components
   * `pds-github-util#7 <https://github.com/NASA-PDS/pds-github-util/issues/7>`_ As a PDS software user, I want to have a hierarchical view of the PDS EN components that apply to my user interests

--------

PDS.nasa.gov-UX
###############

*PDS.nasa.gov User Experience Task Issue and Prototype repository*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/PDS.nasa.gov-UX#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/PDS.nasa.gov-UX>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PDS.nasa.gov-UX/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PDS.nasa.gov-UX/releases>`_ 

* `PDS.nasa.gov-UX#78 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/78>`_ **Initial Design Validation and Usability Testing**
* `PDS.nasa.gov-UX#77 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/77>`_ **Initial Information Architecture**
* `PDS.nasa.gov-UX#79 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/79>`_ **Initial Visual Design**
* `PDS.nasa.gov-UX#76 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/76>`_ **User Personas and Stories**
* `PDS.nasa.gov-UX#75 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/75>`_ **User Testing for NASA CMS Trade Study**
* `PDS.nasa.gov-UX#74 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/74>`_ **Plan and Kick-off PDS WMWG**
   * `PDS.nasa.gov-UX#73 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/73>`_ Rev 3 of milestones to breakdown of notional goals and deliverables

--------

pdsen-operations
################

*Tickets for the PDSEN Operations Team*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pdsen-operations#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pdsen-operations>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pdsen-operations/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pdsen-operations/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pdsen-operations/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pdsen-operations/releases>`_ 

* `pdsen-operations#94 <https://github.com/NASA-PDS/pdsen-operations/issues/94>`_ **Develop and implement PDS CD Strategy**
   * `pds-api#51 <https://github.com/NASA-PDS/pds-api/issues/51>`_ As a developer, I want a continuous deployment of the API available for testing
   * `pdsen-operations#89 <https://github.com/NASA-PDS/pdsen-operations/issues/89>`_ As an SA, I want a monitoring capability to check that PDS search and access services are up and running 99.9% of the time
   * `pdsen-operations#95 <https://github.com/NASA-PDS/pdsen-operations/issues/95>`_ As a developer, I want a system for continuous deployment of PDS EN services in development.
* `pdsen-operations#93 <https://github.com/NASA-PDS/pdsen-operations/issues/93>`_ **Refine Continuous Integration processes**
   * `roundup-action#31 <https://github.com/NASA-PDS/roundup-action/issues/31>`_ Improve roundup action for tagging and releasing software packages
   * `roundup-action#36 <https://github.com/NASA-PDS/roundup-action/issues/36>`_ Java documentation is empty when attached to repo
   * `pdsen-operations#90 <https://github.com/NASA-PDS/pdsen-operations/issues/90>`_ As a developer, I want to make sure I have access to all our Python PyPi package repos.
   * `pdsen-operations#91 <https://github.com/NASA-PDS/pdsen-operations/issues/91>`_ As an EN developer, I want to make sure I have access to all PDS repos.
   * `roundup-action#37 <https://github.com/NASA-PDS/roundup-action/issues/37>`_ Document stable release CI/CD
   * `roundup-action#42 <https://github.com/NASA-PDS/roundup-action/issues/42>`_ Roundup environment doesn't appear to be taking packages seriously

--------

cloud-initiative
################

*PDS Cloud Migration documentation, issue, tracking and simple tools for assisting in the PDS hybrid cloud study and migration efforts.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/cloud-initiative#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/cloud-initiative>`_
     - `Issue Tracking <https://github.com/NASA-PDS/cloud-initiative/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/cloud-initiative/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/cloud-initiative/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/cloud-initiative/releases>`_ 

* `cloud-initiative#2 <https://github.com/NASA-PDS/cloud-initiative/issues/2>`_ **B12.0 Refine AWS Registry Deployment Strategy**
   * `pds-registry-app#89 <https://github.com/NASA-PDS/pds-registry-app/issues/89>`_ Document AWS deployment for Registry
   * `pds-registry-app#122 <https://github.com/NASA-PDS/pds-registry-app/issues/122>`_ Deploy the API on AWS as test
   * `cloud-initiative#1 <https://github.com/NASA-PDS/cloud-initiative/issues/1>`_ As a manager, I want a cost monitoring capability for AWS deployments
   * `pds-registry-app#151 <https://github.com/NASA-PDS/pds-registry-app/issues/151>`_ Employ budget alerts and if possible, rate/egress limits on AWS services


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
