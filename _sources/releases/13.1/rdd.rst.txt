==========================================
Release Description Document (Build B13.1)
==========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B13.1`_

The following sections can be found in this document:

.. toctree::
   :glob: 
   :maxdepth: 3

   rdd.rst

PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Board
and implemented by the PDS within the latest build period.

+--------------------------------+-----------------------------------------------------------------------------------------------------+
|Ref                             |Title                                                                                                |
+================================+=====================================================================================================+
|`pds4-information-model#502`_   |CCB-350: Adopt more rigorous / stringent rules for leap seconds and use of "24:00:00" in datetimes   |
+--------------------------------+-----------------------------------------------------------------------------------------------------+
|`pds4-information-model#599`_   |CCB-360: Add new permissible value to Units_of_Misc                                                  |
+--------------------------------+-----------------------------------------------------------------------------------------------------+
|`pds4-information-model#602`_   |CCB-361: Add a permissible value for microradians to Units_of_Angle                                  |
+--------------------------------+-----------------------------------------------------------------------------------------------------+
|`pds4-information-model#603`_   |CCB-362: Add a permissible value of nm/mm to Units_of_Misc                                           |
+--------------------------------+-----------------------------------------------------------------------------------------------------+
|`pds4-information-model#608`_   |CCB-354: Add new permissible values to Header/parsing_standard_id to support new versions of CDF     |
+--------------------------------+-----------------------------------------------------------------------------------------------------+
|`pds4-information-model#611`_   |CCB-355: Add Funding_Acknowledgement class to Citation_Information Class                             |
+--------------------------------+-----------------------------------------------------------------------------------------------------+
|`pds4-information-model#616`_   |CCB-325: Support for video and audio as product observational                                        |
+--------------------------------+-----------------------------------------------------------------------------------------------------+

Software Changes
================
The changes types are 'Bug', 'Enhancement' or 'Requirement'. For each software repository, the changes are listed in 2
categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B13.1`_)
The 'Other Updates' occurs during the build cycle witout being planned or attached to a theme. They are organized by
types (bug, enhancements, requirements, tasks). Any updates that require a de-scope of planned tasks are reviewed by the
PDS Software Working Group.

The deliveries are validated by the development team and go through an additional Integration & Test process, as
applicable, as indicated by the ```Testing Status``` column in the tables below. There are 3 possible statuses for
testing:

- |:blue_circle:| Skip Testing - Testing is not needed for this ticket. These are determined at the discretion of the team based upon the technical or operational nature of the closed task.
- |:yellow_circle:| Testing Needed
- |:green_circle:| Testing Complete - Initial testing complete, and test cases/results documented.

--------

Cloud-tasks
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
`cloud-tasks#24`_ Re-imagine and Implement New Registry Architecture in AWS
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`cloud-tasks#34`_ Phase 1: Plan and Architect SBN-PSI Catalina Sky Survey Migration
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`cloud-tasks#40`_ NGAP Onboarding
+++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`cloud-tasks#57`_ Prototype and Adapt ESDIS Thin Egresss App (TEA) for PDS
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`cloud-tasks#60`_ Develop initial PDS Cloud Cost Model
++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

--------

Deep-archive
------------
*PDS Open Archival Information System (OAIS) utilities, including Submission Information Package (SIP) and Archive Information Package (AIP) generators*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/deep-archive/>`_
     - `Github Repo <https://github.com/NASA-PDS/deep-archive>`_
     - `Issue Tracking <https://github.com/NASA-PDS/deep-archive/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/deep-archive/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/deep-archive/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/deep-archive/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================================================================+====================+==========================+
|`deep-archive#134`_ Cannot connect to any PDS API endpoints for pds-deep-archive-registry                ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`deep-archive#145`_ Canonical path is not processed correctly ('/../ in path)                            ||:yellow_circle:|   |s.critical                |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`deep-archive#137`_ Pagination handling does not appear to work properly for pds-deep-registry-archive   ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Doi-service
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

+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================================================================+====================+==========================+
|`doi-service#403`_ CICD: build does not work because of dependency conflicts                             ||:blue_circle:|     |s.high                    |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`doi-service#398`_ Still -- Unable to generate / export json report of DOI metadata                      ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`doi-service#377`_ DOI Service does not accurately parse <author_list> and <editor_list> in XML labels   ||:green_circle:|    |s.medium                  |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|Issue                                                                                                                           |I&T Status         |Priority / Bug Severity   |
+================================================================================================================================+===================+==========================+
|`doi-service#344`_ As a user, I want to release a DOI with a label that does not contain the DOI                                ||:green_circle:|   |p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`doi-service#283`_ As a publisher, I want to be notified when a new DOI has been minted or significant update to the metadata   ||:green_circle:|   |p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                    |I&T Status        |Priority / Bug Severity   |
+=========================================================================+==================+==========================+
|`doi-service#363`_ Enhance weekly reporting to push to ADS SFTP server   ||:blue_circle:|   |p.must-have               |
+-------------------------------------------------------------------------+------------------+--------------------------+

--------

Doi-ui
------
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
`doi-ui#153`_ Develop DOI Editor and Service Documentation
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                 |I&T Status          |Priority / Bug Severity   |
+======================================================================+====================+==========================+
|`doi-ui#130`_ Remove vulnerabilities from the package per npm audit   ||:yellow_circle:|   |s.high                    |
+----------------------------------------------------------------------+--------------------+--------------------------+
|`doi-ui#167`_ doi-editor release ui inoperable under Firefox          ||:yellow_circle:|   |s.high                    |
+----------------------------------------------------------------------+--------------------+--------------------------+

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

+--------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                       |I&T Status          |Priority / Bug Severity   |
+============================================================================================+====================+==========================+
|`harvest#112`_ --overwrite flag is not respected for <bundles> elements in harvest config   ||:yellow_circle:|   |s.high                    |
+--------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`harvest#102`_ Harvest skips path that is the root of a soft link                           ||:green_circle:|    |s.high                    |
+--------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------+--------------------+--------------------------+
|Issue                                                 |I&T Status          |Priority / Bug Severity   |
+======================================================+====================+==========================+
|`harvest#106`_ Improve skipped product INFO message   ||:yellow_circle:|   |p.should-have             |
+------------------------------------------------------+--------------------+--------------------------+

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
`nucleus#2`_ Initial Implementation and Operationalize Nucleus
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                              |I&T Status          |Level         |Priority / Bug Severity   |
+===================================================================================+====================+==============+==========================+
|`nucleus#29`_ As a user, I want to know the baseline architecture and deployment   ||:yellow_circle:|   |requirement   |p.must-have               |
+-----------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


`nucleus#14`_ B13.1 Technology Selection and Internal Review
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`nucleus#16`_ Develop Cost Model
++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+
|Issue                                                                                             |I&T Status          |Level   |Priority / Bug Severity   |
+==================================================================================================+====================+========+==========================+
|`nucleus#37`_ Prepare cost model for Nucleus - Considering Amazon Managed Airflow (Amazon MWAA)   ||:yellow_circle:|   |task    |unknown                   |
+--------------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+


`nucleus#18`_ Develop Detailed Technical Architecture
+++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

--------

Operations
----------
*Tickets for the PDSEN Operations Team*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/operations#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/operations>`_
     - `Issue Tracking <https://github.com/NASA-PDS/operations/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/operations/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/operations/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/operations/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`operations#309`_ Initial Wordpress migration for pds-engineering website
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`operations#369`_ B13.1 Prep and Stage IM and Tools for I&T
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

--------

Pds-api
-------
*PDS web APIs specifications and user's manual*

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
`pds-api#181`_ Initial PDS Keyword Search Design
++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`pds-api#230`_ Support latest product search from API
+++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                                                        |I&T Status          |Level         |Priority / Bug Severity   |
+=============================================================================================================+====================+==============+==========================+
|`pds-api#220`_ Past versions are being returned by API, by default                                           ||:yellow_circle:|   |bug           |s.high                    |
+-------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`pds-api#221`_ As a user, I want to query only the latest versions of products unless explicitly requested   ||:yellow_circle:|   |requirement   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


`pds-api#235`_ Enable Swagger Interface on pds.nasa.gov
+++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                                                                       |I&T Status          |Level         |Priority / Bug Severity   |
+============================================================================================================================+====================+==============+==========================+
|`pds-api#193`_ As a user, I want to be able to access the Search API Swagger interface from pds.nasa.gov                    ||:yellow_circle:|   |requirement   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`pds-api#239`_ As a user, I want to get application/json response format by default if I request an API url in my browser   ||:yellow_circle:|   |requirement   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                               |I&T Status          |Priority / Bug Severity   |
+====================================================================================================+====================+==========================+
|`pds-api#257`_ Search API documentation seems outdated?                                             ||:blue_circle:|     |s.medium                  |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#251`_ link to registry-api documentation from registry page is incorrect                   ||:blue_circle:|     |s.low                     |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#214`_ vnd.nasa.pds.pds4+json format does return information                                ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#240`_ API Client cannot connect to current deployed API                                    ||:yellow_circle:|   |s.high                    |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#213`_ Accept header of text/csv returns blank lines                                        ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#199`_ `hits` appears to be showing the current page count, not the overall number of its   ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#215`_ vnd.nasa.pds.pds4+xml format does not return information                             ||:green_circle:|    |s.medium                  |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#200`_ API performance degradation from B12.1 release                                       ||:yellow_circle:|   |s.high                    |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#196`_ Swagger API page does not show the expected deployed API version                     ||:yellow_circle:|   |s.low                     |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                         |I&T Status          |Priority / Bug Severity   |
+==============================================================================================+====================+==========================+
|`pds-api#198`_ As a user, I want query responses for empty results to be clearly documented   ||:green_circle:|    |p.should-have             |
+----------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#175`_ As a user, I want to know how to query observational data only                 ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------+-------------------+--------------------------+
|Issue                                                                   |I&T Status         |Priority / Bug Severity   |
+========================================================================+===================+==========================+
|`pds-api#194`_ Develop NASA/PDS Skin for Search API Swagger interface   ||:green_circle:|   |unknown                   |
+------------------------------------------------------------------------+-------------------+--------------------------+

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
`pds4-information-model#513`_ B13.1 Prep IM and LDDTool for new IM Version
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`pds4-information-model#544`_ Test and Validate Term Mapping Implementation
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`pds4-information-model#546`_ B13.1 Continue Refactoring the IMTool/LDDTool Code
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`pds4-information-model#547`_ B13.1 Updates per CCB-Approved SCRs
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|Issue                                                                                                                            |I&T Status         |Level         |Priority / Bug Severity   |
+=================================================================================================================================+===================+==============+==========================+
|`pds4-information-model#599`_ CCB-360: Add new permissible value to Units_of_Misc                                                ||:green_circle:|   |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|`pds4-information-model#602`_ CCB-361: Add a permissible value for microradians to Units_of_Angle                                ||:green_circle:|   |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|`pds4-information-model#603`_ CCB-362: Add a permissible value of nm/mm to Units_of_Misc                                         ||:green_circle:|   |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|`pds4-information-model#608`_ CCB-354: Add new permissible values to Header/parsing_standard_id to support new versions of CDF   ||:green_circle:|   |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|`pds4-information-model#611`_ CCB-355: Add Funding_Acknowledgement class to Citation_Information Class                           ||:green_circle:|   |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|`pds4-information-model#616`_ CCB-325: Support for video and audio as product observational                                      ||:green_circle:|   |requirement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+


`pds4-information-model#548`_ B13.1 Expand Support for SKOSS Terminological Entry Mapping
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------+------------------+--------+--------------------------+
|Issue                                                                         |I&T Status        |Level   |Priority / Bug Severity   |
+==============================================================================+==================+========+==========================+
|`pds4-information-model#544`_ Test and Validate Term Mapping Implementation   ||:blue_circle:|   |theme   |unknown                   |
+------------------------------------------------------------------------------+------------------+--------+--------------------------+


`pds4-information-model#549`_ B13.1 Initial Support for Target Ontology Project
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`pds4-information-model#625`_ B13.1 Document Updates
++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                          |I&T Status          |Priority / Bug Severity   |
+===============================================================================================================================+====================+==========================+
|`pds4-information-model#648`_ Revert date format change from #641 in Product_XML_Schema                                        ||:yellow_circle:|   |s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds4-information-model#618`_ Information Model does not have Product_External included in Identification_Area.product_class   ||:green_circle:|    |s.critical                |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds4-information-model#606`_ LDDTool does not write a DocBook file for the Common Dictionary                                  ||:blue_circle:|     |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds4-information-model#506`_ hyb2 has incorrect namespace for IM v1.14                                                        ||:blue_circle:|     |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds4-information-model#507`_ Bug generating BepiColombo SERENA dictionary                                                     ||:blue_circle:|     |s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|Issue                                                                                                                                    |I&T Status         |Priority / Bug Severity   |
+=========================================================================================================================================+===================+==========================+
|`pds4-information-model#473`_ As a user, I want to describe a relationship between an attribute in the model and the column of a table   ||:green_circle:|   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`pds4-information-model#502`_ CCB-350: Adopt more rigorous / stringent rules for leap seconds and use of "24:00:00" in datetimes         ||:green_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`pds4-information-model#458`_ As a developer I want to have the PDS4 Information Model expressed in the RDF/OWL/TTL format.              ||:blue_circle:|    |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`pds4-information-model#620`_ As a user I want to export the IM in the RDF/OWL format in RDF format                                      ||:blue_circle:|    |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                   |I&T Status        |Priority / Bug Severity   |
+========================================================================+==================+==========================+
|`pds4-information-model#641`_ Update date format to be timezone aware   ||:blue_circle:|   |unknown                   |
+------------------------------------------------------------------------+------------------+--------------------------+

--------

Pds4-jparser
------------
*Java Library providing APIs for parsing and exporting information on PDS4 products, including table and image objects to various formats including CSV, PNG, VICAR, FITs, etc.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds4-jparser/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-jparser>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-jparser/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/pds4-jparser/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-jparser/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-jparser/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                            |I&T Status          |Priority / Bug Severity   |
+=================================================================================+====================+==========================+
|`pds4-jparser#57`_ Parse failure for table fields of type ASCII_Numeric_Base16   ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------+--------------------+--------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                     |I&T Status          |Priority / Bug Severity   |
+==========================================================================================================+====================+==========================+
|`portal-tasks#55`_ dataset status needs to be updated to better handle potential security vulnerability   ||:yellow_circle:|   |s.critical                |
+----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`portal-tasks#47`_ [SECURITY] JQuery upgrade needed to avoid possible injection                           ||:yellow_circle:|   |s.high                    |
+----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`portal-tasks#54`_ Possible XSS vulnerability on data set view pages                                      ||:yellow_circle:|   |s.critical                |
+----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`portal-tasks#69`_ Freedom of Information Act link is sending users to an Access Denied page.             ||:yellow_circle:|   |s.low                     |
+----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`portal-tasks#31`_ Data release manager pages missing login session check                                 ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`portal-tasks#68`_ Links returning 404                                                                    ||:yellow_circle:|   |s.low                     |
+----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`portal-tasks#56`_ SQL permission on data-search                                                          ||:blue_circle:|     |s.critical                |
+----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`portal-tasks#8`_ URL Encoding errors from Subscription Service pages                                     ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|Issue                                                                                                                 |I&T Status         |Priority / Bug Severity   |
+======================================================================================================================+===================+==========================+
|`portal-tasks#49`_ Update DataSet View to display DOI from label if there is no DOI for the product in our database   ||:green_circle:|   |p.should-have             |
+----------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`portal-tasks#58`_ Update PDS4 data dictionary links to be more consistent between Common and Local DD links          ||:blue_circle:|    |unknown                   |
+----------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`portal-tasks#57`_ Add new MILabel video and presentation to training site                                            ||:blue_circle:|    |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+

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
`registry#148`_ Develop Simple Dashboard for Node Monitoring
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|Issue                                                                                                                      |I&T Status         |Level         |Priority / Bug Severity   |
+===========================================================================================================================+===================+==============+==========================+
|`registry#130`_ As a user, I want to view dashboard report of bundles with archive status and other tracking information   ||:green_circle:|   |requirement   |p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                                                                        |I&T Status          |Priority / Bug Severity   |
+=============================================================================================================================================================================================+====================+==========================+
|`registry#159`_ ref_collection_lidvid field in some node registries populated using older versions of registry loader tools create string fields in the schema vs. the expected list types   ||:green_circle:|    |s.medium                  |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#118`_ archive status value was not changed on bundle's contents                                                                                                                    ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#146`_ OpenSearch service of Registry won't start on Linux                                                                                                                          ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#136`_ follow on to #118, registry-manager still unable to change archive status on bundle contents                                                                                 ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#97`_ registry-manager won't set archive-status on some collections                                                                                                                 ||:green_circle:|    |s.high                    |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#150`_ TLS termination listening on wrong port                                                                                                                                      ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#120`_ Continuous Delivery not working with OpenSearch                                                                                                                              ||:blue_circle:|     |s.medium                  |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                          |I&T Status          |Priority / Bug Severity   |
+===============================================================================================+====================+==========================+
|`registry#153`_ As a user, I want to all metadata attributes to be searchable                  ||:yellow_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#52`_ As a user, I want to indicate a product has been superseded                     ||:green_circle:|    |p.should-have             |
+-----------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#100`_ Update documentation to include explicit example of how to query staged data   ||:green_circle:|    |p.must-have               |
+-----------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|Issue                                                                                                  |I&T Status         |Priority / Bug Severity   |
+=======================================================================================================+===================+==========================+
|`registry#100`_ Update documentation to include explicit example of how to query staged data           ||:green_circle:|   |p.must-have               |
+-------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`registry#139`_ Update docs to be more clear that there is a required next step after data ingestion   ||:blue_circle:|    |unknown                   |
+-------------------------------------------------------------------------------------------------------+-------------------+--------------------------+

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
`registry-api#257`_ B13.1 Fix must-have bugs for Registry API
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+
|Issue                                                                                       |I&T Status          |Level   |Priority / Bug Severity   |
+============================================================================================+====================+========+==========================+
|`registry-api#241`_ requests with bad `q=` syntax should return 400 error                   ||:yellow_circle:|   |bug     |s.medium                  |
+--------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+
|`registry-api#258`_ not found lidvid does not return 404 error                              ||:yellow_circle:|   |bug     |s.medium                  |
+--------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+
|`registry-api#260`_ api does not return 400 error when q parameter value cannot be parsed   ||:yellow_circle:|   |bug     |s.medium                  |
+--------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+
|`registry-api#261`_ The members of a bundle can not be requested                            ||:yellow_circle:|   |bug     |s.high                    |
+--------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+
|`registry-api#287`_ Search criteria not producing expected matches                          ||:green_circle:|    |task    |unknown                   |
+--------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                     |I&T Status          |Priority / Bug Severity   |
+==========================================================================================================================================+====================+==========================+
|`registry-api#293`_ Requests with Accept:application/vnd.nasa.gds.pds4+json fail for products with no ops:Label_File_Info/ops:file_name   ||:blue_circle:|     |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#190`_ /all suffix returns a message which I don't understand                                                                ||:green_circle:|    |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#202`_ observational end-point returns collections                                                                           ||:green_circle:|    |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#231`_ /classes/collections/<lidvid>/members (and deprecated equivalent) hangs                                               ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#121`_ Fix vulnerabilities raised by sonalift                                                                                ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#224`_ registry-api does not return latest version of product metadata when multiple versions are harvested                  ||:green_circle:|    |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#148`_ *Critical OSS Vulnerability:* spring-web@5.3.20                                                                       ||:yellow_circle:|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#206`_ When q="" the returned status is 500 instead of 400                                                                   ||:yellow_circle:|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#207`_ lidvid not found raises 500 error                                                                                     ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#211`_ swaggger ui error in production                                                                                       ||:green_circle:|    |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#191`_ version number are treated as floats                                                                                  ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#227`_ Keyword search does not work on registry-api deployed on pds.nasa.gov                                                 ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#196`_ documents / members returns an error                                                                                  ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#240`_ Pagination not working as expected with /collections/{identifier}/products                                            ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#200`_ /classes endpoint does not work in a browser                                                                          ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#234`_ registry-api does not respect VID when a LIDVID is used as an id, instead returns latest version                      ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                      |I&T Status          |Priority / Bug Severity   |
+===========================================================================================================================================+====================+==========================+
|`registry-api#212`_ As a user, I want the API to support redundant `/` in the url                                                          ||:green_circle:|    |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#223`_ As a user, I want to know the members of a bundle product                                                              ||:green_circle:|    |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#282`_ As a user, I want to search by any metadata attribute                                                                  ||:green_circle:|    |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#208`_ As a registry-tool/registry-user I want to ensure leading multiple forward-slashes in request paths are stripped out   ||:green_circle:|    |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#248`_ Suggest: Return Content-Type application/json by default                                                               ||:yellow_circle:|   |unknown                   |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Registry-common
---------------
*Library utilized by tools that manage and load data into the PDS Registry, including Harvest, Registry Manager, and Supplementer*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-common>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-common/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-common/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-common/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-common/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                          |I&T Status          |Priority / Bug Severity   |
+===============================================================================================================+====================+==========================+
|`registry-common#32`_ JSON BLOB performs undesirable conversion of floating-point types with int-like values   ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-common#31`_ Registry manager fails with updates to LDDTool to support ISO Formatted dates            ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Registry-crawler-service
------------------------
*Server application providing the functionality for crawling PDS4 products. It has to be used with other components, such as RabbitMQ message broker, Harvest Server and Harvest Client  to enable performant ingestion of large data sets into PDS Registry (https://github.com/NASA-PDS/registry).*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-crawler-service#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-crawler-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-crawler-service/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-crawler-service/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-crawler-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-crawler-service/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                                  |I&T Status        |Priority / Bug Severity   |
+=======================================================================================+==================+==========================+
|`registry-crawler-service#24`_ Stable Roundup can no longer trigger Imaging workflow   ||:blue_circle:|   |unknown                   |
+---------------------------------------------------------------------------------------+------------------+--------------------------+

--------

Registry-harvest-cli
--------------------
*Client application providing the functionality for capturing and indexing product metadata into the PDS Registry system (https://github.com/NASA-PDS/registry). Different from the standalone Harvest Tool, this goes along with Crawler and Harvest Server to enable performant ingestion of large data sets.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-harvest-cli#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-harvest-cli>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-harvest-cli/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-harvest-cli/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-harvest-cli/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-harvest-cli/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                              |I&T Status        |Priority / Bug Severity   |
+===================================================================================+==================+==========================+
|`registry-harvest-cli#16`_ Stable Roundup can no longer trigger Imaging workflow   ||:blue_circle:|   |unknown                   |
+-----------------------------------------------------------------------------------+------------------+--------------------------+

--------

Registry-harvest-service
------------------------
*Server application providing the functionality for capturing and indexing product metadata into the PDS Registry system (https://github.com/NASA-PDS/registry). Different from the standalone Harvest Tool, this goes along with Crawler and Harvest Client to enable performant ingestion of large data sets.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-harvest-service#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-harvest-service>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-harvest-service/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-harvest-service/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-harvest-service/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-harvest-service/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------------+-------------------+--------------------------+
|Issue                                                                                       |I&T Status         |Priority / Bug Severity   |
+============================================================================================+===================+==========================+
|`registry-harvest-service#25`_ Harvest service sometimes skips collection inventory files   ||:green_circle:|   |s.high                    |
+--------------------------------------------------------------------------------------------+-------------------+--------------------------+

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

+-----------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                  |I&T Status          |Priority / Bug Severity   |
+=======================================================================+====================+==========================+
|`registry-mgr#57`_ ref_lid_collection error when ingesting data sets   ||:yellow_circle:|   |s.medium                  |
+-----------------------------------------------------------------------+--------------------+--------------------------+

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

+------------------------------------------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                                                             |I&T Status        |Priority / Bug Severity   |
+==================================================================================================================+==================+==========================+
|`roundup-action#104`_ Versions in CHANGELOG off a bit since we moved to release tagging scheme on Java projects   ||:blue_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------+------------------+--------------------------+
|`roundup-action#96`_ Roundup failing on unstable build                                                            ||:blue_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------+------------------+--------------------------+
|`roundup-action#103`_ unstable build failed                                                                       ||:blue_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------+------------------+--------------------------+
|`roundup-action#98`_ git push in roundup action failing w/ remote ahead of local                                  ||:blue_circle:|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------+------------------+--------------------------+
|`roundup-action#105`_ Roundup broken for python repos                                                             ||:blue_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------+------------------+--------------------------+

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
`software-issues-repo#52`_ B13.1 Planning
+++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

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
Bugs
++++

+----------------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                                   |I&T Status        |Priority / Bug Severity   |
+========================================================================================+==================+==========================+
|`template-repo-python#67`_ Local pre-commit checks pass, but in branch workflow fails   ||:blue_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------+------------------+--------------------------+

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
`validate#414`_ Referential Integrity Checking with the Registry+API
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                                                            |I&T Status          |Level         |Priority / Bug Severity   |
+=================================================================================================================+====================+==============+==========================+
|`validate#415`_ As a user, I want to validate all internal references to products in the PDS archive are valid   ||:yellow_circle:|   |requirement   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#601`_ Create command-line script to wrap the new registry referential integrity checker                ||:blue_circle:|     |enhancement   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


`validate#481`_ B13.1 Content Validation Improvements: Intermingled Headers
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|Issue                                                                                                    |I&T Status         |Level         |Priority / Bug Severity   |
+=========================================================================================================+===================+==============+==========================+
|`validate#425`_ Refactor content validation to more robustly handle intermingled Headers                 ||:green_circle:|   |enhancement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|`validate#480`_ Validate does not calculate overlaps correctly when Header is not first object in file   ||:green_circle:|   |bug           |s.medium                  |
+---------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+


`validate#498`_ Improve Content Validation Performance through Spot Checking
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|Issue                                                                                  |I&T Status         |Level         |Priority / Bug Severity   |
+=======================================================================================+===================+==============+==========================+
|`validate#1`_ As a user, I want to execute content validation against every nth file   ||:green_circle:|   |requirement   |p.could-have              |
+---------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+


`validate#557`_ Dockerize Validate
++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|Issue                                                                                  |I&T Status         |Level         |Priority / Bug Severity   |
+=======================================================================================+===================+==============+==========================+
|`validate#556`_ As a user, I want to be able to use validate from a docker container   ||:green_circle:|   |requirement   |p.should-have             |
+---------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+


`validate#578`_ B13.1 Fix Must-Have Priority Bugs
+++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|Issue                                                                                                                                                 |I&T Status         |Level   |Priority / Bug Severity   |
+======================================================================================================================================================+===================+========+==========================+
|`validate#444`_ pds4.bundle option seems to not travel through enough subdirectories                                                                  ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#453`_ Validate should not check PDF/A validity if content validation is disabled                                                            ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#474`_ Validate can't find files in directory specified by <directory_path_name>                                                             ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#499`_ validate doesn't flag a data file with only LF                                                                                        ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#503`_ validate passes confusing message to the command window                                                                               ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#511`_ Table_Character not accurately checking field formats                                                                                 ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#514`_ Validate does not catch NaNs in Binary Tables                                                                                         ||:green_circle:|   |bug     |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#519`_ Validate should throw record length error when record delimiter does not occur in correct location                                    ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#529`_  ERROR  [error.array.value_out_of_min_max_range] evaluation is not correct                                                            ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#531`_ ERROR  [error.table.bad_file_read] incorrectly reports that GroupFieldBinary group_length is larger than size of contained fields     ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#544`_ validate gives a error.table.bad_field_read error                                                                                     ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#554`_ --spot-check-data flag throws IOException                                                                                             ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#564`_ Array object validation regression in v3.0.3                                                                                          ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#576`_ validate does not correctly handle field format checks for hex values                                                                 ||:green_circle:|   |bug     |p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#597`_ Validate does not maintain history of other versions it comes across as it traverses directories causing erroneous WARNING messages   ||:green_circle:|   |bug     |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+
|`validate#611`_ Missing validation of valid_maximum and valid_minimum from Special_Constants                                                          ||:green_circle:|   |bug     |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+--------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                           |I&T Status          |Priority / Bug Severity   |
+================================================================================================================+====================+==========================+
|`validate#593`_ Regression in validate no longer enabling CRLF to be embedded within a Table_Character record   ||:green_circle:|    |s.high                    |
+----------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#551`_ Validate fails regression test on issue 188                                                     ||:green_circle:|    |s.medium                  |
+----------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#620`_ verbosity flag does not appear to output INFO messages                                          ||:blue_circle:|     |s.medium                  |
+----------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#473`_ NullPointerException when Table_Delimited is missing records attribute                          ||:green_circle:|    |s.low                     |
+----------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#616`_ validate does not correctly validate byte offsets to data objects                               ||:green_circle:|    |s.high                    |
+----------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#155`_ Fix uncaught exception error when validating an array object                                    ||:green_circle:|    |s.low                     |
+----------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#614`_ invalid_object_definition occurs upon out-of-order data objects                                 ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|Issue                                                                                                                        |I&T Status         |Priority / Bug Severity   |
+=============================================================================================================================+===================+==========================+
|`validate#595`_ As a user, I want to validate all collections referenced from a bundle exist within the archive              ||:green_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`validate#596`_ As a user, I want to validate all products referenced from a collection exist within the archive             ||:green_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`validate#316`_ As a user, I want to validate all internal references from one product to another exist within the archive   ||:green_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+--------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------------------------------+-------------------+--------------------------+
|Issue                                                                                       |I&T Status         |Priority / Bug Severity   |
+============================================================================================+===================+==========================+
|`validate#537`_ Refactor `getMessageCountBasedOnProblemType` function using introspection   ||:blue_circle:|    |unknown                   |
+--------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`validate#436`_ Improve error messages for overlapping objects in a label                   ||:green_circle:|   |p.should-have             |
+--------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`validate#569`_ Improve error message when file is truncated and cannot be read             ||:green_circle:|   |p.could-have              |
+--------------------------------------------------------------------------------------------+-------------------+--------------------------+
|`validate#434`_ Scaled value min/max error does not display scaled value                    ||:blue_circle:|    |p.should-have             |
+--------------------------------------------------------------------------------------------+-------------------+--------------------------+

--------

Wds-implementation
------------------
*PDS Web Design System*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds>`_
     - `Github Repo <https://github.com/NASA-PDS/wds-implementation>`_
     - `Issue Tracking <https://github.com/NASA-PDS/wds-implementation/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/wds-implementation/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/wds-implementation/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/wds-implementation/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`wds-implementation#22`_ Initial Data Search Journey Prototype
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

--------

Web-analytics
-------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/web-analytics#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/web-analytics>`_
     - `Issue Tracking <https://github.com/NASA-PDS/web-analytics/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/web-analytics/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/web-analytics/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/web-analytics/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                 |I&T Status          |Priority / Bug Severity   |
+======================================================================================================+====================+==========================+
|`web-analytics#2`_ As a data engineer, I want to sync logs from PDS website in an automated fashion   ||:yellow_circle:|   |p.should-have             |
+------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Web-modernization
-----------------
*PDS.nasa.gov Web Modernization repo for managing the overall design process and user testing for modernizing the PDS web experience.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/web-modernization#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/web-modernization>`_
     - `Issue Tracking <https://github.com/NASA-PDS/web-modernization/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/web-modernization/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/web-modernization/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/web-modernization/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`web-modernization#161`_ B13.1 User Journey Figma Prototyping: Homepage & Search
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Liens
=====

+------------------------------------------------------------------+------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Issue                                                             |Title                                                 |Rationale                                                                                                                                                                                                                                                                                                                                                                 |
+==================================================================+======================================================+==========================================================================================================================================================================================================================================================================================================================================================================+
|pds-swg_21_ [CR] Defer Validate Content Validation Improvements   |[CR] Defer Validate Content Validation Improvements   |Numerous bug fixes added onto the front half of the build implementation pushed out all other higher priority improvements. This will move onto B14.0 stack. Additionally, a lot of these tickets may have been fixed or improved from some of the bug fixes from B13.1, but we have not had the time to come up with sufficient test data to test all the table types.   |
+------------------------------------------------------------------+------------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B13.1)`_

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

.. _plan B13.1: https://nasa-pds.github.io/releases/13.1/plan.html
.. _pds4-information-model#502: https://github.com/NASA-PDS/pds4-information-model/issues/502
.. _pds4-information-model#599: https://github.com/NASA-PDS/pds4-information-model/issues/599
.. _pds4-information-model#602: https://github.com/NASA-PDS/pds4-information-model/issues/602
.. _pds4-information-model#603: https://github.com/NASA-PDS/pds4-information-model/issues/603
.. _pds4-information-model#608: https://github.com/NASA-PDS/pds4-information-model/issues/608
.. _pds4-information-model#611: https://github.com/NASA-PDS/pds4-information-model/issues/611
.. _pds4-information-model#616: https://github.com/NASA-PDS/pds4-information-model/issues/616
.. _cloud-tasks#24: https://github.com/NASA-PDS/cloud-tasks/issues/24
.. _cloud-tasks#34: https://github.com/NASA-PDS/cloud-tasks/issues/34
.. _cloud-tasks#40: https://github.com/NASA-PDS/cloud-tasks/issues/40
.. _cloud-tasks#57: https://github.com/NASA-PDS/cloud-tasks/issues/57
.. _cloud-tasks#60: https://github.com/NASA-PDS/cloud-tasks/issues/60
.. _deep-archive#134: https://github.com/NASA-PDS/deep-archive/issues/134
.. _deep-archive#145: https://github.com/NASA-PDS/deep-archive/issues/145
.. _deep-archive#137: https://github.com/NASA-PDS/deep-archive/issues/137
.. _doi-service#403: https://github.com/NASA-PDS/doi-service/issues/403
.. _doi-service#398: https://github.com/NASA-PDS/doi-service/issues/398
.. _doi-service#377: https://github.com/NASA-PDS/doi-service/issues/377
.. _doi-service#344: https://github.com/NASA-PDS/doi-service/issues/344
.. _doi-service#283: https://github.com/NASA-PDS/doi-service/issues/283
.. _doi-service#363: https://github.com/NASA-PDS/doi-service/issues/363
.. _doi-ui#153: https://github.com/NASA-PDS/doi-ui/issues/153
.. _doi-ui#130: https://github.com/NASA-PDS/doi-ui/issues/130
.. _doi-ui#167: https://github.com/NASA-PDS/doi-ui/issues/167
.. _harvest#112: https://github.com/NASA-PDS/harvest/issues/112
.. _harvest#102: https://github.com/NASA-PDS/harvest/issues/102
.. _harvest#106: https://github.com/NASA-PDS/harvest/issues/106
.. _nucleus#2: https://github.com/NASA-PDS/nucleus/issues/2
.. _nucleus#29: https://github.com/NASA-PDS/nucleus/issues/29
.. _nucleus#14: https://github.com/NASA-PDS/nucleus/issues/14
.. _nucleus#16: https://github.com/NASA-PDS/nucleus/issues/16
.. _nucleus#37: https://github.com/NASA-PDS/nucleus/issues/37
.. _nucleus#18: https://github.com/NASA-PDS/nucleus/issues/18
.. _operations#309: https://github.com/NASA-PDS/operations/issues/309
.. _operations#369: https://github.com/NASA-PDS/operations/issues/369
.. _pds-api#181: https://github.com/NASA-PDS/pds-api/issues/181
.. _pds-api#230: https://github.com/NASA-PDS/pds-api/issues/230
.. _pds-api#220: https://github.com/NASA-PDS/pds-api/issues/220
.. _pds-api#221: https://github.com/NASA-PDS/pds-api/issues/221
.. _pds-api#235: https://github.com/NASA-PDS/pds-api/issues/235
.. _pds-api#193: https://github.com/NASA-PDS/pds-api/issues/193
.. _pds-api#239: https://github.com/NASA-PDS/pds-api/issues/239
.. _pds-api#257: https://github.com/NASA-PDS/pds-api/issues/257
.. _pds-api#251: https://github.com/NASA-PDS/pds-api/issues/251
.. _pds-api#214: https://github.com/NASA-PDS/pds-api/issues/214
.. _pds-api#240: https://github.com/NASA-PDS/pds-api/issues/240
.. _pds-api#213: https://github.com/NASA-PDS/pds-api/issues/213
.. _pds-api#199: https://github.com/NASA-PDS/pds-api/issues/199
.. _pds-api#215: https://github.com/NASA-PDS/pds-api/issues/215
.. _pds-api#200: https://github.com/NASA-PDS/pds-api/issues/200
.. _pds-api#196: https://github.com/NASA-PDS/pds-api/issues/196
.. _pds-api#198: https://github.com/NASA-PDS/pds-api/issues/198
.. _pds-api#175: https://github.com/NASA-PDS/pds-api/issues/175
.. _pds-api#194: https://github.com/NASA-PDS/pds-api/issues/194
.. _pds4-information-model#513: https://github.com/NASA-PDS/pds4-information-model/issues/513
.. _pds4-information-model#544: https://github.com/NASA-PDS/pds4-information-model/issues/544
.. _pds4-information-model#546: https://github.com/NASA-PDS/pds4-information-model/issues/546
.. _pds4-information-model#547: https://github.com/NASA-PDS/pds4-information-model/issues/547
.. _pds4-information-model#599: https://github.com/NASA-PDS/pds4-information-model/issues/599
.. _pds4-information-model#602: https://github.com/NASA-PDS/pds4-information-model/issues/602
.. _pds4-information-model#603: https://github.com/NASA-PDS/pds4-information-model/issues/603
.. _pds4-information-model#608: https://github.com/NASA-PDS/pds4-information-model/issues/608
.. _pds4-information-model#611: https://github.com/NASA-PDS/pds4-information-model/issues/611
.. _pds4-information-model#616: https://github.com/NASA-PDS/pds4-information-model/issues/616
.. _pds4-information-model#548: https://github.com/NASA-PDS/pds4-information-model/issues/548
.. _pds4-information-model#544: https://github.com/NASA-PDS/pds4-information-model/issues/544
.. _pds4-information-model#549: https://github.com/NASA-PDS/pds4-information-model/issues/549
.. _pds4-information-model#625: https://github.com/NASA-PDS/pds4-information-model/issues/625
.. _pds4-information-model#648: https://github.com/NASA-PDS/pds4-information-model/issues/648
.. _pds4-information-model#618: https://github.com/NASA-PDS/pds4-information-model/issues/618
.. _pds4-information-model#606: https://github.com/NASA-PDS/pds4-information-model/issues/606
.. _pds4-information-model#506: https://github.com/NASA-PDS/pds4-information-model/issues/506
.. _pds4-information-model#507: https://github.com/NASA-PDS/pds4-information-model/issues/507
.. _pds4-information-model#473: https://github.com/NASA-PDS/pds4-information-model/issues/473
.. _pds4-information-model#502: https://github.com/NASA-PDS/pds4-information-model/issues/502
.. _pds4-information-model#458: https://github.com/NASA-PDS/pds4-information-model/issues/458
.. _pds4-information-model#620: https://github.com/NASA-PDS/pds4-information-model/issues/620
.. _pds4-information-model#641: https://github.com/NASA-PDS/pds4-information-model/issues/641
.. _pds4-jparser#57: https://github.com/NASA-PDS/pds4-jparser/issues/57
.. _portal-tasks#55: https://github.com/NASA-PDS/portal-tasks/issues/55
.. _portal-tasks#47: https://github.com/NASA-PDS/portal-tasks/issues/47
.. _portal-tasks#54: https://github.com/NASA-PDS/portal-tasks/issues/54
.. _portal-tasks#69: https://github.com/NASA-PDS/portal-tasks/issues/69
.. _portal-tasks#31: https://github.com/NASA-PDS/portal-tasks/issues/31
.. _portal-tasks#68: https://github.com/NASA-PDS/portal-tasks/issues/68
.. _portal-tasks#56: https://github.com/NASA-PDS/portal-tasks/issues/56
.. _portal-tasks#8: https://github.com/NASA-PDS/portal-tasks/issues/8
.. _portal-tasks#49: https://github.com/NASA-PDS/portal-tasks/issues/49
.. _portal-tasks#58: https://github.com/NASA-PDS/portal-tasks/issues/58
.. _portal-tasks#57: https://github.com/NASA-PDS/portal-tasks/issues/57
.. _registry#148: https://github.com/NASA-PDS/registry/issues/148
.. _registry#130: https://github.com/NASA-PDS/registry/issues/130
.. _registry#159: https://github.com/NASA-PDS/registry/issues/159
.. _registry#118: https://github.com/NASA-PDS/registry/issues/118
.. _registry#146: https://github.com/NASA-PDS/registry/issues/146
.. _registry#136: https://github.com/NASA-PDS/registry/issues/136
.. _registry#97: https://github.com/NASA-PDS/registry/issues/97
.. _registry#150: https://github.com/NASA-PDS/registry/issues/150
.. _registry#120: https://github.com/NASA-PDS/registry/issues/120
.. _registry#153: https://github.com/NASA-PDS/registry/issues/153
.. _registry#52: https://github.com/NASA-PDS/registry/issues/52
.. _registry#100: https://github.com/NASA-PDS/registry/issues/100
.. _registry#100: https://github.com/NASA-PDS/registry/issues/100
.. _registry#139: https://github.com/NASA-PDS/registry/issues/139
.. _registry-api#257: https://github.com/NASA-PDS/registry-api/issues/257
.. _registry-api#241: https://github.com/NASA-PDS/registry-api/issues/241
.. _registry-api#258: https://github.com/NASA-PDS/registry-api/issues/258
.. _registry-api#260: https://github.com/NASA-PDS/registry-api/issues/260
.. _registry-api#261: https://github.com/NASA-PDS/registry-api/issues/261
.. _registry-api#287: https://github.com/NASA-PDS/registry-api/issues/287
.. _registry-api#293: https://github.com/NASA-PDS/registry-api/issues/293
.. _registry-api#190: https://github.com/NASA-PDS/registry-api/issues/190
.. _registry-api#202: https://github.com/NASA-PDS/registry-api/issues/202
.. _registry-api#231: https://github.com/NASA-PDS/registry-api/issues/231
.. _registry-api#121: https://github.com/NASA-PDS/registry-api/issues/121
.. _registry-api#224: https://github.com/NASA-PDS/registry-api/issues/224
.. _registry-api#148: https://github.com/NASA-PDS/registry-api/issues/148
.. _registry-api#206: https://github.com/NASA-PDS/registry-api/issues/206
.. _registry-api#207: https://github.com/NASA-PDS/registry-api/issues/207
.. _registry-api#211: https://github.com/NASA-PDS/registry-api/issues/211
.. _registry-api#191: https://github.com/NASA-PDS/registry-api/issues/191
.. _registry-api#227: https://github.com/NASA-PDS/registry-api/issues/227
.. _registry-api#196: https://github.com/NASA-PDS/registry-api/issues/196
.. _registry-api#240: https://github.com/NASA-PDS/registry-api/issues/240
.. _registry-api#200: https://github.com/NASA-PDS/registry-api/issues/200
.. _registry-api#234: https://github.com/NASA-PDS/registry-api/issues/234
.. _registry-api#212: https://github.com/NASA-PDS/registry-api/issues/212
.. _registry-api#223: https://github.com/NASA-PDS/registry-api/issues/223
.. _registry-api#282: https://github.com/NASA-PDS/registry-api/issues/282
.. _registry-api#208: https://github.com/NASA-PDS/registry-api/issues/208
.. _registry-api#248: https://github.com/NASA-PDS/registry-api/issues/248
.. _registry-common#32: https://github.com/NASA-PDS/registry-common/issues/32
.. _registry-common#31: https://github.com/NASA-PDS/registry-common/issues/31
.. _registry-crawler-service#24: https://github.com/NASA-PDS/registry-crawler-service/issues/24
.. _registry-harvest-cli#16: https://github.com/NASA-PDS/registry-harvest-cli/issues/16
.. _registry-harvest-service#25: https://github.com/NASA-PDS/registry-harvest-service/issues/25
.. _registry-mgr#57: https://github.com/NASA-PDS/registry-mgr/issues/57
.. _roundup-action#104: https://github.com/NASA-PDS/roundup-action/issues/104
.. _roundup-action#96: https://github.com/NASA-PDS/roundup-action/issues/96
.. _roundup-action#103: https://github.com/NASA-PDS/roundup-action/issues/103
.. _roundup-action#98: https://github.com/NASA-PDS/roundup-action/issues/98
.. _roundup-action#105: https://github.com/NASA-PDS/roundup-action/issues/105
.. _software-issues-repo#52: https://github.com/NASA-PDS/software-issues-repo/issues/52
.. _template-repo-python#67: https://github.com/NASA-PDS/template-repo-python/issues/67
.. _validate#414: https://github.com/NASA-PDS/validate/issues/414
.. _validate#415: https://github.com/NASA-PDS/validate/issues/415
.. _validate#601: https://github.com/NASA-PDS/validate/issues/601
.. _validate#481: https://github.com/NASA-PDS/validate/issues/481
.. _validate#425: https://github.com/NASA-PDS/validate/issues/425
.. _validate#480: https://github.com/NASA-PDS/validate/issues/480
.. _validate#498: https://github.com/NASA-PDS/validate/issues/498
.. _validate#1: https://github.com/NASA-PDS/validate/issues/1
.. _validate#557: https://github.com/NASA-PDS/validate/issues/557
.. _validate#556: https://github.com/NASA-PDS/validate/issues/556
.. _validate#578: https://github.com/NASA-PDS/validate/issues/578
.. _validate#444: https://github.com/NASA-PDS/validate/issues/444
.. _validate#453: https://github.com/NASA-PDS/validate/issues/453
.. _validate#474: https://github.com/NASA-PDS/validate/issues/474
.. _validate#499: https://github.com/NASA-PDS/validate/issues/499
.. _validate#503: https://github.com/NASA-PDS/validate/issues/503
.. _validate#511: https://github.com/NASA-PDS/validate/issues/511
.. _validate#514: https://github.com/NASA-PDS/validate/issues/514
.. _validate#519: https://github.com/NASA-PDS/validate/issues/519
.. _validate#529: https://github.com/NASA-PDS/validate/issues/529
.. _validate#531: https://github.com/NASA-PDS/validate/issues/531
.. _validate#544: https://github.com/NASA-PDS/validate/issues/544
.. _validate#554: https://github.com/NASA-PDS/validate/issues/554
.. _validate#564: https://github.com/NASA-PDS/validate/issues/564
.. _validate#576: https://github.com/NASA-PDS/validate/issues/576
.. _validate#597: https://github.com/NASA-PDS/validate/issues/597
.. _validate#611: https://github.com/NASA-PDS/validate/issues/611
.. _validate#593: https://github.com/NASA-PDS/validate/issues/593
.. _validate#551: https://github.com/NASA-PDS/validate/issues/551
.. _validate#620: https://github.com/NASA-PDS/validate/issues/620
.. _validate#473: https://github.com/NASA-PDS/validate/issues/473
.. _validate#616: https://github.com/NASA-PDS/validate/issues/616
.. _validate#155: https://github.com/NASA-PDS/validate/issues/155
.. _validate#614: https://github.com/NASA-PDS/validate/issues/614
.. _validate#595: https://github.com/NASA-PDS/validate/issues/595
.. _validate#596: https://github.com/NASA-PDS/validate/issues/596
.. _validate#316: https://github.com/NASA-PDS/validate/issues/316
.. _validate#537: https://github.com/NASA-PDS/validate/issues/537
.. _validate#436: https://github.com/NASA-PDS/validate/issues/436
.. _validate#569: https://github.com/NASA-PDS/validate/issues/569
.. _validate#434: https://github.com/NASA-PDS/validate/issues/434
.. _wds-implementation#22: https://github.com/NASA-PDS/wds-implementation/issues/22
.. _web-analytics#2: https://github.com/NASA-PDS/web-analytics/issues/2
.. _web-modernization#161: https://github.com/NASA-PDS/web-modernization/issues/161
.. _pds-swg_21: https://github.com/NASA-PDS/pds-swg/issues/21
.. _Software Release Summary (B13.1): https://nasa-pds.github.io/releases/13.1/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
