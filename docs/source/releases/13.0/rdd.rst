==========================================
Release Description Document (Build B13.0)
==========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B13.0`_

The following sections can be found in this document:

.. toctree::
   :glob: 
   :maxdepth: 3

   rdd.rst

PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Board
and implemented by the PDS within the latest build period.

+--------------------------------+----------------------------------------------------------+
|Ref                             |Title                                                     |
+================================+==========================================================+
|`pds4-information-model#499`_   |CCB-348: Add Units_of_Mass_Density as a unit of measure   |
+--------------------------------+----------------------------------------------------------+

Software Changes
================
The changes types are 'Bug', 'Enhancement' or 'Requirement'. For each software repository, the changes are listed in 2
categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B13.0`_')
The 'Other Updates' occurs during the build cycle witout being planned or attached to a theme. They are organized by
types (bug, enhancements, requirements...). Any updates that require a de-scope of planned tasks are reviewed by the PDS
Software Working Group.

The deliveries are validated by the development team and go through an additional Integration & Test process, as
applicable, as indicated by a specific icon in the following tables.

--------

Cloud Tasks
-----------
*PDS Cloud Migration documentation, issue, tracking and simple tools for assisting in the PDS hybrid cloud study and migration efforts.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/cloud-tasks#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/cloud-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/cloud-tasks/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/cloud-tasks/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/cloud-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/cloud-tasks/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`cloud-tasks#28`_ B13.0 Upgrade Registry Deployments to OpenSearch
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                                                                     |I&T   |Priority / Bug Severity   |
+==========================================================================================================================+======+==========================+
|`cloud-tasks#37`_ Make the current version of the API implementation (v1.0) be published under url 1.0 (instead of 0.4)   |      |unknown                   |
+--------------------------------------------------------------------------------------------------------------------------+------+--------------------------+

--------

PDS Design Team and Web Modernization
-------------------------------------
*PDS.nasa.gov User Experience Task Issue and Prototype repository*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/design-team#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/design-team>`_
     - `Issue Tracking <https://github.com/NASA-PDS/design-team/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/design-team/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/design-team/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/design-team/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`design-team#138`_ Continue High-Fidelity User Journey Designs: Homepage, Search, Mission Portal
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                                                          |I&T   |Level   |Priority / Bug Severity   |
+===============================================================================================+======+========+==========================+
|`design-team#129`_ Design Investigations Portal high-fidelity designs (draft 1)                |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`design-team#130`_ Develop high-fidelity design for data / web search journey (draft 1)        |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`design-team#132`_ High-fidelity design for PDS Homepage                                       |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`design-team#135`_ Develop discipline node high fidelity design for GEO (draft 1)              |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`design-team#136`_ Develop data set landing page high-fidelity designs (draft 1)               |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`design-team#141`_ Design Investigations Portal high-fidelity designs (draft 2)                |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`design-team#143`_ Develop high-fidelity designs for data / web search journey (draft 2)       |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`design-team#152`_ Make the Investigation page for Cassini                                     |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`design-team#153`_ Iterate on MSL Investigations landing high-fidelity designs (draft 3)       |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+
|`design-team#154`_ Iterate on Cassini Investigations landing high-fidelity designs (draft 2)   |      |task    |unknown                   |
+-----------------------------------------------------------------------------------------------+------+--------+--------------------------+


`design-team#139`_ Refine WDS based upon High-Fidelity Designs 
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`design-team#140`_ Usability Testing Phase 1 - Introduction
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

--------

Devops
------
*Parent repo for PDS DevOps activities*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/devops#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/devops>`_
     - `Issue Tracking <https://github.com/NASA-PDS/devops/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/devops/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/devops/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/devops/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`devops#11`_ B13.0 Implement Continuous Deployment Strategy
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                                 |I&T       |Level         |Priority / Bug Severity   |
+======================================================================================================================+==========+==============+==========================+
|`devops#2`_ As a developer, I want a developer staging system with the latest dev versions of PDS services deployed   ||iandt|   |requirement   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`devops#22`_ As a developer, I want access to the latest and continuously deployed exposition API                     ||iandt|   |requirement   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                    |I&T   |Priority / Bug Severity   |
+=========================================================================+======+==========================+
|`devops#24`_ Automatic image creation needs to parameterize Dockerfile   |      |s.low                     |
+-------------------------------------------------------------------------+------+--------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                |I&T       |Priority / Bug Severity   |
+=====================================================================================================================+==========+==========================+
|`devops#27`_ As a developer, I want to have a documentation for the Continuous Deployment in the DEV STAGING venue   ||iandt|   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

DOI Service
-----------
*Service and tools for generating DOIs for PDS bundles, collections, and data sets*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/doi-service>`_
     - `Github Repo <https://github.com/NASA-PDS/doi-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/doi-service/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/doi-service/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/doi-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/doi-service/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                              |I&T       |Priority / Bug Severity   |
+===================================================================================================================+==========+==========================+
|`doi-service#341`_ Fix broken build                                                                                |          |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#350`_ dataCite reserve error on title                                                                 ||iandt|   |s.critical                |
+-------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#331`_ doi sync failing for SBN-PSI DOIs                                                               ||iandt|   |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#336`_ DOI-service application inaccurately reports LID as being invalid                               ||iandt|   |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#328`_ Valid PDS4 xml input is converted into an invalid json that fails internal datacite validator   ||iandt|   |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                          |I&T       |Priority / Bug Severity   |
+===============================================================================================================+==========+==========================+
|`doi-service#13`_ The software shall validate the DOI metadata when reserving, releasing, or updating a DOI.   ||iandt|   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#224`_ As a DOI user, I would like to know the licensing information PDS data                      ||iandt|   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#335`_ As a DOI user, I would like to know the copyright for PDS data                              ||iandt|   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-service#344`_ As a user, I want to release a DOI with a label that does not contain the DOI               ||iandt|   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

DOI User Interface
------------------
*The web interface for the PDS DOI Service providing the ability management PDS archive DOIs. See the DOI Service for more details on the available capabilities. https://nasa-pds.github.io/doi-service/*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/doi-ui#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/doi-ui>`_
     - `Issue Tracking <https://github.com/NASA-PDS/doi-ui/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/doi-ui/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/doi-ui/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/doi-ui/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                    |I&T       |Priority / Bug Severity   |
+=========================================================================================================+==========+==========================+
|`doi-ui#137`_ [SECURITY] Triage and determine severity of dependabot and code scanning vulnerabilities   |          |s.medium                  |
+---------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#151`_ Error messages are inconsistent                                                            ||iandt|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#130`_ Remove vulnerabilities from the package per npm audit                                      ||iandt|   |s.high                    |
+---------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#160`_ Sometimes there is a null error message when there is no error                             ||iandt|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#155`_ Keywords text box and info icon do not appear correctly                                    ||iandt|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                             |I&T       |Priority / Bug Severity   |
+==================================================================================================================+==========+==========================+
|`doi-ui#92`_ As a user, I want to get an error message with support contact when the backend API is unavailable   ||iandt|   |p.could-have              |
+------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#145`_ As a user, I want to access the DOI UI from outside JPL                                             ||iandt|   |p.must-have               |
+------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                         |I&T       |Priority / Bug Severity   |
+==============================================================================+==========+==========================+
|`doi-ui#149`_ create an ASR for the application                               ||iandt|   |unknown                   |
+------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#143`_ Deploy doi-ui in production on AWS                              |          |unknown                   |
+------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#146`_ Upgrade deployment of DOI UI to patched v1.0.1                  |          |unknown                   |
+------------------------------------------------------------------------------+----------+--------------------------+
|`doi-ui#147`_ Replace authentication with Cognito on DOI UI and DOI service   ||iandt|   |unknown                   |
+------------------------------------------------------------------------------+----------+--------------------------+

--------

Harvest
-------
*Standalone Harvest client application providing the functionality for capturing and indexing product metadata into the PDS Registry system (https://github.com/nasa-pds/registry).*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/harvest>`_
     - `Issue Tracking <https://github.com/NASA-PDS/harvest/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/harvest/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/harvest/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/harvest/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                            |I&T       |Priority / Bug Severity   |
+=================================================================================================+==========+==========================+
|`harvest#90`_ Incorrect "lidvid" and  "_id" fields are ingested (trailing zeros are truncated)   ||iandt|   |s.critical                |
+-------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Nucleus
-------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/nucleus#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/nucleus>`_
     - `Issue Tracking <https://github.com/NASA-PDS/nucleus/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/nucleus/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/nucleus/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/nucleus/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`nucleus#1`_ B13.0 Initial Design and Trade Study
+++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

--------

Pds-api
-------
*PDS API Application with client and server integrated into one package*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <http://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-api/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/pds-api/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-api/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`pds-api#129`_ Prep for API v1.0 Release
++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                  |I&T       |Level         |Priority / Bug Severity   |
+=======================================================================+==========+==============+==========================+
|`pds-api#169`_ As a user, I want to have a PDS Search API user guide   ||iandt|   |requirement   |p.must-have               |
+-----------------------------------------------------------------------+----------+--------------+--------------------------+


+----------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                             |I&T       |Level         |Priority / Bug Severity   |
+==================================================================================+==========+==============+==========================+
|`pds-api#173`_ Replace summary-only=true by limit=0                               ||iandt|   |enhancement   |unknown                   |
+----------------------------------------------------------------------------------+----------+--------------+--------------------------+
|`pds-api#202`_ Complete refactoring per API WG discussion on end-point redesign   |          |enhancement   |p.must-have               |
+----------------------------------------------------------------------------------+----------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                        |I&T   |Priority / Bug Severity   |
+=============================================================================+======+==========================+
|`pds-api#209`_ clarifications needed for fields reference in documentation   |      |s.low                     |
+-----------------------------------------------------------------------------+------+--------------------------+
|`pds-api#206`_ fix broken link in API docs                                   |      |s.low                     |
+-----------------------------------------------------------------------------+------+--------------------------+
|`pds-api#216`_ is "bites" a typo for "bytes" or "bits"?                      |      |s.low                     |
+-----------------------------------------------------------------------------+------+--------------------------+

Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                                                   |I&T       |Priority / Bug Severity   |
+========================================================================================================================================================+==========+==========================+
|`pds-api#148`_ As a user, I want to search for past versions of a product where the LID changed during the product history                              ||iandt|   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#60`_ As an API user, I want to know the Bundle for a given Product.                                                                            ||iandt|   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#101`_ As a user, I want to receive a JSON response that contains the PDS4 label metadata in JSON format (application/vnd.nasa.pds.pds4+json)   ||iandt|   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#125`_ As a user, I want to receive a XML response that contains the PDS4 label metadata in XML format (application/vnd.nasa.pds.pds4+xml)      ||iandt|   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#191`_ As a user, I want to get directions whenever I arrive on an API URL                                                                      ||iandt|   |p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                     |I&T       |Priority / Bug Severity   |
+==========================================================================================+==========+==========================+
|`pds-api#183`_ Create a cookbook page on the content negotiation for the PDS Search API   ||iandt|   |p.should-have             |
+------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#189`_ Update README to reflect best practices of other PDS repositories          |          |p.must-have               |
+------------------------------------------------------------------------------------------+----------+--------------------------+
|`pds-api#172`_ Create user guide for the search api                                       ||iandt|   |p.should-have             |
+------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Pds4-information-model
----------------------
*The software tools and data necessary for generating the Information Model including PDS4 ontology, data, and information model.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-information-model/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-information-model>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-information-model/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/pds4-information-model/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-information-model/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-information-model/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                      |I&T       |Priority / Bug Severity   |
+===========================================================================================================+==========+==========================+
|`pds4-information-model#468`_ LDDTool is generating multiple Schematron rules to test the same condition   ||iandt|   |s.medium                  |
+-----------------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                   |I&T       |Priority / Bug Severity   |
+========================================================================================+==========+==========================+
|`pds4-information-model#499`_ CCB-348: Add Units_of_Mass_Density as a unit of measure   ||iandt|   |p.must-have               |
+----------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                      |I&T   |Priority / Bug Severity   |
+===========================================================================+======+==========================+
|`pds4-information-model#460`_ [namespace-registry] move namespace "wave"   |      |p.must-have               |
+---------------------------------------------------------------------------+------+--------------------------+

--------

Planetarydata.org
-----------------
*Website and related services for the International Planetary Data Alliance, nominally run at https://planetarydata.org/*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/planetarydata.org#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/planetarydata.org>`_
     - `Issue Tracking <https://github.com/NASA-PDS/planetarydata.org/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/planetarydata.org/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/planetarydata.org/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/planetarydata.org/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------+----------+--------------------------+
|Issue                                                  |I&T       |Priority / Bug Severity   |
+=======================================================+==========+==========================+
|`planetarydata.org#6`_ IPDA Charter blocked by login   ||iandt|   |s.medium                  |
+-------------------------------------------------------+----------+--------------------------+

--------

Portal-tasks
------------
*PDS Portal tasks repo used to track update requests for the website. Actual code and website are managed in separate private repo*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://pds.nasa.gov>`_
     - `Github Repo <https://github.com/NASA-PDS/portal-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/portal-tasks/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/portal-tasks/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/portal-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/portal-tasks/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`portal-tasks#35`_ Initial Migration of PDS.nasa.gov to New CMS
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                 |I&T       |Priority / Bug Severity   |
+======================================================================================+==========+==========================+
|`portal-tasks#38`_ fix filenames for CASSINI_1B00_1300 in online archive              ||iandt|   |s.medium                  |
+--------------------------------------------------------------------------------------+----------+--------------------------+
|`portal-tasks#22`_ Fix odd spacing in header for keyword search and data set status   ||iandt|   |s.medium                  |
+--------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                                                       |I&T   |Priority / Bug Severity   |
+============================================================================================================+======+==========================+
|`portal-tasks#26`_ As a node user, I want guidelines for handling DOI metadata for accumulating data sets   |      |p.should-have             |
+------------------------------------------------------------------------------------------------------------+------+--------------------------+

--------

Registry
--------
*PDS Registry provides service and software application necessary for tracking, searching, auditing, locating, and maintaining artifacts within the system. These artifacts can range from data files and label files, schemas, dictionary definitions for objects and elements, services, etc.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/registry>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`registry#55`_ Re-imagine Registry Handling of Product Versioning
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------------------+------+--------+--------------------------+
|Issue                                                                                           |I&T   |Level   |Priority / Bug Severity   |
+================================================================================================+======+========+==========================+
|`registry#57`_ Design the PDS4 definition for describing superseded LIDs via product metadata   |      |task    |unknown                   |
+------------------------------------------------------------------------------------------------+------+--------+--------------------------+


`registry#45`_ Preparations to Support B12.1 Registry Upgrades
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                         |I&T       |Priority / Bug Severity   |
+==============================================================================================+==========+==========================+
|`registry#64`_ Scalable Harvest does not replace file paths with the appropriate URL prefix   ||iandt|   |s.high                    |
+----------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry#84`_ Missing INSIGHT LDD v1600                                                      |          |s.low                     |
+----------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                             |I&T       |Priority / Bug Severity   |
+==================================================================================================================+==========+==========================+
|`registry#67`_ As a registry node user from JPL, I want to use my JPL login to access the Registry's OpenSearch   ||iandt|   |p.should-have             |
+------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Registry-api
------------
*Web API service for the PDS Registry, providing the implementation of the PDS Search API (https://github.com/nasa-pds/pds-api) for the PDS Registry.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-api>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-api>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-api/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-api/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-api/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-api/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`registry-api#138`_ Response Metadata Improvements
++++++++++++++++++++++++++++++++++++++++++++++++++
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                                                                    |I&T       |Priority / Bug Severity   |
+=========================================================================================================================================================================+==========+==========================+
|`registry-api#134`_ wildcard search in query parameter returning odd results                                                                                             ||iandt|   |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#121`_ Fix vulnerabilities raised by sonalift                                                                                                               ||iandt|   |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#141`_ / is not returning swagger API doc                                                                                                                   ||iandt|   |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#162`_ fields parameter does not return values if more than one value is requested for CSV format                                                           ||iandt|   |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#171`_ summary does not contain the property values                                                                                                         ||iandt|   |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#137`_ [SECURITY] Log4j vulnerability in lexer                                                                                                              ||iandt|   |s.critical                |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#150`_ bundle of a product does not return result                                                                                                           ||iandt|   |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#128`_ Registry API Service docker container fails to start with error: Unable to access jarfile /usr/local/registry-api-service/registry-api-service.jar   ||iandt|   |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#172`_ `fields` query parameter does not work consistently across all response formats                                                                      ||iandt|   |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#167`_ summary-only does not work as expected                                                                                                               ||iandt|   |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#178`_ The /products, /bundles & /collections endpoints are missing from the API                                                                            ||iandt|   |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#179`_ limit=0 is not providing list of properties (fka summary-only)                                                                                       ||iandt|   |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#152`_ summary-only does not work on products of a collection                                                                                               ||iandt|   |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                                   |I&T       |Priority / Bug Severity   |
+========================================================================================================================+==========+==========================+
|`registry-api#109`_ As a user, I want to have an administrator contact when I am getting an error 500 from the server   ||iandt|   |p.should-have             |
+------------------------------------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                          |I&T       |Priority / Bug Severity   |
+===============================================================================================================+==========+==========================+
|`registry-api#108`_ Remove the home controller from the swagger-ui                                             ||iandt|   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#131`_ Refactor API endpoints for simpler architecture/design/implementation to maintain/extend   ||iandt|   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#117`_ Support override of application.properties for AWS Docker image                            |          |p.must-have               |
+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#122`_ [SECURITY] Upgrade jackson dependencies to remove vulnerability                            |          |s.low                     |
+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`registry-api#140`_ Add back the Dockerfile used for the AWS/Fargate deployment                                ||iandt|   |unknown                   |
+---------------------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Registry-mgr
------------
*Standalone Registry Manager application responsible for managing the PDS Registry (https://github.com/NASA-PDS/registry) schemas and indexes.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-mgr>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-mgr/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-mgr/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-mgr/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-mgr/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                      |I&T       |Priority / Bug Severity   |
+===========================================================================+==========+==========================+
|`registry-mgr#53`_ bug with pagination limitations per OpenSearch config   ||iandt|   |s.high                    |
+---------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------+----------+--------------------------+
|Issue                                                        |I&T       |Priority / Bug Severity   |
+=============================================================+==========+==========================+
|`registry-mgr#50`_ As a user I want to search on ref_lid_*   ||iandt|   |p.should-have             |
+-------------------------------------------------------------+----------+--------------------------+

--------

Roundup-action
--------------
*Do a "roundup", a/k/a PDS-style continuous integration and delivery*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/roundup-action#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/roundup-action>`_
     - `Issue Tracking <https://github.com/NASA-PDS/roundup-action/issues>`_
     - `Requirements <https://github.com/NASA-PDS/roundup-action/tree/main/docs/requirements>`_
     - `Stable Release <https://github.com/NASA-PDS/roundup-action/releases/latest>`_
     - `Dev Release <https://github.com/NASA-PDS/roundup-action/releases>`_


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                       |I&T       |Priority / Bug Severity   |
+============================================================================================+==========+==========================+
|`roundup-action#82`_ roundup versioning not working properly on nested maven repositories   ||iandt|   |s.medium                  |
+--------------------------------------------------------------------------------------------+----------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                                     |I&T   |Priority / Bug Severity   |
+==========================================================================================+======+==========================+
|`roundup-action#81`_ Update SNAPSHOT / DEV versioning to always increment minor version   |      |p.should-have             |
+------------------------------------------------------------------------------------------+------+--------------------------+

--------

Software-issues-repo
--------------------
*Issue tracking repository as a centralized entry point for general PDS software bugs and feature requests.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/software-issues-repo#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/software-issues-repo>`_
     - `Issue Tracking <https://github.com/NASA-PDS/software-issues-repo/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/software-issues-repo/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/software-issues-repo/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/software-issues-repo/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`software-issues-repo#36`_ Prep and Improvements for B13.0 Build and Deployment
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+-----------------------------------------------------------------------+------+--------------------------+
|Issue                                                                  |I&T   |Priority / Bug Severity   |
+=======================================================================+======+==========================+
|`software-issues-repo#35`_ Improve internal deployment documentation   |      |p.should-have             |
+-----------------------------------------------------------------------+------+--------------------------+

--------

Template-repo-python
--------------------
*template repository for PDS python developments *

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/template-repo-python>`_
     - `Github Repo <https://github.com/NASA-PDS/template-repo-python>`_
     - `Issue Tracking <https://github.com/NASA-PDS/template-repo-python/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/template-repo-python/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/template-repo-python/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/template-repo-python/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------+------+--------------------------+
|Issue                                                                                                   |I&T   |Priority / Bug Severity   |
+========================================================================================================+======+==========================+
|`template-repo-python#56`_ As a developer, I want to perform continuous integration tests on branches   |      |p.should-have             |
+--------------------------------------------------------------------------------------------------------+------+--------------------------+

--------

Validate
--------
*Validates PDS4 product labels, data and PDS3 Volumes*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/validate/>`_
     - `Github Repo <https://github.com/NASA-PDS/validate>`_
     - `Issue Tracking <https://github.com/NASA-PDS/validate/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/validate/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/validate/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/validate/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`validate#496`_ Support new lblx file extension
+++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+
|Issue                                                                                                    |I&T       |Level         |Priority / Bug Severity   |
+=========================================================================================================+==========+==============+==========================+
|`validate#482`_ As a user, I want to validate labels/bundles/collections using the LBLX file extension   ||iandt|   |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------+----------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                     |I&T       |Priority / Bug Severity   |
+==========================================================================================================+==========+==========================+
|`validate#516`_ validate embedded in an app bundled as a fat-jar raise exception on product validation    ||iandt|   |s.low                     |
+----------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#479`_ validate erroneously flags PDF/A-1a compliant file                                        ||iandt|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#507`_ validate having issues checking some file content on windows                              ||iandt|   |s.high                    |
+----------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#503`_ validate passes confusing message to the command window                                   ||iandt|   |s.high                    |
+----------------------------------------------------------------------------------------------------------+----------+--------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|Issue                                                                                                           |I&T       |Priority / Bug Severity   |
+================================================================================================================+==========+==========================+
|`validate#241`_ As a developer, I want an API method enable specifying of non-registered context products       |          |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+----------+--------------------------+
|`validate#524`_ As a user, I want to receive an error when no products are found within the validation target   ||iandt|   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------+----------+--------------------------+

--------

Wds-web
-------
*PDS Web Design System - Basic web implementation*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds-web>`_
     - `Github Repo <https://github.com/NASA-PDS/wds-web>`_
     - `Issue Tracking <https://github.com/NASA-PDS/wds-web/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/wds-web/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/wds-web/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/wds-web/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------+----------+--------------------------+
|Issue                                                   |I&T       |Priority / Bug Severity   |
+========================================================+==========+==========================+
|`wds-web#31`_ App bar issue identified on ATM website   ||iandt|   |s.medium                  |
+--------------------------------------------------------+----------+--------------------------+

Liens
=====

+-------------------------------------------------------+-------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Issue                                                  |Title                                      |Rationale                                                                                                                                                                                            |
+=======================================================+===========================================+=====================================================================================================================================================================================================+
|pds-swg_17_ [CR] Defer Cloud Pilot projects to B13.1   |[CR] Defer Cloud Pilot projects to B13.1   |All pilot projects are being tabled until next FY when the EN Team has a better grasp of NGAP and how we are able to easily architect and deploy these applications, services, and data into NGAP.   |
+-------------------------------------------------------+-------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B13.0)`_

Installation and Operation
==========================
PDS Engineering Node Software have 3 different venues/purposes for execution: Standalone, Discipline Node Deployment or
Engineering Node-only Deployment
For the Installation and Operation manual see the `users manuals` in the software summary sections below:

- `PDS Standalone`_

- `PDS Discipline Nodes`_

- `PDS Engineering Node Only`_

Reference documents
===================
This section details the controlling and applicable documents referenced for this release. The controlling documents are
as follows:

- PDS Level 1, 2 and 3 Requirements, April 20, 2017.

- PDS4 Project Plan, July 17, 2013.

- PDS4 System Architecture Specification, Version 1.3, September 1, 2013.

- PDS4 Operations Concept, Version 1.0, September 1, 2013.

- PDS Harvest Tool Software Requirements and Design Document (SRD/SDD), Version 1.2, September 1, 2013.

- PDS Preparation Tools Software Requirements and Design Document (SRD/SDD), Version 0.3, September 1, 2013.

- PDS Registry Service Software Requirements and Design Document (SRD/SDD), Version 1.1, September 1, 2013.

- PDS Report Service Software Requirements and Design Document (SRD/SDD), Version 1.1, September 1, 2013.

- PDS Search Service Software Requirements and Design Document (SRD/SDD), Version 1.0, September 1, 2013.

- PDS Search Scenarios, Version 1.0, September 1, 2013.

- PDS Search Protocol, Version 1.2, March 21, 2014.

- PDAP Search Protocol, Version 1.0, March 21, 2014.

- PDS Security Service Software Requirements and Design Document (SRD/SDD), Version 1.1, September 1, 2013.

- `PDS Deep Archive Software Requirements and Design Document (SRD/SDD)`_

- `PDS DOI Service Requirements and Design Document (SRD/SDD)`_

.. _plan B13.0: https://nasa-pds.github.io/releases/13.0/plan.html
.. _pds4-information-model#499: https://github.com/NASA-PDS/pds4-information-model/issues/499
.. |iandt| image:: https://nasa-pds.github.io/_static/images/noun_certified_18093.png
   :alt: I&T
   :width: 20
.. _cloud-tasks#28: https://github.com/NASA-PDS/cloud-tasks/issues/28
.. _cloud-tasks#37: https://github.com/NASA-PDS/cloud-tasks/issues/37
.. _design-team#138: https://github.com/NASA-PDS/design-team/issues/138
.. _design-team#129: https://github.com/NASA-PDS/design-team/issues/129
.. _design-team#130: https://github.com/NASA-PDS/design-team/issues/130
.. _design-team#132: https://github.com/NASA-PDS/design-team/issues/132
.. _design-team#135: https://github.com/NASA-PDS/design-team/issues/135
.. _design-team#136: https://github.com/NASA-PDS/design-team/issues/136
.. _design-team#141: https://github.com/NASA-PDS/design-team/issues/141
.. _design-team#143: https://github.com/NASA-PDS/design-team/issues/143
.. _design-team#152: https://github.com/NASA-PDS/design-team/issues/152
.. _design-team#153: https://github.com/NASA-PDS/design-team/issues/153
.. _design-team#154: https://github.com/NASA-PDS/design-team/issues/154
.. _design-team#139: https://github.com/NASA-PDS/design-team/issues/139
.. _design-team#140: https://github.com/NASA-PDS/design-team/issues/140
.. _devops#11: https://github.com/NASA-PDS/devops/issues/11
.. _devops#2: https://github.com/NASA-PDS/devops/issues/2
.. _devops#22: https://github.com/NASA-PDS/devops/issues/22
.. _devops#24: https://github.com/NASA-PDS/devops/issues/24
.. _devops#27: https://github.com/NASA-PDS/devops/issues/27
.. _doi-service#350: https://github.com/NASA-PDS/doi-service/issues/350
.. _doi-service#331: https://github.com/NASA-PDS/doi-service/issues/331
.. _doi-service#13: https://github.com/NASA-PDS/doi-service/issues/13
.. _doi-service#224: https://github.com/NASA-PDS/doi-service/issues/224
.. _doi-service#335: https://github.com/NASA-PDS/doi-service/issues/335
.. _doi-service#344: https://github.com/NASA-PDS/doi-service/issues/344
.. _doi-ui#137: https://github.com/NASA-PDS/doi-ui/issues/137
.. _doi-ui#151: https://github.com/NASA-PDS/doi-ui/issues/151
.. _doi-ui#130: https://github.com/NASA-PDS/doi-ui/issues/130
.. _doi-ui#160: https://github.com/NASA-PDS/doi-ui/issues/160
.. _doi-ui#155: https://github.com/NASA-PDS/doi-ui/issues/155
.. _doi-ui#145: https://github.com/NASA-PDS/doi-ui/issues/145
.. _doi-ui#149: https://github.com/NASA-PDS/doi-ui/issues/149
.. _doi-ui#143: https://github.com/NASA-PDS/doi-ui/issues/143
.. _doi-ui#147: https://github.com/NASA-PDS/doi-ui/issues/147
.. _harvest#90: https://github.com/NASA-PDS/harvest/issues/90
.. _nucleus#1: https://github.com/NASA-PDS/nucleus/issues/1
.. _pds-api#129: https://github.com/NASA-PDS/pds-api/issues/129
.. _pds-api#169: https://github.com/NASA-PDS/pds-api/issues/169
.. _pds-api#173: https://github.com/NASA-PDS/pds-api/issues/173
.. _pds-api#202: https://github.com/NASA-PDS/pds-api/issues/202
.. _pds-api#209: https://github.com/NASA-PDS/pds-api/issues/209
.. _pds-api#216: https://github.com/NASA-PDS/pds-api/issues/216
.. _pds-api#148: https://github.com/NASA-PDS/pds-api/issues/148
.. _pds-api#60: https://github.com/NASA-PDS/pds-api/issues/60
.. _pds-api#101: https://github.com/NASA-PDS/pds-api/issues/101
.. _pds-api#125: https://github.com/NASA-PDS/pds-api/issues/125
.. _pds-api#191: https://github.com/NASA-PDS/pds-api/issues/191
.. _pds-api#183: https://github.com/NASA-PDS/pds-api/issues/183
.. _pds-api#172: https://github.com/NASA-PDS/pds-api/issues/172
.. _pds4-information-model#468: https://github.com/NASA-PDS/pds4-information-model/issues/468
.. _pds4-information-model#499: https://github.com/NASA-PDS/pds4-information-model/issues/499
.. _pds4-information-model#460: https://github.com/NASA-PDS/pds4-information-model/issues/460
.. _planetarydata.org#6: https://github.com/NASA-PDS/planetarydata.org/issues/6
.. _portal-tasks#35: https://github.com/NASA-PDS/portal-tasks/issues/35
.. _portal-tasks#38: https://github.com/NASA-PDS/portal-tasks/issues/38
.. _portal-tasks#22: https://github.com/NASA-PDS/portal-tasks/issues/22
.. _portal-tasks#26: https://github.com/NASA-PDS/portal-tasks/issues/26
.. _registry#55: https://github.com/NASA-PDS/registry/issues/55
.. _registry#57: https://github.com/NASA-PDS/registry/issues/57
.. _registry#45: https://github.com/NASA-PDS/registry/issues/45
.. _registry#64: https://github.com/NASA-PDS/registry/issues/64
.. _registry#84: https://github.com/NASA-PDS/registry/issues/84
.. _registry#67: https://github.com/NASA-PDS/registry/issues/67
.. _registry-api#134: https://github.com/NASA-PDS/registry-api/issues/134
.. _registry-api#121: https://github.com/NASA-PDS/registry-api/issues/121
.. _registry-api#162: https://github.com/NASA-PDS/registry-api/issues/162
.. _registry-api#172: https://github.com/NASA-PDS/registry-api/issues/172
.. _registry-api#167: https://github.com/NASA-PDS/registry-api/issues/167
.. _registry-api#178: https://github.com/NASA-PDS/registry-api/issues/178
.. _registry-api#179: https://github.com/NASA-PDS/registry-api/issues/179
.. _registry-api#109: https://github.com/NASA-PDS/registry-api/issues/109
.. _registry-api#117: https://github.com/NASA-PDS/registry-api/issues/117
.. _registry-api#122: https://github.com/NASA-PDS/registry-api/issues/122
.. _registry-mgr#53: https://github.com/NASA-PDS/registry-mgr/issues/53
.. _registry-mgr#50: https://github.com/NASA-PDS/registry-mgr/issues/50
.. _software-issues-repo#36: https://github.com/NASA-PDS/software-issues-repo/issues/36
.. _software-issues-repo#35: https://github.com/NASA-PDS/software-issues-repo/issues/35
.. _template-repo-python#56: https://github.com/NASA-PDS/template-repo-python/issues/56
.. _validate#496: https://github.com/NASA-PDS/validate/issues/496
.. _validate#482: https://github.com/NASA-PDS/validate/issues/482
.. _validate#516: https://github.com/NASA-PDS/validate/issues/516
.. _validate#507: https://github.com/NASA-PDS/validate/issues/507
.. _validate#524: https://github.com/NASA-PDS/validate/issues/524
.. _wds-web#31: https://github.com/NASA-PDS/wds-web/issues/31
.. _pds-swg_17: https://github.com/NASA-PDS/pds-swg/issues/17
.. _Software Release Summary (B13.0): https://nasa-pds.github.io/releases/13.0/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
