Build 11.1 Plan
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

.. list-table:: Key Dates
    :widths: 15 10 30
    :header-rows: 1

    * - Date
      - Name
      - Description
    * - 03/19/2021
      - Delivery to I&T
      - The PDS4 IM and all software updated during this 
        build cycle are delivered to EN I&T.
    * - 04/05/2021
      - Test Readiness Review (TRR)
      - PDS EN internal review to verify readiness to enter I&T phase.
    * - 05/27/2021
      - Delivery and Deployment Review (DRR)
      - PDS internal review with PDS Software Working Group to verify readiness to deploy build system.
    * - 06/11/2021
      - Operational Deployment
      - PDS4 system is operationally deployed and website is updated accordingly.

For a more detailed schedule, see https://pds-engineering.jpl.nasa.gov/content/schedules.

Planned PDS4 Information Model Changes
+++++++++++++++++++++++++++++++++++++++

This section details the planned changes to the PDS4 Information Model for this build. These changes are deliverables by the PDS Data Design Working Group (DDWG) to the Engineering Node for implementation.

* `pds4-information-model#258 <https://github.com/NASA-PDS/pds4-information-model/issues/258>`_ **CCB-301: The attribute <name> in the <DD_Attribute> and <DD_Class> classes is not properly constrained**
* `pds4-information-model#256 <https://github.com/NASA-PDS/pds4-information-model/issues/256>`_ **CCB-312: <ldd_version_id> does not appear to be constrained the way LDDTool expects**
* `pds4-information-model#254 <https://github.com/NASA-PDS/pds4-information-model/issues/254>`_ **CCB-305: Missing validation constraint on <specified_unit_id>**
* `pds4-information-model#253 <https://github.com/NASA-PDS/pds4-information-model/issues/253>`_ **CCB-313: Definition of <external_source_product_identifier> refers to non-existent documentation**
* `pds4-information-model#249 <https://github.com/NASA-PDS/pds4-information-model/issues/249>`_ **CCB-288: Change Internal_Reference reference type to 'guided' text**
* `pds4-information-model#257 <https://github.com/NASA-PDS/pds4-information-model/issues/257>`_ **CCB-302: No <reference_type> values defined in DD_Attribute or DD_Class contexts**
* `pds4-information-model#255 <https://github.com/NASA-PDS/pds4-information-model/issues/255>`_ **CCB-300: Apparently deprecated units of measure are not actually deprecated**
* `pds4-information-model#251 <https://github.com/NASA-PDS/pds4-information-model/issues/251>`_ **CCB-303: The definition for <skos_relation_name> is not sufficient.**
* `pds4-information-model#250 <https://github.com/NASA-PDS/pds4-information-model/issues/250>`_ **CCB-315: "PDS3" is an allowed parsing standard for Bundle documentation file**



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

* `validate#250 <https://github.com/NASA-PDS/validate/issues/250>`_ **Improvements to meet updated Standards Reference since initial requirements implementation**
   * `validate#5 <https://github.com/NASA-PDS/validate/issues/5>`_ Improve file base name check according to Standards Reference
   * `validate#6 <https://github.com/NASA-PDS/validate/issues/6>`_ Improve pds4.bundle unlabeled files check to handle files without a file suffix
   * `validate#11 <https://github.com/NASA-PDS/validate/issues/11>`_ Update allowable field_format values per Standards Reference definition regarding [+|-] characters
   * `validate#81 <https://github.com/NASA-PDS/validate/issues/81>`_ Validate and throw error when duplicate LIDs are found in Bundle
   * `validate#153 <https://github.com/NASA-PDS/validate/issues/153>`_ Update validate to throw error when a file has a space in the filename
   * `validate#230 <https://github.com/NASA-PDS/validate/issues/230>`_ Update validate per SR requirements for collection inventories
   * `validate#240 <https://github.com/NASA-PDS/validate/issues/240>`_ Unexpected error for data collection in a sub-directory
   * `validate#242 <https://github.com/NASA-PDS/validate/issues/242>`_ Update LID validation to meet latest PDS4 SR Requirements
* `validate#249 <https://github.com/NASA-PDS/validate/issues/249>`_ **Improvements for validating accumulating bundles / collections**
   * `validate#51 <https://github.com/NASA-PDS/validate/issues/51>`_ Provide the capability to specify multiple locations for pds4.bundle validation
   * `validate#231 <https://github.com/NASA-PDS/validate/issues/231>`_ For accumulating bundles, validate latest version of collections only
   * `validate#238 <https://github.com/NASA-PDS/validate/issues/238>`_ validate does not perform full bundle validation when using a specific bundle.xml
   * `validate#246 <https://github.com/NASA-PDS/validate/issues/246>`_ Add output directory flag to validate-bundle tool
   * `validate#256 <https://github.com/NASA-PDS/validate/issues/256>`_ validate should only do integrity checking on latest version of a collection when referenced by LID

--------

pds4-jparser
############

*Java Library providing APIs for parsing and exporting information on PDS4 products, including table and image objects to various formats including CSV, PNG, VICAR, FITs, etc.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-jparser/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-jparser>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-jparser/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds4-jparser/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-jparser/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-jparser/releases>`_ 

* `pds4-jparser#21 <https://github.com/NASA-PDS/pds4-jparser/issues/21>`_ **Update table reads for large files and improve memory footprints**
   * `validate#189 <https://github.com/NASA-PDS/validate/issues/189>`_ Validate error reading tables > 2GiB

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

* `pds4-information-model#242 <https://github.com/NASA-PDS/pds4-information-model/issues/242>`_ **DocBook HTML/WebHelp generation and conversion processes**
   * `pds4-information-model#170 <https://github.com/NASA-PDS/pds4-information-model/issues/170>`_ LDDTool: DocBook generation does not work from any file system location
   * `pds4-information-model#243 <https://github.com/NASA-PDS/pds4-information-model/issues/243>`_ Document how to generate the DocBook XML and how to generate HTML/WebHelp
* `pds4-information-model#241 <https://github.com/NASA-PDS/pds4-information-model/issues/241>`_ **Improvements from Build 11.0 testing**
   * `pds4-information-model#104 <https://github.com/NASA-PDS/pds4-information-model/issues/104>`_ LDDTool: Enable to ability to set custom namespace base URI in IngestLDD  
   * `pds4-information-model#175 <https://github.com/NASA-PDS/pds4-information-model/issues/175>`_ LDDTool: Displaying invalid Imaging Discipline Classes
   * `pds4-information-model#186 <https://github.com/NASA-PDS/pds4-information-model/issues/186>`_ PDS4_PDS_1E00.sch inconsistent rules for type of Investigation vs Investigation_Area
   * `pds4-information-model#235 <https://github.com/NASA-PDS/pds4-information-model/issues/235>`_ Incorrect error messages for DD_Associate_External_Class
* `pds4-information-model#238 <https://github.com/NASA-PDS/pds4-information-model/issues/238>`_ **Continuing refactoring of IMTool / LDDTool**
   * `pds4-information-model#239 <https://github.com/NASA-PDS/pds4-information-model/issues/239>`_ Refactor Class information from config to Data Dictionary Protege ontology
   * `pds4-information-model#240 <https://github.com/NASA-PDS/pds4-information-model/issues/240>`_ Improve argument handling using argument parsing library

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

* `pds-deep-archive#80 <https://github.com/NASA-PDS/pds-deep-archive/issues/80>`_ **NSSDCA Delivery Onboarding**

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

* `pds-doi-service#68 <https://github.com/NASA-PDS/pds-doi-service/issues/68>`_ **Develop Web UI for DOI service**
   * `pds-doi-service#67 <https://github.com/NASA-PDS/pds-doi-service/issues/67>`_ Mock web UI for DOI management 
   * `pds-doi-service#108 <https://github.com/NASA-PDS/pds-doi-service/issues/108>`_ Reserve DOI UI forms
   * `pds-doi-service#109 <https://github.com/NASA-PDS/pds-doi-service/issues/109>`_ Release existing DOI (previously reserved, drafted or released) UI forms
   * `pds-doi-service#110 <https://github.com/NASA-PDS/pds-doi-service/issues/110>`_ Release new DOI forms
* `pds-doi-service#52 <https://github.com/NASA-PDS/pds-doi-service/issues/52>`_ **API Implementation for DOI Service**
   * `pds-doi-service#38 <https://github.com/NASA-PDS/pds-doi-service/issues/38>`_ Add Status / Query component to API
   * `pds-doi-service#77 <https://github.com/NASA-PDS/pds-doi-service/issues/77>`_ Add POST PDS4 or  OSTI DOI label to API
   * `pds-doi-service#78 <https://github.com/NASA-PDS/pds-doi-service/issues/78>`_ Add POST Reserve xslx/csv DOI function to API
   * `pds-doi-service#79 <https://github.com/NASA-PDS/pds-doi-service/issues/79>`_ Add Release DOI function to API
   * `pds-doi-service#80 <https://github.com/NASA-PDS/pds-doi-service/issues/80>`_ Develop API specification in SwaggerHub
   * `pds-doi-service#100 <https://github.com/NASA-PDS/pds-doi-service/issues/100>`_ Add GET DOI to the API
   * `pds-doi-service#101 <https://github.com/NASA-PDS/pds-doi-service/issues/101>`_ Add PUT DOI to the API (for updates)
   * `pds-doi-service#105 <https://github.com/NASA-PDS/pds-doi-service/issues/105>`_ Complete get DOIS criterias with the arguments proposed in command line
   * `pds-doi-service#106 <https://github.com/NASA-PDS/pds-doi-service/issues/106>`_ Add exception name in the error messages
   * `pds-doi-service#107 <https://github.com/NASA-PDS/pds-doi-service/issues/107>`_ allow to post PDS4 labels in the payload (for draft)
* `pds-doi-service#91 <https://github.com/NASA-PDS/pds-doi-service/issues/91>`_ **Develop User Access / Management Strategy**
* `pds-doi-service#86 <https://github.com/NASA-PDS/pds-doi-service/issues/86>`_ **Deploy DOI API and UI**
   * `pds-doi-service#87 <https://github.com/NASA-PDS/pds-doi-service/issues/87>`_ Dev beta testing with API
   * `pds-doi-service#88 <https://github.com/NASA-PDS/pds-doi-service/issues/88>`_ Operations team test interface with DOI Service
   * `pds-doi-service#89 <https://github.com/NASA-PDS/pds-doi-service/issues/89>`_ Update procedures to use DOI web interface submission
   * `pds-doi-service#90 <https://github.com/NASA-PDS/pds-doi-service/issues/90>`_ Deploy point build of DOI service and UI
* `pds-doi-service#23 <https://github.com/NASA-PDS/pds-doi-service/issues/23>`_ **Document how to Deactivate a DOI (with curl command)**

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

* `pds-registry-app#13 <https://github.com/NASA-PDS/pds-registry-app/issues/13>`_ **Beta test operational deployment**
   * `pds-registry-app#82 <https://github.com/NASA-PDS/pds-registry-app/issues/82>`_ Develop test plan
   * `pds-registry-app#83 <https://github.com/NASA-PDS/pds-registry-app/issues/83>`_ Deploy and install multi-node ES
   * `pds-registry-app#84 <https://github.com/NASA-PDS/pds-registry-app/issues/84>`_ Download large data set for testing
   * `pds-registry-app#85 <https://github.com/NASA-PDS/pds-registry-app/issues/85>`_ Document performance benchmarks in registry app docs
* `pds-registry-app#42 <https://github.com/NASA-PDS/pds-registry-app/issues/42>`_ **Integrate Registry API into pds-registry-app**
* `pds-registry-app#27 <https://github.com/NASA-PDS/pds-registry-app/issues/27>`_ **Manage PDS4 product relationships**
   * `pds-registry-app#76 <https://github.com/NASA-PDS/pds-registry-app/issues/76>`_ Manage relationships between bundles / collections / products
   * `pds-registry-app#77 <https://github.com/NASA-PDS/pds-registry-app/issues/77>`_ Manage relationships described by reference types
   * `pds-registry-app#97 <https://github.com/NASA-PDS/pds-registry-app/issues/97>`_ Research RDF technologies to handle pds4 label cross-references in the registry
* `pds-registry-app#92 <https://github.com/NASA-PDS/pds-registry-app/issues/92>`_ **Update Registry API per PDS API v0-beta**
* `pds-registry-app#91 <https://github.com/NASA-PDS/pds-registry-app/issues/91>`_ **Deploy Registries in AWS**
   * `pds-registry-app#86 <https://github.com/NASA-PDS/pds-registry-app/issues/86>`_ Deploy EN Registry in AWS
   * `pds-registry-app#87 <https://github.com/NASA-PDS/pds-registry-app/issues/87>`_ Deploy GEO Registry in AWS
   * `pds-registry-app#88 <https://github.com/NASA-PDS/pds-registry-app/issues/88>`_ Deploy IMG Registry in AWS
   * `pds-registry-app#89 <https://github.com/NASA-PDS/pds-registry-app/issues/89>`_ Document AWS deployment for Registry
   * `pds-registry-app#90 <https://github.com/NASA-PDS/pds-registry-app/issues/90>`_ Develop cost model and reporting for Registry deployments
* `pds-registry-app#81 <https://github.com/NASA-PDS/pds-registry-app/issues/81>`_ **Registry Integration component**
* `pds-registry-app#12 <https://github.com/NASA-PDS/pds-registry-app/issues/12>`_ **Ingest PDS supplemental metadata**
* `pds-registry-app#53 <https://github.com/NASA-PDS/pds-registry-app/issues/53>`_ **Improve Attribute Search Component**
   * `pds-registry-app#45 <https://github.com/NASA-PDS/pds-registry-app/issues/45>`_ Validate Elastic Search index configuration for attribute search
   * `pds-registry-app#61 <https://github.com/NASA-PDS/pds-registry-app/issues/61>`_ Update the index schema in ES dynamically when new record are ingested
   * `pds-registry-app#64 <https://github.com/NASA-PDS/pds-registry-app/issues/64>`_ Fix the Json data dictionary format  
   * `pds-registry-mgr-elastic#5 <https://github.com/NASA-PDS/pds-registry-mgr-elastic/issues/5>`_ Create a field-data type lookup table
   * `pds-registry-mgr-elastic#6 <https://github.com/NASA-PDS/pds-registry-mgr-elastic/issues/6>`_ Update the field-data type lookup table
   * `pds-registry-app#93 <https://github.com/NASA-PDS/pds-registry-app/issues/93>`_ Research tech stack modifications due to large number of search fields in registry

--------

PDS.nasa.gov-Search
###################

*Front-end interface for PDS.nasa.gov data search capability*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/PDS.nasa.gov-Search#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/PDS.nasa.gov-Search>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PDS.nasa.gov-Search/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PDS.nasa.gov-Search/releases>`_ 

* `PDS.nasa.gov-Search#20 <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/20>`_ **Search Details Page / DOI Landing Page**
   * `PDS.nasa.gov-Search#26 <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/26>`_ Review search details / DOI page updates
* `PDS.nasa.gov-Search#21 <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/21>`_ **DOI Landing Page Requirements and Design**
   * `PDS.nasa.gov-Search#22 <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/22>`_ Develop DOI Landing Page Scope
   * `PDS.nasa.gov-Search#23 <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/23>`_ Revise requirements to meet scope
   * `PDS.nasa.gov-Search#24 <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/24>`_ Review scope and requirements with DOI WG
   * `PDS.nasa.gov-Search#25 <https://github.com/NASA-PDS/PDS.nasa.gov-Search/issues/25>`_ Develop more formalized design documentation

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

* `pds-api#31 <https://github.com/NASA-PDS/pds-api/issues/31>`_ **Streamline testing of API server implementation**
* `pds-api#17 <https://github.com/NASA-PDS/pds-api/issues/17>`_ **Response format conventions and parameter definition**
   * `pds-api#18 <https://github.com/NASA-PDS/pds-api/issues/18>`_ Refine format conventions defined by the API WG
   * `pds-api#19 <https://github.com/NASA-PDS/pds-api/issues/19>`_ Define default response fields
   * `pds-api#20 <https://github.com/NASA-PDS/pds-api/issues/20>`_ Define required response fields
   * `pds-api#21 <https://github.com/NASA-PDS/pds-api/issues/21>`_ Define response formatting for default vs "additional" metadata fields
   * `pds-api#22 <https://github.com/NASA-PDS/pds-api/issues/22>`_ Update API Spec with refined response format conventions and field definitions
   * `pds-api#23 <https://github.com/NASA-PDS/pds-api/issues/23>`_ Implement response format definition in API Service
* `pds-api#35 <https://github.com/NASA-PDS/pds-api/issues/35>`_ **Initial Federated API implementation**
* `pds-api#34 <https://github.com/NASA-PDS/pds-api/issues/34>`_ **Deploy PDS API v0 (beta) for beta testing**
   * `pds-api#32 <https://github.com/NASA-PDS/pds-api/issues/32>`_ Deploy PDS API v0 (beta) on pds-gamma test server
   * `pds-api#33 <https://github.com/NASA-PDS/pds-api/issues/33>`_ Update public PDS API Spec in Github
* `pds-api#30 <https://github.com/NASA-PDS/pds-api/issues/30>`_ **SwaggerHub CodeGen Server adaptation and integration how-tos**
   * `pds-api-pythonlib#1 <https://github.com/NASA-PDS/pds-api-pythonlib/issues/1>`_ Test and write a procedure to develop a python implementation from swaggerHub
   * `pds-api#26 <https://github.com/NASA-PDS/pds-api/issues/26>`_ Document basic adaptation capabilities from pds-api-service
* `pds-api#28 <https://github.com/NASA-PDS/pds-api/issues/28>`_ **DN Pilot API Project(s)**
   * `pds-api#16 <https://github.com/NASA-PDS/pds-api/issues/16>`_ Implement EN query of DN API service
   * `pds-api#26 <https://github.com/NASA-PDS/pds-api/issues/26>`_ Document basic adaptation capabilities from pds-api-service
   * `pds-api#27 <https://github.com/NASA-PDS/pds-api/issues/27>`_ Identify nodes and define scope for piloting pds-api-service adaptation
   * `pds-api#29 <https://github.com/NASA-PDS/pds-api/issues/29>`_ Implement EN query passing to DN search UI
* `pds-api#24 <https://github.com/NASA-PDS/pds-api/issues/24>`_ **Define PDS handling of enriched / supplemental metadata**
* `pds-api#25 <https://github.com/NASA-PDS/pds-api/issues/25>`_ **PDS API extension convention for discipline-specific search engines**
* `pds-api#15 <https://github.com/NASA-PDS/pds-api/issues/15>`_ **Query passing and search integration design**
* `pds-api#14 <https://github.com/NASA-PDS/pds-api/issues/14>`_ **Define intra-discipline (product-level) search scope**
* `pds-api#12 <https://github.com/NASA-PDS/pds-api/issues/12>`_ **Initial Query Syntax Lexer Implementation**
* `pds-api#7 <https://github.com/NASA-PDS/pds-api/issues/7>`_ **Initial discipline/node-specific search parameter definition**

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

* `pdsen-corral#16 <https://github.com/NASA-PDS/pdsen-corral/issues/16>`_ **Github Action and Documentation Generation Best Practices**
   * `nasa-pds.github.io#3 <https://github.com/NASA-PDS/nasa-pds.github.io/issues/3>`_ Update nasa-pds.github.io with software documentation best practices
   * `nasa-pds.github.io#4 <https://github.com/NASA-PDS/nasa-pds.github.io/issues/4>`_ Update nasa-pds.github.io with github action best practices
   * `pds-template-repo-python#2 <https://github.com/NASA-PDS/pds-template-repo-python/issues/2>`_ Define a PDS standard to manage version in python project
   * `pds-deep-archive#81 <https://github.com/NASA-PDS/pds-deep-archive/issues/81>`_ Update Github Actions for dev and ops releases
   * `pds-doi-service#94 <https://github.com/NASA-PDS/pds-doi-service/issues/94>`_ Update to use pds round-up github action
   * `roundup-action#1 <https://github.com/NASA-PDS/roundup-action/issues/1>`_ Add Java / Maven support
   * `pdsen-corral#24 <https://github.com/NASA-PDS/pdsen-corral/issues/24>`_ Re-evaluate generating requirements for -dev versions
   * `pds-template-repo-python#3 <https://github.com/NASA-PDS/pds-template-repo-python/issues/3>`_ Add the roundup action in the template
   * `validate#255 <https://github.com/NASA-PDS/validate/issues/255>`_ Retrofit validate CI to use roundup-action
   * `pds4-jparser#30 <https://github.com/NASA-PDS/pds4-jparser/issues/30>`_ Retrofit pds4-jparser CI to use roundup-action
   * `pds-registry-app#94 <https://github.com/NASA-PDS/pds-registry-app/issues/94>`_ Retrofit pds-registry-app CI to use roundup-action
* `pdsen-corral#23 <https://github.com/NASA-PDS/pdsen-corral/issues/23>`_ **AWS Continuous Deployment Implementation**
* `pdsen-corral#22 <https://github.com/NASA-PDS/pdsen-corral/issues/22>`_ **Integration with Test Rail**
* `pdsen-corral#20 <https://github.com/NASA-PDS/pdsen-corral/issues/20>`_ **AWS Continuous Deployment Strategy**

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

* `PDS.nasa.gov-UX#3 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/3>`_ **Formulate user stories for prototype**
   * `PDS.nasa.gov-UX#14 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/14>`_ Develop user personas based upon outputs from user interview synthesis
   * `PDS.nasa.gov-UX#58 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/58>`_ Propose users stories for selected subset of the user personnas
* `PDS.nasa.gov-UX#6 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/6>`_ **Model workflows and initial design directions**
* `PDS.nasa.gov-UX#8 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/8>`_ **Design mockups and develop Figma prototype**
   * `PDS.nasa.gov-UX#10 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/10>`_ Develop generic design and mockups for cross-node Material templates
   * `PDS.nasa.gov-UX#11 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/11>`_ Define component (footer/header) styles
* `PDS.nasa.gov-UX#41 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/41>`_ **Review Feedback Widget Design**
   * `PDS.nasa.gov-UX#38 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/38>`_ Re-evaluate the design of the Feedback widget
   * `PDS.nasa.gov-UX#40 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/40>`_ Re-visit Feedback Widget Content
   * `feedback-widget#10 <https://github.com/NASA-PDS/feedback-widget/issues/10>`_ Apply WDS to Widget
   * `pds-wds#11 <https://github.com/NASA-PDS/pds-wds/issues/11>`_ Implement Feedback Widget in React
* `PDS.nasa.gov-UX#47 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/47>`_ **Design System Documentation**
   * `pds-wds#1 <https://github.com/NASA-PDS/pds-wds/issues/1>`_ Show Text Field component that displays units
   * `pds-wds#2 <https://github.com/NASA-PDS/pds-wds/issues/2>`_ Add other organizational logos
   * `pds-wds#4 <https://github.com/NASA-PDS/pds-wds/issues/4>`_ Propagate PDS brand colors across all components in Figma
   * `pds-wds#6 <https://github.com/NASA-PDS/pds-wds/issues/6>`_ Define types of banner notifications
   * `pds-wds#8 <https://github.com/NASA-PDS/pds-wds/issues/8>`_ Document UI guidelines and rules
   * `pds-wds#9 <https://github.com/NASA-PDS/pds-wds/issues/9>`_ Restructure component organization in Figma
   * `PDS.nasa.gov-UX#54 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/54>`_ Relay for Figma (continuous delivery)
* `PDS.nasa.gov-UX#53 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/53>`_ **PDS Sitemap Generator**
   * `PDS.nasa.gov-UX#49 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/49>`_ Evaluate sitemap generator tools
   * `PDS.nasa.gov-UX#50 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/50>`_ Generate sitemap for pds.nasa.gov
   * `PDS.nasa.gov-UX#51 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/51>`_ Submit sitemap to Google Webmaster
   * `PDS.nasa.gov-UX#52 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/52>`_ Integrate Google Webmaster and sitemap generator with DNs
* `PDS.nasa.gov-UX#45 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/45>`_ **WDS Mobile Considerations**
* `PDS.nasa.gov-UX#35 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/35>`_ **Content Management System**
   * `PDS.nasa.gov-UX#36 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/36>`_ Abstract out the structure of PDS pages from CMS
   * `PDS.nasa.gov-UX#37 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/37>`_ Converge on a CMS solution
* `PDS.nasa.gov-UX#31 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/31>`_ **Formulate PDS Information Architecture**
   * `PDS.nasa.gov-UX#32 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/32>`_ Evaluate the current structure of PDS structure using mapping tools
   * `PDS.nasa.gov-UX#33 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/33>`_ Re-organize PDS web content based on business/user needs
   * `PDS.nasa.gov-UX#34 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/34>`_ Consolidate pages and ensure there is a logical structure to how we are organizing our sites
* `PDS.nasa.gov-UX#30 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/30>`_ **User Documentation Consolidation**
   * `PDS.nasa.gov-UX#28 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/28>`_ Document the information that is redundant across nodes
   * `PDS.nasa.gov-UX#29 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/29>`_ Consolidate PDS wide information in to a user guide
   * `pds-api#36 <https://github.com/NASA-PDS/pds-api/issues/36>`_ Propose PDS style for API documentation

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

* `pdsen-operations#14 <https://github.com/NASA-PDS/pdsen-operations/issues/14>`_ **LDD CCB and Management processes**
   * `pdsen-operations#15 <https://github.com/NASA-PDS/pdsen-operations/issues/15>`_ Work with LDD Stewards to develop process and CCB
   * `pdsen-operations#16 <https://github.com/NASA-PDS/pdsen-operations/issues/16>`_ Update LDD CI/CD accordingly to match the expectations from the CCB review process
   * `pdsen-operations#22 <https://github.com/NASA-PDS/pdsen-operations/issues/22>`_ Document how to tag an LDD Release

--------

pds-tracking-service
####################

*Provides functionality for tracking status and other aspects pertaining to PDS products that are not captured in the Registry Service.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-tracking-service#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-tracking-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-tracking-service/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-tracking-service/issues?q=is%3Aopen+is%3Aissue+label%3Abacklog>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-tracking-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-tracking-service/releases>`_ 

* `pds-tracking-service#1 <https://github.com/NASA-PDS/pds-tracking-service/issues/1>`_ **Open Source Tracking Service**
* `pds-tracking-service#6 <https://github.com/NASA-PDS/pds-tracking-service/issues/6>`_ **Refactor Tracking Service**
   * `pds-tracking-service#5 <https://github.com/NASA-PDS/pds-tracking-service/issues/5>`_ De-couple individual components
   * `pds-tracking-service#7 <https://github.com/NASA-PDS/pds-tracking-service/issues/7>`_ Deploy beta of individual components
   * `pds-tracking-service#8 <https://github.com/NASA-PDS/pds-tracking-service/issues/8>`_ Integrate DOI Tracking with DOI Service
* `pds-tracking-service#2 <https://github.com/NASA-PDS/pds-tracking-service/issues/2>`_ **Review Tracking Service Requirements and Design**
   * `pds-tracking-service#4 <https://github.com/NASA-PDS/pds-tracking-service/issues/4>`_ Identify implemented requirements


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
