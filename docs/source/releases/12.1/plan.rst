Build 12.1 Plan
========================

..  toctree::
    :glob:
    :maxdepth: 4

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
    * - 02/25/2022
      - SCR Freeze Date
      - DDWG
      - Freeze date for identifying SCRs to be implemented in this release.
    * - 04/21/2022
      - Standards Documents Updates Due
      - Document Authoring Team
      - Updates to PDS4 standards documents due to EN for review.
    * - 05/02/2022 - 05/20/2022
      - Beta Testing Period
      - DNs, IPDA
      - Changes to PDS4 IM and system components available for beta testing.
    * - 04/22/2022 - 05/20/2022
      - dLDD Integration and Test
      - dLDD Stewards
      - Auto-generated dLDDs should be reviews by dLDD Stewards, and final updates to dLDDs should be completed during this time.
    * - 05/10/2022
      - Standards Documents Review Due
      - Document Review Team
      - Review updates to PDS4 standards documents.
    * - 06/03/2022
      - System Release
      - EN
      - PDS4 system is operationally deployed and website is updated accordingly.

.. list-table:: Key Dates for Engineering Node
    :widths: 20 40 40
    :header-rows: 1

    * - Date
      - Name
      - Description
    * - 03/25/2022
      - Delivery to I&T
      - The PDS4 IM and all software updated during this 
        build cycle are delivered to EN I&T.
    * - 04/07/2022
      - Test Readiness Review (TRR)
      - PDS EN internal review to verify readiness to enter I&T phase.
    * - 05/23/2022
      - Delivery and Deployment Review (DRR)
      - PDS internal review with PDS Software Working Group to verify readiness to deploy build system.
    * - 06/03/2022
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

Data Stewardship Tools
----------------------

Validate
########

*Validates PDS4 product labels, data and PDS3 Volumes*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/validate/>`_
     - `Github Repo <https://github.com/NASA-PDS/validate>`_
     - `Issue Tracking <https://github.com/NASA-PDS/validate/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/validate/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/validate/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/validate/releases>`_ 

* `validate#407 <https://github.com/NASA-PDS/validate/issues/407>`_ **B12.1 Referential Integrity Improvements**
   * `validate#307 <https://github.com/NASA-PDS/validate/issues/307>`_ As a user, I want to validate that all XML Schema collections in NASA PDS archives are secondary collections
* `validate#409 <https://github.com/NASA-PDS/validate/issues/409>`_ **B12.1 PDF/A Handling Improvements**
   * `validate#388 <https://github.com/NASA-PDS/validate/issues/388>`_ Improve PDF/A validation to include more robust reporting on failures
   * `validate#412 <https://github.com/NASA-PDS/validate/issues/412>`_ Update PDF validation to check against flavour specified in PDF metadata
* `validate#414 <https://github.com/NASA-PDS/validate/issues/414>`_ **Referential Integrity Checking with the Registry**
   * `validate#415 <https://github.com/NASA-PDS/validate/issues/415>`_ As a user, I want to perform referential integrity checking against a registry
* `validate#422 <https://github.com/NASA-PDS/validate/issues/422>`_ **B12.1 Re-imagine Output Logging for Validity vs Metadata Quality**
* `validate#426 <https://github.com/NASA-PDS/validate/issues/426>`_ **B12.1 Content Validation Improvements**
   * `validate#423 <https://github.com/NASA-PDS/validate/issues/423>`_ Validate does not allow a single-character subdirectory
   * `validate#424 <https://github.com/NASA-PDS/validate/issues/424>`_ Validate does not allow SIP tab file to have lines of differing lengths
   * `validate#425 <https://github.com/NASA-PDS/validate/issues/425>`_ Refactor content validation to more robustly handle intermingled Headers

--------

LDDTool and PDS4 Information Model
##################################

*The software tools and data necessary for generating the Information Model including PDS4 ontology, data, and information model.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-information-model/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-information-model>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-information-model/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds4-information-model/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-information-model/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-information-model/releases>`_ 

* `pds4-information-model#306 <https://github.com/NASA-PDS/pds4-information-model/issues/306>`_ **Refactoring of IMTool**
   * `pds4-information-model#239 <https://github.com/NASA-PDS/pds4-information-model/issues/239>`_ Refactor Class information from config to Data Dictionary Protege ontology
   * `pds4-information-model#281 <https://github.com/NASA-PDS/pds4-information-model/issues/281>`_ Tag ops classes/attributes in IM so they are easily identifiable by users
* `pds4-information-model#356 <https://github.com/NASA-PDS/pds4-information-model/issues/356>`_ **Kick-off PDS4 Information Model in GraphDB**
   * `pds4-information-model#357 <https://github.com/NASA-PDS/pds4-information-model/issues/357>`_ Ingest PDS4 IM into BlazeGraph
   * `pds4-information-model#358 <https://github.com/NASA-PDS/pds4-information-model/issues/358>`_ Replicate diagram from PDS4 IM Spec
   * `pds4-information-model#359 <https://github.com/NASA-PDS/pds4-information-model/issues/359>`_ Deploy new Amazon Neptune instance for PDS4 IM prototype
   * `pds4-information-model#387 <https://github.com/NASA-PDS/pds4-information-model/issues/387>`_ As an operator, I want to be able to convert from XML to RDF using the PDS4 Information Model
* `pds4-information-model#410 <https://github.com/NASA-PDS/pds4-information-model/issues/410>`_ **B12.1 LDDTool / PDS4 IM Documentation Updates**

--------

PDS Deep Archive
################

*PDS Open Archival Information System (OAIS) utilities, including Submission Information Package (SIP) and Archive Information Package (AIP) generators*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-deep-archive/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-deep-archive>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-deep-archive/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-deep-archive/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-deep-archive/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-deep-archive/releases>`_ 

* `pds-deep-archive#115 <https://github.com/NASA-PDS/pds-deep-archive/issues/115>`_ **Revisit PDS Deep Archive Integration with Registry**
   * `pds-deep-archive#107 <https://github.com/NASA-PDS/pds-deep-archive/issues/107>`_ Update PDS Deep "Registry" Archive and remove workaround + implement latest-only-feature per API updates

--------

DOI Services
------------

PDS DOI Service
###############

*Service and tools for generating DOIs for PDS bundles, collections, and data sets*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-doi-service>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-doi-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-doi-service/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-doi-service/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-doi-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-doi-service/releases>`_ 

* `pds-doi-service#251 <https://github.com/NASA-PDS/pds-doi-service/issues/251>`_ **B12.1 Enhancements to PDS DOI Metadata**
   * `pds-doi-service#102 <https://github.com/NASA-PDS/pds-doi-service/issues/102>`_ Add new alternateIdentifier to match SBN schema
   * `pds-doi-service#224 <https://github.com/NASA-PDS/pds-doi-service/issues/224>`_ As a user, I would like to include licensing information with all PDS DOIs
   * `pds-doi-service#282 <https://github.com/NASA-PDS/pds-doi-service/issues/282>`_ Improve metadata based upon parameters ADS keys off of
   * `pds-doi-service#283 <https://github.com/NASA-PDS/pds-doi-service/issues/283>`_ As a publisher, I want to be notified when a new DOI has been minted or significant update to the metadata
* `pds-doi-service#252 <https://github.com/NASA-PDS/pds-doi-service/issues/252>`_ **B12.1 Enhancements to DOI Search Component**
   * `pds-doi-ui#61 <https://github.com/NASA-PDS/pds-doi-ui/issues/61>`_ As a PDS.nasa.gov user, I want to search for the DOI for a PDS4 data product from a public facing website (pds.nasa.gov)
   * `pds-doi-ui#83 <https://github.com/NASA-PDS/pds-doi-ui/issues/83>`_ Combine NPM Package And Embeddable JS Script Toolchains
   * `pds-wds-react#4 <https://github.com/NASA-PDS/pds-wds-react/issues/4>`_ Add Search DOI Component
   * `pds-doi-ui#88 <https://github.com/NASA-PDS/pds-doi-ui/issues/88>`_ Pre-existing keyword show i a weird way in the UI
* `pds-doi-service#270 <https://github.com/NASA-PDS/pds-doi-service/issues/270>`_ **B12.1 DOI Metadata and Update Functionality Improvements**
   * `pds-doi-service#257 <https://github.com/NASA-PDS/pds-doi-service/issues/257>`_ As a PDS Operator, I want to perform a bulk update of a specific field across many DOI records
   * `pds-doi-service#278 <https://github.com/NASA-PDS/pds-doi-service/issues/278>`_ As a user, I want to update the LIDVID associated with a DOI 

--------

PDS DOI UI
##########

*web UI for pds-doi-service*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-doi-ui#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-doi-ui>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-doi-ui/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-doi-ui/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-doi-ui/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-doi-ui/releases>`_ 

* `pds-doi-ui#60 <https://github.com/NASA-PDS/pds-doi-ui/issues/60>`_ **DOI Search Component**

--------

Registry + API Services
-----------------------

PDS Registry App
################

*Registry application enabling a PDS node to register all its data products for long term preservation and sharing with the rest of the PDS system.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-registry-app/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-registry-app>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-registry-app/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-registry-app/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-registry-app/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-registry-app/releases>`_ 

* `pds-registry-app#184 <https://github.com/NASA-PDS/pds-registry-app/issues/184>`_ **B12.1 Registry Tools Performance Improvements**
   * `pds-registry-app#179 <https://github.com/NASA-PDS/pds-registry-app/issues/179>`_ As a user, I want the registry app components to be able to ingest data sets containing 1+ million products
   * `pds-registry-mgr-elastic#31 <https://github.com/NASA-PDS/pds-registry-mgr-elastic/issues/31>`_ Update registy-mgr to use schema from schemaLocation in file
   * `pds-registry-app#195 <https://github.com/NASA-PDS/pds-registry-app/issues/195>`_ Big Data Harvest analysis / POC
   * `pds-registry-app#200 <https://github.com/NASA-PDS/pds-registry-app/issues/200>`_ As a user, I want big data ingestion tools packaged and dockerized together
* `pds-registry-app#190 <https://github.com/NASA-PDS/pds-registry-app/issues/190>`_ **Support Staging vs. Operational Data**
   * `pds-api#106 <https://github.com/NASA-PDS/pds-api/issues/106>`_ As a API manager, I want to restrict access to registered products that should not be publicly accessible
   * `pds-registry-app#201 <https://github.com/NASA-PDS/pds-registry-app/issues/201>`_ As a user, I want to be able to ingest a set of files specified in a file listing
* `pds-registry-app#191 <https://github.com/NASA-PDS/pds-registry-app/issues/191>`_ **B12.1 Initial external source integration**
   * `pds-registry-app#176 <https://github.com/NASA-PDS/pds-registry-app/issues/176>`_ As a registry user, I want to ingest supplemental metadata from external data sources
   * `pds-api#90 <https://github.com/NASA-PDS/pds-api/issues/90>`_ As an API user, I want to search for registered supplemental metadata ingested from external data sources
* `pds-registry-app#194 <https://github.com/NASA-PDS/pds-registry-app/issues/194>`_ **Populate EN Registry**
   * `pds-registry-app#192 <https://github.com/NASA-PDS/pds-registry-app/issues/192>`_ As a user, I want to ingest legacy PDS3 data sets
   * `pds-registry-app#193 <https://github.com/NASA-PDS/pds-registry-app/issues/193>`_ Deploy harvest / registry-mgr as cron to regularly upload PDS EN data to registry
* `pds-registry-app#199 <https://github.com/NASA-PDS/pds-registry-app/issues/199>`_ **Dockerize Registry Components for Dev and Ops Deployments**

--------

PDS API
#######

*PDS API Application with client and server integrated into one package*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-api/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api/releases>`_ 

* `pds-api#114 <https://github.com/NASA-PDS/pds-api/issues/114>`_ **Improve PDS API Development Workflow and Versioning**
   * `pds-api#122 <https://github.com/NASA-PDS/pds-api/issues/122>`_ analysis of current workflow, ideas for improvment
   * `pds-api#123 <https://github.com/NASA-PDS/pds-api/issues/123>`_ create a super registry+api repository
* `pds-api#117 <https://github.com/NASA-PDS/pds-api/issues/117>`_ **[pds-api] B12.1 API Response Improvements**
   * `pds-api#45 <https://github.com/NASA-PDS/pds-api/issues/45>`_ As a user, I want the API to be schema.org compliant
   * `pds-api#65 <https://github.com/NASA-PDS/pds-api/issues/65>`_ As an API user, I want to get only the fields I explicitly requested
   * `pds-api#66 <https://github.com/NASA-PDS/pds-api/issues/66>`_ As an API user, I want to get an XML response
   * `pds-api#68 <https://github.com/NASA-PDS/pds-api/issues/68>`_ As an API user, I want to know in the response how many hits are returned for an API query.
   * `registry-api-service#33 <https://github.com/NASA-PDS/registry-api-service/issues/33>`_ As a user, I want  to get a 404 error when I attempt to request a resource which does not exists
   * `pds-api#88 <https://github.com/NASA-PDS/pds-api/issues/88>`_ As a user,I want to get the list of properties available in summary sorted in alphabetical order
   * `pds-api#89 <https://github.com/NASA-PDS/pds-api/issues/89>`_ As a user, I want to know the DOI associated with a product
   * `pds-api#110 <https://github.com/NASA-PDS/pds-api/issues/110>`_ Extend application/pds4+json support to all endpoints
   * `pds-api#118 <https://github.com/NASA-PDS/pds-api/issues/118>`_ As an API user, I want to receive a HTML response
   * `pds-api#120 <https://github.com/NASA-PDS/pds-api/issues/120>`_ As an API user, I want a CSV response format option
   * `pds-api#125 <https://github.com/NASA-PDS/pds-api/issues/125>`_ As a user, I want to get the PDS4 original XML label
   * `pds-api#127 <https://github.com/NASA-PDS/pds-api/issues/127>`_ As a user, I want to clearly see which formats are accepted by the API

--------

PDS Web Modernization and Unification
-------------------------------------

PDS Web Design
#####################

*PDS.nasa.gov User Experience Task Issue and Prototype repository*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/PDS.nasa.gov-UX#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/PDS.nasa.gov-UX>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PDS.nasa.gov-UX/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PDS.nasa.gov-UX/releases>`_ 

* `PDS.nasa.gov-UX#100 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/100>`_ **B12.1 Continuation of User Persona and User Story Development**
   * `PDS.nasa.gov-UX#99 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/99>`_ Document initial User Stories using WMWG feedback 
   * `PDS.nasa.gov-UX#103 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/103>`_ Iterate on WMWG feedback
   * `PDS.nasa.gov-UX#107 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/107>`_ Tag user stories to modules and templates
* `PDS.nasa.gov-UX#101 <https://github.com/NASA-PDS/PDS.nasa.gov-UX/issues/101>`_ **Deploy new Citing PDS Data Web Pages**

--------

PDS Web Implementation
######################

*PDS Web Implementation Team assessing and prioritizing the unification of the PDS web presence.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-web-mgmt#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-web-mgmt>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-web-mgmt/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-web-mgmt/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-web-mgmt/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-web-mgmt/releases>`_ 

* `pds-web-mgmt#1 <https://github.com/NASA-PDS/pds-web-mgmt/issues/1>`_ **Initial Assessment of Today’s Web Management Landscape**
* `pds-web-mgmt#2 <https://github.com/NASA-PDS/pds-web-mgmt/issues/2>`_ **Preliminary Design of Migration**
* `pds-web-mgmt#3 <https://github.com/NASA-PDS/pds-web-mgmt/issues/3>`_ **High level Implementation Plan**

--------

Cloud Strategy and Services
---------------------------

*PDS Cloud Migration documentation, issue, tracking and simple tools for assisting in the PDS hybrid cloud study and migration efforts.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/cloud-strategy#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/cloud-strategy>`_
     - `Issue Tracking <https://github.com/NASA-PDS/cloud-strategy/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/cloud-strategy/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/cloud-strategy/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/cloud-strategy/releases>`_ 

* `cloud-strategy#3 <https://github.com/NASA-PDS/cloud-strategy/issues/3>`_ **B12.1 pds.nasa.gov Website Lift-and-Shift Pilot Project**
   * `cloud-strategy#9 <https://github.com/NASA-PDS/cloud-strategy/issues/9>`_ AWS testing for PDS and PDS Engineering sites
* `cloud-strategy#4 <https://github.com/NASA-PDS/cloud-strategy/issues/4>`_ **B12.1 pds-engineering.nasa.gov Website Lift-and-Shift Pilot Project**
   * `cloud-strategy#9 <https://github.com/NASA-PDS/cloud-strategy/issues/9>`_ AWS testing for PDS and PDS Engineering sites
* `cloud-strategy#5 <https://github.com/NASA-PDS/cloud-strategy/issues/5>`_ **B12.1 NAIF.nasa.gov Website Lift-and-Shift Pilot Project**
* `cloud-strategy#6 <https://github.com/NASA-PDS/cloud-strategy/issues/6>`_ **B12.1 pds-imaging.jpl.nasa.gov Website Lift-and-Shift Pilot Project**
* `cloud-strategy#7 <https://github.com/NASA-PDS/cloud-strategy/issues/7>`_ **B12.1 Refine AWS Registry Deployment Strategy**
   * `pds-registry-app#87 <https://github.com/NASA-PDS/pds-registry-app/issues/87>`_ Deploy GEO Registry in AWS
   * `pds-registry-app#88 <https://github.com/NASA-PDS/pds-registry-app/issues/88>`_ Deploy IMG Registry in AWS
   * `pds-registry-app#89 <https://github.com/NASA-PDS/pds-registry-app/issues/89>`_ Document AWS deployment for Registry
   * `pds-registry-app#90 <https://github.com/NASA-PDS/pds-registry-app/issues/90>`_ Develop cost model and reporting for Registry deployments
   * `pds-doi-service#164 <https://github.com/NASA-PDS/pds-doi-service/issues/164>`_ Develop AWS deployment architecture and test deployment for DOI Service
   * `cloud-strategy#1 <https://github.com/NASA-PDS/cloud-strategy/issues/1>`_ As a manager, I want a cost monitoring capability for AWS deployments
   * `registry-api-service#22 <https://github.com/NASA-PDS/registry-api-service/issues/22>`_ Work w/ SAs to define production deployment strategy in AWS
   * `registry-api-service#78 <https://github.com/NASA-PDS/registry-api-service/issues/78>`_ Add aws cost tagging and secret/parameter creation to ECS terraform script
* `cloud-strategy#8 <https://github.com/NASA-PDS/cloud-strategy/issues/8>`_ **Develop Roadmap and Cost Model for PDS Cloud**
* `cloud-strategy#10 <https://github.com/NASA-PDS/cloud-strategy/issues/10>`_ **PDS-ESDIS NGAP Pilot Project**

--------

Nucleus
-------

*Pipeline for automated, streamlined deployment and execution of PDS validation, ingestion, and transformation services.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/nucleus#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/nucleus>`_
     - `Issue Tracking <https://github.com/NASA-PDS/nucleus/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/nucleus/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/nucleus/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/nucleus/releases>`_ 

* `nucleus#1 <https://github.com/NASA-PDS/nucleus/issues/1>`_ **B12.1 Initial Design and Trade Study**
* `nucleus#2 <https://github.com/NASA-PDS/nucleus/issues/2>`_ **Initial Implementation**

--------

Other EN Internal Plans
-----------------------

PDS Github Util
###############

*github utility functions to enforce the PDS engineering node software life cycle.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-github-util>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-github-util>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-github-util/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/pds-github-util/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-github-util/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-github-util/releases>`_ 

* `pds-github-util#47 <https://github.com/NASA-PDS/pds-github-util/issues/47>`_ **B12.1 Software Release Documentation Updates**
   * `pds-github-util#14 <https://github.com/NASA-PDS/pds-github-util/issues/14>`_ As a user, I want to see the status of the tickets shown in the current build plan

--------

Systems Engineering
###################

*Issue tracking repository as a centralized entry point for general PDS software bugs and feature requests.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/PDS-Software-Issues-Repo#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/PDS-Software-Issues-Repo>`_
     - `Issue Tracking <https://github.com/NASA-PDS/PDS-Software-Issues-Repo/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/PDS-Software-Issues-Repo/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/PDS-Software-Issues-Repo/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/PDS-Software-Issues-Repo/releases>`_ 

* `PDS-Software-Issues-Repo#14 <https://github.com/NASA-PDS/PDS-Software-Issues-Repo/issues/14>`_ **B12.0 Prep for I&T**
   * `PDS-Software-Issues-Repo#15 <https://github.com/NASA-PDS/PDS-Software-Issues-Repo/issues/15>`_ Generate Draft B12.0 RDD
   * `PDS-Software-Issues-Repo#16 <https://github.com/NASA-PDS/PDS-Software-Issues-Repo/issues/16>`_ Final testing and delivery to I&T
* `PDS-Software-Issues-Repo#17 <https://github.com/NASA-PDS/PDS-Software-Issues-Repo/issues/17>`_ **B12.1 Generate Release Plan**

--------

DevOps
######

*Parent repo for PDS DevOps activities*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/devops#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/devops>`_
     - `Issue Tracking <https://github.com/NASA-PDS/devops/issues>`_ 
     - `Backlog <https://github.com/NASA-PDS/devops/issues?q=is%3Aopen+is%3Aissue+label%3Aicebox>`_ 
     - `Stable Release <https://github.com/NASA-PDS/devops/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/devops/releases>`_ 

* `devops#13 <https://github.com/NASA-PDS/devops/issues/13>`_ **Continuous improvements to Continuous Integration**
   * `pds-registry-app#177 <https://github.com/NASA-PDS/pds-registry-app/issues/177>`_ stable continuous integration don't generate the packages tar.gz and .zip properly.
   * `devops#10 <https://github.com/NASA-PDS/devops/issues/10>`_ Rollout template updates to existing repos
   * `roundup-action#67 <https://github.com/NASA-PDS/roundup-action/issues/67>`_ Roundup's Python Environment Should Be Separate from the Packages It Builds
   * `devops#12 <https://github.com/NASA-PDS/devops/issues/12>`_ Remove Versioneer
   * `devops#14 <https://github.com/NASA-PDS/devops/issues/14>`_ Update Stable Major Releases of PDS software with DOIs
   * `devops#15 <https://github.com/NASA-PDS/devops/issues/15>`_ Update stable releases to handle Java repos
   * `roundup-action#69 <https://github.com/NASA-PDS/roundup-action/issues/69>`_ Roundup handling VERSION.txt
   * `pds-github-util#48 <https://github.com/NASA-PDS/pds-github-util/issues/48>`_ Versions seem to be not incrementing correctly for python unstable releases

--------


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