========================================
Release Description Document (Build B18)
========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B18`_

The following sections can be found in this document:

.. toctree::
   :glob:
   :maxdepth: 3

   rdd.rst


PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Board
and implemented by the PDS within the latest build period.

+--------------------------------+--------------------------------------------------------------------------------------------------+
| Ref                            | Title                                                                                            |
+================================+==================================================================================================+
| `pds4-information-model#1002`_ | CCB-75: Add new value for object type  - "Interstellar Object"                                   |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1003`_ | CCB-58: New Product_Native values for MSL/Mastcam                                                |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1004`_ | CCB-79: Add enumerated value day**-1 to Units_of_Rates                                           |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1005`_ | CCB-80: Support NEF as a Native format for Artemis                                               |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1006`_ | CCB-85: Expand definition of DataCurator to account for non-PDS archivists and for cloud storage |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1007`_ | CCB-86: List_Author and similar list classes should have cardinality 0:1 instead of 0:M          |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1008`_ | CCB-88: Broken link to the PDS Policy on Packed Data in the Standards Reference                  |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1032`_ | [documentation] CCB-68: Update ASCII_File_Name and ASCII_Directory_Path_Name                     |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1033`_ | [documentation] CCB-58: New Product_Native values for MSL/Mastcam                                |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1034`_ | [documentation] CCB-79 : Add enumerated value day**-1 to Units_of_Rates                          |
+--------------------------------+--------------------------------------------------------------------------------------------------+
| `pds4-information-model#1035`_ | [documentation] CCB-80: Support NEF as a Native format for Artemis                               |
+--------------------------------+--------------------------------------------------------------------------------------------------+

Software Changes
================
For each software repository, the changes are listed in 2 categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B18`_).

The 'Other Updates' occurs during the build cycle without being planned or attached to a theme. They are organized by
types (bug, enhancements, requirements, tasks). Any updates that require a de-scope of planned tasks are reviewed by the
PDS Software Working Group.

The deliveries are validated by the development team and go through an additional Integration & Test process, as
applicable, as indicated by the ```Testing Status``` column in the tables below. There are 3 possible statuses for
testing:

- |:blue_circle:| Skip Testing - Testing is not needed for this ticket. These are determined at the discretion of the
  team based upon the technical or operational nature of the closed task.
- |:yellow_circle:| Testing Needed
- |:green_circle:| Testing Complete - Initial testing complete, and test cases/results documented.

--------

Component: Cloud Operations
---------------------------
*Cloud operations, utilities, and authentication*

--------

Component: Cloud Platform Engineering
-------------------------------------
*Planetary Data Cloud platform infrastructure and engineering*

--------

Component: Data Upload Manager
------------------------------
*Data Upload Manager (DUM) for managing data uploads to PDC*

--------

Data-upload-manager
~~~~~~~~~~~~~~~~~~~
*Data Upload Manager (DUM) component for managing the interface for data uploads to the Planetary Data Cloud from Data Providers and PDS Nodes.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/data-upload-manager>`_
     - `Github Repo <https://github.com/NASA-PDS/data-upload-manager>`_
     - `Issue Tracking <https://github.com/NASA-PDS/data-upload-manager/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/data-upload-manager/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/data-upload-manager/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/data-upload-manager/releases>`_ 


Planned Updates
+++++++++++++++
`data-upload-manager#349`_ B18 DUM Support:  High Priority Enhancements / Bug Fixes / Tasks
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
+++++++++++++
Bugs
^^^^

+-------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                               | I&T Status        | Priority / Bug Severity   |
+=====================================================================================+===================+===========================+
| `data-upload-manager#352`_ DUM v2.4.2 CloudWatch Logs SerializationException Errors | |:yellow_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Component: Deep Archive
-----------------------
*PDS Open Archival Information System (OAIS) utilities for deep archive operations*

--------

Component: Devops
-----------------
*DevOps tools, CI/CD pipelines, and automation infrastructure*

--------

Roundup-action
~~~~~~~~~~~~~~
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
+++++++++++++++
No planned updates realized for this build in this repository.

Other Updates
+++++++++++++
Requirements
^^^^^^^^^^^^

+---------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================================================+===================+===========================+
| `roundup-action#170`_ As a developer, I want Maven builds to always force re-resolution of previously failed artifact downloads | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Component: DOI Service
----------------------
*Digital Object Identifier (DOI) service for PDS data products*

--------

Component: Integration And Testing
----------------------------------
*Integration and testing infrastructure*

--------

Component: Nucleus
------------------
*Nucleus workflow platform for planetary data processing*

--------

Component: Operations
---------------------
*PDS Engineering Node operations and issue tracking*

--------

En-ops-utils
~~~~~~~~~~~~
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/en-ops-utils#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/en-ops-utils>`_
     - `Issue Tracking <https://github.com/NASA-PDS/en-ops-utils/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/en-ops-utils/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/en-ops-utils/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/en-ops-utils/releases>`_ 


Planned Updates
+++++++++++++++
No planned updates realized for this build in this repository.

Other Updates
+++++++++++++
Requirements
^^^^^^^^^^^^

+--------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================================================================================+===================+===========================+
| `en-ops-utils#18`_ As a user, I want to verify context product version_id matches filename version suffix                | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `en-ops-utils#19`_ As a user, I want to verify deprecated context product LIDs have been removed from the PDS Search API | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `en-ops-utils#16`_ As a steward, I want auto-generated LDD release PRs to include a reviewer checklist                   | |:yellow_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Component: PDS4 Information Model
---------------------------------
*PDS4 Information Model, ontology, and data dictionary tools*

--------

Pds4-context-products
~~~~~~~~~~~~~~~~~~~~~
*Repository for managing PDS4 Context Products*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds4-context-products#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pds4-context-products>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds4-context-products/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/pds4-context-products/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds4-context-products/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds4-context-products/releases>`_ 


Planned Updates
+++++++++++++++
`pds4-context-products#85`_ Cleanup Deprecated Context Products from API and Web Portal
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+----------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------+---------------------------+
| Issue                                                                                                                                        | I&T Status      | Level   | Priority / Bug Severity   |
+==============================================================================================================================================+=================+=========+===========================+
| `pds4-context-products#84`_ Chandrayaan-1 NASA PDS investigation (and maybe instrument host, and instruments?) are not accurately deprecated | |:blue_circle:| | bug     | s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------+---------------------------+


Other Updates
+++++++++++++
Requirements
^^^^^^^^^^^^

+----------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                              | I&T Status        | Priority / Bug Severity   |
+====================================================================================================================================================+===================+===========================+
| `pds4-context-products#94`_ As a user, I want CI to verify deprecated LIDs are removed from the PDS Search API when lids_deprecated.csv is updated | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Pds4-information-model
~~~~~~~~~~~~~~~~~~~~~~
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
+++++++++++++++
`pds4-information-model#984`_ B17 Information Model Delivery to I&T
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+---------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================================+=================+===========================+
| `pds4-information-model#984`_ B17 Information Model Delivery to I&T | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------+-----------------+---------------------------+


`pds4-information-model#1014`_ B18 Information Model SCR Implementation and LDDTool Updates
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+----------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                          | I&T Status        | Level   | Priority / Bug Severity   |
+================================================================+===================+=========+===========================+
| `pds4-information-model#1047`_ ldd-prov test cases are failing | |:yellow_circle:| | bug     | s.high                    |
+----------------------------------------------------------------+-------------------+---------+---------------------------+


`pds4-information-model#1015`_ B18 SCR Freeze
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`pds4-information-model#1016`_ B18 Information Model Delivery to I&T
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`pds4-information-model#1017`_ B18 Standards Documents Updates
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`pds4-information-model#1026`_ Complete v1.0 of OPS LDD
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
+++++++++++++
Bugs
^^^^

+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================================+===================+===========================+
| `pds4-information-model#1042`_ Radar namespace is not present in namespace registry                   | |:yellow_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#1049`_ lddtool generates confusing error message for Local_Internal_Reference | |:yellow_circle:| | s.low                     |
+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
^^^^^^^^^^^^

+-----------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                       | I&T Status      | Priority / Bug Severity   |
+=============================================================================+=================+===========================+
| `pds4-information-model#1038`_ [namespace-registry] add new namespace AV    | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#1040`_ [namespace-registry] add new namespace BOPPS | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------------------+-----------------+---------------------------+

--------

Component: PDS4 Viewer
----------------------
*Tools for viewing and visualizing PDS4 data products*

--------

Pds4-jparser
~~~~~~~~~~~~
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
+++++++++++++++
No planned updates realized for this build in this repository.

Other Updates
+++++++++++++
Bugs
^^^^

+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================================================+===================+===========================+
| `pds4-jparser#200`_ RawTableReader readNextLine() treats 0xFF data bytes as EOF due to byte-to-int sign-extension | |:yellow_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
^^^^^^^^^^^^

+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================================================================================================================================================================+===================+===========================+
| `pds4-jparser#197`_ As a PDS data engineer, I want RawTableReader to use buffered bulk I/O so that large table products with millions of records can be validated without extreme performance degradation | |:yellow_circle:| | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
^^^^^^^^^^^^

+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================================================================================================================================================================+===================+===========================+
| `pds4-jparser#197`_ As a PDS data engineer, I want RawTableReader to use buffered bulk I/O so that large table products with millions of records can be validated without extreme performance degradation | |:yellow_circle:| | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Component: Peppi
----------------
*Planetary Data Explorer Python (PEPPi) client library*

--------

Peppi
~~~~~
*Planetary Data Explorer: Python (PEPPi) client library (pds.peppi) to access Planetary Data from the NASA Planetary Data System*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/peppi>`_
     - `Github Repo <https://github.com/NASA-PDS/peppi>`_
     - `Issue Tracking <https://github.com/NASA-PDS/peppi/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/peppi/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/peppi/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/peppi/releases>`_ 


Planned Updates
+++++++++++++++
`peppi#171`_ Support DOI Search
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+-------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                             | I&T Status        | Level       | Priority / Bug Severity   |
+===================================================================+===================+=============+===========================+
| `peppi#158`_ As a data user, I want to search for products by DOI | |:yellow_circle:| | requirement | unknown                   |
+-------------------------------------------------------------------+-------------------+-------------+---------------------------+


Other Updates
+++++++++++++
Bugs
^^^^

+----------------------------------------------------------+-------------------+---------------------------+
| Issue                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================+===================+===========================+
| `peppi#168`_ count() does not return the total hit count | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------+-------------------+---------------------------+

--------

Component: Registry Tools
-------------------------
*PDS Registry backend services and data loading tools*

--------

Harvest
~~~~~~~
*Version<=4 of the standalone Harvest client application providing the functionality for capturing and indexing product metadata into the PDS Registry system. Version 5+ are now managed through https://github.com/NASA-PDS/registry-loader/*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/harvest>`_
     - `Issue Tracking <https://github.com/NASA-PDS/harvest/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/harvest/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/harvest/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/harvest/releases>`_ 


Planned Updates
+++++++++++++++
No planned updates realized for this build in this repository.

Other Updates
+++++++++++++
Bugs
^^^^

+--------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================================+===================+===========================+
| `harvest#316`_ ops:Harvest_Meta fields missing data type definitions in registry data dictionary | |:yellow_circle:| | s.critical                |
+--------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry
~~~~~~~~
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
+++++++++++++++
`registry#266`_ Implement design for alternate data file paths / file path updates
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry#371`_ Adapt Harvest to Support Using Inventories for Data File Metadata
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry#432`_ Onboard IPDA Partner: ISRO
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry#498`_ B18 Registry Support: High Priority Enhancements / Bug Fixes / Tasks
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+--------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                  | I&T Status        | Level       | Priority / Bug Severity   |
+========================================================================================================+===================+=============+===========================+
| `registry#497`_ As a developer, I want human-readable Postman collection docs auto-generated on update | |:yellow_circle:| | requirement | p.should-have             |
+--------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `registry#509`_ set-archive-status does not apply to secondary products in a collection                | |:yellow_circle:| | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`registry#517`_ Integrate Registry sub-components with Managed Opensearch
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
+++++++++++++
Requirements
^^^^^^^^^^^^

+-------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================================================================+===================+===========================+
| `registry#510`_ As a registry operator, I want burnup charts and per-node tracking in status reports to monitor data loading progress over time | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
^^^^^^^^^^^^

+-------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================================================================+===================+===========================+
| `registry#510`_ As a registry operator, I want burnup charts and per-node tracking in status reports to monitor data loading progress over time | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry-api
~~~~~~~~~~~~
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
+++++++++++++++
`registry-api#715`_ Complete Design for Supporting Registration and Search of Mirrored Archives
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#617`_ Develop Test Suite for Testing Production Registry API
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#682`_ Enable Free-Text Search for the PDS Registry
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#698`_ Refactor Registry API Functionality for `/products/{identifier}/members/members`
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#708`_ Develop a Throttling and Scaling Strategy for Registry and API
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#729`_ Update Functionality To Find When Class / Attribute Has Been Used / Exists
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+----------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                                  | I&T Status      | Level       | Priority / Bug Severity   |
+========================================================================================+=================+=============+===========================+
| `registry-api#727`_ As a user, I want the exists operator to be prepended to the query | |:blue_circle:| | enhancement | p.should-have             |
+----------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


`registry-api#749`_ B18 Registry API Support: High Priority Enhancements / Bug Fixes / Tasks
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#751`_ Finalize Release of`/members` Enhancements to Production
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#760`_ Automate Integration Testing in GitHub Actions CI Pipeline
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#768`_ Complete Transition to Full Structured XML Metadata in Registry
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
+++++++++++++
Bugs
^^^^

+-------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                       | I&T Status        | Priority / Bug Severity   |
+=============================================================================================================+===================+===========================+
| `registry-api#742`_ A query to pds.nasa.gov does not respond the same as a query to pds.mcp.nasa.gov        | |:yellow_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#745`_ Integration tests in unstable build suite do not pass when run locally                  | |:yellow_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#748`_ Investigate and fix skipped `product/{id}/member*` integration tests                    | |:blue_circle:|   | s.medium                  |
+-------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#744`_ Unstable build does not complete on develop branch due to GitHub Actions runner timeout | |:yellow_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
^^^^^^^^^^^^

+-------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                       | I&T Status        | Priority / Bug Severity   |
+=============================================================================================================+===================+===========================+
| `registry-api#611`_ As a user, I want to search by a full/unique hierarchical path for a specific attribute | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry-loader
~~~~~~~~~~~~~~~
*Tools used to load and update data in the registry, currently harvest and registry manager package in a docker image. *

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-loader#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-loader>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-loader/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-loader/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-loader/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-loader/releases>`_ 


Planned Updates
+++++++++++++++
`registry-loader#67`_ Enforce strict schema and data type resolution during product loading
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                                                              | I&T Status        | Level       | Priority / Bug Severity   |
+====================================================================================================================================================================================+===================+=============+===========================+
| `registry-loader#65`_ As a node operator, I want harvest to fail product loading when a namespace schema or attribute data type cannot be found                                    | |:yellow_circle:| | requirement | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `registry-loader#66`_ As a node operator, I want to force-load products when namespace schema or attribute type is unresolvable, knowing affected fields will not be fully indexed | |:yellow_circle:| | requirement | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


Other Updates
+++++++++++++
Bugs
^^^^

+-------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================================================================================================+===================+===========================+
| `registry-loader#77`_ Harvest does not download LDD on Windows: temp file creation fails with 'The system cannot find the path specified' | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry-mgr
~~~~~~~~~~~~
*Version<=5 of the standalone Registry Manager application responsible for managing the PDS Registry (https://github.com/NASA-PDS/registry) schemas and indexes. Version 6+ is now managed through https://github.com/NASA-PDS/registry-loader/ .*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-mgr>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-mgr/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-mgr/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-mgr/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-mgr/releases>`_ 


Planned Updates
+++++++++++++++
No planned updates realized for this build in this repository.

Other Updates
+++++++++++++
Bugs
^^^^

+----------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                            | I&T Status      | Priority / Bug Severity   |
+==================================================================================+=================+===========================+
| `registry-mgr#72`_ When delete-data command is used, log file specified is empty | |:blue_circle:| | s.medium                  |
+----------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Registry-sweepers
~~~~~~~~~~~~~~~~~
*Scripts that run regularly on the registry database, to clean and consolidate information *

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-sweepers#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-sweepers>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-sweepers/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-sweepers/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-sweepers/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-sweepers/releases>`_ 


Planned Updates
+++++++++++++++
`registry-sweepers#201`_ Implement Handling of Partial Collections Uploads and Orphan Products
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-sweepers#205`_ Implement Support for Superseded Data using PROV LDD
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-sweepers#210`_ Implement Sweepers Execution in Airflow
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                                                          | I&T Status        | Level   | Priority / Bug Severity   |
+================================================================================================+===================+=========+===========================+
| `registry-sweepers#208`_ legacy-sync sweeper does not run in DEV venue on EN node via airflow. | |:yellow_circle:| | bug     | s.medium                  |
+------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+


Other Updates
+++++++++++++
Bugs
^^^^

+--------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                | I&T Status        | Priority / Bug Severity   |
+======================================================================================================================================+===================+===========================+
| `registry-sweepers#212`_ Legacy registry sync node assignment does not use registry API metadata, causing incorrect node assignments | |:yellow_circle:| | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-sweepers#220`_ Race condition exists when sweepers ensures index mappings and writes document updates very soon after      | |:yellow_circle:| | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Component: Search API
---------------------
*PDS Search API and client libraries*

--------

Component: System Engineering
-----------------------------
*System-level engineering, requirements, and documentation*

--------

Component: System Tools
-----------------------
*System-level utilities and libraries*

--------

Pds-agent-skills
~~~~~~~~~~~~~~~~
*Claude Code skills marketplace for NASA PDS workflows - automated release notes, program status reports, and more*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/pds-agent-skills/>`_
     - `Github Repo <https://github.com/NASA-PDS/pds-agent-skills>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pds-agent-skills/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/pds-agent-skills/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pds-agent-skills/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pds-agent-skills/releases>`_ 


Planned Updates
+++++++++++++++
No planned updates realized for this build in this repository.

Other Updates
+++++++++++++
Requirements
^^^^^^^^^^^^

+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================================================================================================================================================+===================+===========================+
| `pds-agent-skills#6`_ As a PDS developer, I want to export and triage GitHub Dependabot alerts so that I can track and remediate dependency vulnerabilities across NASA-PDS repositories | |:yellow_circle:| | p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Component: Validate
-------------------
*PDS4 data product validation tools*

--------

Validate
~~~~~~~~
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
+++++++++++++++
`validate#1549`_ B18 Validate Support: High Priority Enhancements / Bug Fixes / Tasks
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`validate#1595`_ Performance Improvements for Large Bundle Validation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                                                                  | I&T Status        | Level       | Priority / Bug Severity   |
+========================================================================================================================================================================================+===================+=============+===========================+
| `validate#1570`_ As a PDS developer, I want inline regex patterns in FieldValueValidator pre-compiled as static constants so that per-field Pattern compilation overhead is eliminated | |:blue_circle:|   | requirement | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#1571`_ validate does not complete validation of large bundles (23000+ products) due to OutOfMemoryError in InMemoryRegistrar                                                 | |:yellow_circle:| | bug         | s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#1565`_ As a PDS data engineer, I want schematron transformers to be cached rather than recompiled for every label so that bundle validation is significantly faster          | |:blue_circle:|   | requirement | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#1568`_ As a PDS data engineer, I want parsed DOM trees cached and reused during referential integrity checks so that labels are not re-parsed from disk a second time        | |:yellow_circle:| | enhancement | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


Other Updates
+++++++++++++
Bugs
^^^^

+--------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================================================================================+===================+===========================+
| `validate#1548`_ validate does not fail or report errors when an explicitly-specified target file does not exist         | |:yellow_circle:| | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1601`_ warning.integrity.member_not_found should be an ERROR by default, with new flag to downgrade to warning | |:yellow_circle:| | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Component: Web Analytics
------------------------
*Web analytics tools and monitoring*

--------

Component: Web Content
----------------------
*PDS website content management and legacy systems*

--------

Portal
~~~~~~
*Parent repository for the NASA Planetary Data System (PDS) portal ecosystem. It serves as the central location for tracking update requests, tasks, and issues related to the pds.nasa.gov website.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://pds.nasa.gov>`_
     - `Github Repo <https://github.com/NASA-PDS/portal>`_
     - `Issue Tracking <https://github.com/NASA-PDS/portal/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/portal/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/portal/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/portal/releases>`_ 


Planned Updates
+++++++++++++++
`portal#143`_ B18 Website Support: High Priority Enhancements / Bug Fixes / Tasks
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+----------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                                            | I&T Status        | Level   | Priority / Bug Severity   |
+==================================================================================+===================+=========+===========================+
| `portal#144`_ Citing page does not link to correct PDS DOI policy document       | |:yellow_circle:| | bug     | s.medium                  |
+----------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| `portal#145`_ Feedback widget does not direct users to pds-operator@jpl.nasa.gov | |:yellow_circle:| | bug     | s.medium                  |
+----------------------------------------------------------------------------------+-------------------+---------+---------------------------+


--------

Component: Web Design
---------------------
*PDS Web Design System (WDS) components and implementations*

--------

Component: Web Dev
------------------
*Web development tools and demonstration applications*

--------

S3-browser-cloudfront
~~~~~~~~~~~~~~~~~~~~~
*Web view for files in S3 buckets*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/s3-browser-cloudfront#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/s3-browser-cloudfront>`_
     - `Issue Tracking <https://github.com/NASA-PDS/s3-browser-cloudfront/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/s3-browser-cloudfront/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/s3-browser-cloudfront/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/s3-browser-cloudfront/releases>`_ 


Planned Updates
+++++++++++++++
`s3-browser-cloudfront#138`_ S3 Browser Testing and Enhancements to Support LROC Launch
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

+-----------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                                                         | I&T Status        | Level   | Priority / Bug Severity   |
+===============================================================================================+===================+=========+===========================+
| `s3-browser-cloudfront#144`_ open-data-registry configuration broken by CloudFront PR changes | |:yellow_circle:| | bug     | p.must-have               |
+-----------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+


Other Updates
+++++++++++++
Requirements
^^^^^^^^^^^^

+----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                        | I&T Status        | Priority / Bug Severity   |
+==============================================================================================================================================+===================+===========================+
| `s3-browser-cloudfront#143`_ As a developer, I want the S3 browser to work with CloudFront as the S3 passthrough vs. direct S3 bucket access | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `s3-browser-cloudfront#158`_ As a developer, I need the ability to deep link into a bucket that is served via CloudFront                     | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `s3-browser-cloudfront#174`_ As a PDS Engineer, I want the domain of data paths for buckets we control to be automatically configured        | |:yellow_circle:| | unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `s3-browser-cloudfront#159`_ As a user, I need s3-browser to properly display breadcrumbs that include the bucket I chose                    | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Release Summary Metrics
=======================
This section provides a summary of the issues addressed in this release, organized by issue type.


+----------------------------+--------+----------------+----------------+---------+----------+---------+
| Component/Repo             | Bugs   | Enhancements   | Requirements   | Tasks   | Themes   | Total   |
+============================+========+================+================+=========+==========+=========+
| **Data Upload Manager**    | 1      | 0              | 0              | 0       | 1        | 2       |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **Devops**                 | 0      | 0              | 1              | 0       | 0        | 1       |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **Operations**             | 0      | 0              | 3              | 0       | 0        | 3       |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **PDS4 Information Model** | 4      | 2              | 1              | 0       | 7        | 14      |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **PDS4 Viewer**            | 1      | 1              | 1              | 0       | 0        | 3       |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **Peppi**                  | 1      | 0              | 1              | 0       | 1        | 3       |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **Registry Tools**         | 11     | 2              | 5              | 0       | 19       | 37      |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **System Tools**           | 0      | 0              | 1              | 0       | 0        | 1       |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **Validate**               | 3      | 1              | 2              | 0       | 2        | 8       |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **Web Content**            | 2      | 0              | 0              | 0       | 1        | 3       |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **Web Dev**                | 1      | 0              | 4              | 0       | 1        | 6       |
+----------------------------+--------+----------------+----------------+---------+----------+---------+
| **TOTAL**                  | **24** | **6**          | **19**         | **0**   | **32**   | **81**  |
+----------------------------+--------+----------------+----------------+---------+----------+---------+


Liens
=====

+---------+---------+-------------+
| Issue   | Title   | Rationale   |
+=========+=========+=============+
+---------+---------+-------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B18)`_

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

.. _plan B18: https://nasa-pds.github.io/releases/18/plan.html
.. _pds4-information-model#1002: https://github.com/NASA-PDS/pds4-information-model/issues/1002
.. _pds4-information-model#1003: https://github.com/NASA-PDS/pds4-information-model/issues/1003
.. _pds4-information-model#1004: https://github.com/NASA-PDS/pds4-information-model/issues/1004
.. _pds4-information-model#1005: https://github.com/NASA-PDS/pds4-information-model/issues/1005
.. _pds4-information-model#1006: https://github.com/NASA-PDS/pds4-information-model/issues/1006
.. _pds4-information-model#1007: https://github.com/NASA-PDS/pds4-information-model/issues/1007
.. _pds4-information-model#1008: https://github.com/NASA-PDS/pds4-information-model/issues/1008
.. _pds4-information-model#1032: https://github.com/NASA-PDS/pds4-information-model/issues/1032
.. _pds4-information-model#1033: https://github.com/NASA-PDS/pds4-information-model/issues/1033
.. _pds4-information-model#1034: https://github.com/NASA-PDS/pds4-information-model/issues/1034
.. _pds4-information-model#1035: https://github.com/NASA-PDS/pds4-information-model/issues/1035
.. _data-upload-manager#349: https://github.com/NASA-PDS/data-upload-manager/issues/349
.. _data-upload-manager#352: https://github.com/NASA-PDS/data-upload-manager/issues/352
.. _roundup-action#170: https://github.com/NASA-PDS/roundup-action/issues/170
.. _en-ops-utils#18: https://github.com/NASA-PDS/en-ops-utils/issues/18
.. _en-ops-utils#19: https://github.com/NASA-PDS/en-ops-utils/issues/19
.. _en-ops-utils#16: https://github.com/NASA-PDS/en-ops-utils/issues/16
.. _pds4-context-products#85: https://github.com/NASA-PDS/pds4-context-products/issues/85
.. _pds4-context-products#84: https://github.com/NASA-PDS/pds4-context-products/issues/84
.. _pds4-context-products#94: https://github.com/NASA-PDS/pds4-context-products/issues/94
.. _pds4-information-model#984: https://github.com/NASA-PDS/pds4-information-model/issues/984
.. _pds4-information-model#1014: https://github.com/NASA-PDS/pds4-information-model/issues/1014
.. _pds4-information-model#1047: https://github.com/NASA-PDS/pds4-information-model/issues/1047
.. _pds4-information-model#1015: https://github.com/NASA-PDS/pds4-information-model/issues/1015
.. _pds4-information-model#1016: https://github.com/NASA-PDS/pds4-information-model/issues/1016
.. _pds4-information-model#1017: https://github.com/NASA-PDS/pds4-information-model/issues/1017
.. _pds4-information-model#1026: https://github.com/NASA-PDS/pds4-information-model/issues/1026
.. _pds4-information-model#1042: https://github.com/NASA-PDS/pds4-information-model/issues/1042
.. _pds4-information-model#1049: https://github.com/NASA-PDS/pds4-information-model/issues/1049
.. _pds4-information-model#1038: https://github.com/NASA-PDS/pds4-information-model/issues/1038
.. _pds4-information-model#1040: https://github.com/NASA-PDS/pds4-information-model/issues/1040
.. _pds4-jparser#200: https://github.com/NASA-PDS/pds4-jparser/issues/200
.. _pds4-jparser#197: https://github.com/NASA-PDS/pds4-jparser/issues/197
.. _pds4-jparser#197: https://github.com/NASA-PDS/pds4-jparser/issues/197
.. _peppi#171: https://github.com/NASA-PDS/peppi/issues/171
.. _peppi#158: https://github.com/NASA-PDS/peppi/issues/158
.. _peppi#168: https://github.com/NASA-PDS/peppi/issues/168
.. _harvest#316: https://github.com/NASA-PDS/harvest/issues/316
.. _registry#266: https://github.com/NASA-PDS/registry/issues/266
.. _registry#371: https://github.com/NASA-PDS/registry/issues/371
.. _registry#432: https://github.com/NASA-PDS/registry/issues/432
.. _registry#498: https://github.com/NASA-PDS/registry/issues/498
.. _registry#497: https://github.com/NASA-PDS/registry/issues/497
.. _registry#509: https://github.com/NASA-PDS/registry/issues/509
.. _registry#517: https://github.com/NASA-PDS/registry/issues/517
.. _registry#510: https://github.com/NASA-PDS/registry/issues/510
.. _registry#510: https://github.com/NASA-PDS/registry/issues/510
.. _registry-api#715: https://github.com/NASA-PDS/registry-api/issues/715
.. _registry-api#617: https://github.com/NASA-PDS/registry-api/issues/617
.. _registry-api#682: https://github.com/NASA-PDS/registry-api/issues/682
.. _registry-api#698: https://github.com/NASA-PDS/registry-api/issues/698
.. _registry-api#708: https://github.com/NASA-PDS/registry-api/issues/708
.. _registry-api#729: https://github.com/NASA-PDS/registry-api/issues/729
.. _registry-api#727: https://github.com/NASA-PDS/registry-api/issues/727
.. _registry-api#749: https://github.com/NASA-PDS/registry-api/issues/749
.. _registry-api#751: https://github.com/NASA-PDS/registry-api/issues/751
.. _registry-api#760: https://github.com/NASA-PDS/registry-api/issues/760
.. _registry-api#768: https://github.com/NASA-PDS/registry-api/issues/768
.. _registry-api#742: https://github.com/NASA-PDS/registry-api/issues/742
.. _registry-api#745: https://github.com/NASA-PDS/registry-api/issues/745
.. _registry-api#748: https://github.com/NASA-PDS/registry-api/issues/748
.. _registry-api#744: https://github.com/NASA-PDS/registry-api/issues/744
.. _registry-api#611: https://github.com/NASA-PDS/registry-api/issues/611
.. _registry-loader#67: https://github.com/NASA-PDS/registry-loader/issues/67
.. _registry-loader#65: https://github.com/NASA-PDS/registry-loader/issues/65
.. _registry-loader#66: https://github.com/NASA-PDS/registry-loader/issues/66
.. _registry-loader#77: https://github.com/NASA-PDS/registry-loader/issues/77
.. _registry-mgr#72: https://github.com/NASA-PDS/registry-mgr/issues/72
.. _registry-sweepers#201: https://github.com/NASA-PDS/registry-sweepers/issues/201
.. _registry-sweepers#205: https://github.com/NASA-PDS/registry-sweepers/issues/205
.. _registry-sweepers#210: https://github.com/NASA-PDS/registry-sweepers/issues/210
.. _registry-sweepers#208: https://github.com/NASA-PDS/registry-sweepers/issues/208
.. _registry-sweepers#212: https://github.com/NASA-PDS/registry-sweepers/issues/212
.. _registry-sweepers#220: https://github.com/NASA-PDS/registry-sweepers/issues/220
.. _pds-agent-skills#6: https://github.com/NASA-PDS/pds-agent-skills/issues/6
.. _validate#1549: https://github.com/NASA-PDS/validate/issues/1549
.. _validate#1595: https://github.com/NASA-PDS/validate/issues/1595
.. _validate#1570: https://github.com/NASA-PDS/validate/issues/1570
.. _validate#1571: https://github.com/NASA-PDS/validate/issues/1571
.. _validate#1565: https://github.com/NASA-PDS/validate/issues/1565
.. _validate#1568: https://github.com/NASA-PDS/validate/issues/1568
.. _validate#1548: https://github.com/NASA-PDS/validate/issues/1548
.. _validate#1601: https://github.com/NASA-PDS/validate/issues/1601
.. _portal#143: https://github.com/NASA-PDS/portal/issues/143
.. _portal#144: https://github.com/NASA-PDS/portal/issues/144
.. _portal#145: https://github.com/NASA-PDS/portal/issues/145
.. _s3-browser-cloudfront#138: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/138
.. _s3-browser-cloudfront#144: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/144
.. _s3-browser-cloudfront#143: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/143
.. _s3-browser-cloudfront#158: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/158
.. _s3-browser-cloudfront#174: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/174
.. _s3-browser-cloudfront#159: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/159
.. _Software Release Summary (B18): https://nasa-pds.github.io/releases/18/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md