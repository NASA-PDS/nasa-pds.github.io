==========================================
Release Description Document (Build B14.0)
==========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B14.0`_

The following sections can be found in this document:

.. toctree::
   :glob: 
   :maxdepth: 3

   rdd.rst

PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Board
and implemented by the PDS within the latest build period.

No PDS4 Standards Updates

Software Changes
================
The changes types are 'Bug', 'Enhancement' or 'Requirement'. For each software repository, the changes are listed in 2
categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B14.0`_)
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
`cloud-tasks#29`_ Migrate Web Analytics prototype to PDS Cloud
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`cloud-tasks#65`_ Initial NGAP-to-MCP Migration Research
++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

--------

Data-upload-manager
-------------------
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
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+--------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                       |I&T Status          |Priority / Bug Severity   |
+============================================================================================+====================+==========================+
|`data-upload-manager#24`_ As a user, I want to parallelize upload of data products to PDC   ||:yellow_circle:|   |p.should-have             |
+--------------------------------------------------------------------------------------------+--------------------+--------------------------+

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

+-----------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                              |I&T Status        |Priority / Bug Severity   |
+===================================================================================+==================+==========================+
|`deep-archive#147`_ Jenkins Deep Regsitry Archive ran for the first time, failed   ||:blue_circle:|   |unknown                   |
+-----------------------------------------------------------------------------------+------------------+--------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================================+====================+==========================+
|`devops#34`_ jenkins continuous deployment does not pull docker images   ||:yellow_circle:|   |s.critical                |
+-------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                      |I&T Status          |Priority / Bug Severity   |
+===========================================================================================================+====================+==========================+
|`devops#50`_ As a user, I want PDS EN produced Docker images to support multiple platforms (x86 and ARM)   ||:yellow_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`devops#35`_ As a EN team member, I want to check the API test reports in testrail                         ||:yellow_circle:|   |unknown                   |
+-----------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

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

+---------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                |I&T Status          |Priority / Bug Severity   |
+=====================================================================+====================+==========================+
|`doi-service#408`_ Sync script is pushing non-findable DOIs to ADS   ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------+--------------------+--------------------------+

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

+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                              |I&T Status          |Priority / Bug Severity   |
+===================================================================================================+====================+==========================+
|`harvest#124`_ Access forbidden during nominal pipeline execution of harvest on Mars2020 archive   ||:yellow_circle:|   |s.critical                |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                              |I&T Status          |Priority / Bug Severity   |
+===================================================================================================+====================+==========================+
|`harvest#119`_ As a developer, I want to know what version of Harvest was used to load a product   ||:yellow_circle:|   |p.should-have             |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Nucleus
-------
*Nucleus is a software platform used to create workflows for the Planetary Data (PDS).*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/nucleus>`_
     - `Github Repo <https://github.com/NASA-PDS/nucleus>`_
     - `Issue Tracking <https://github.com/NASA-PDS/nucleus/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/nucleus/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/nucleus/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/nucleus/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`nucleus#38`_ Develop Logging and Monitoring Strategy
+++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`nucleus#39`_ Operationalize Nucleus for Initial CSS Prototype
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                         |I&T Status          |Level         |Priority / Bug Severity   |
+==============================================================================+====================+==============+==========================+
|`nucleus#22`_ As a user, I want to deploy a baseline nucleus automatically.   ||:yellow_circle:|   |requirement   |p.should-have             |
+------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`nucleus#23`_ As a user, I want to monitor a nucleus workflow execution       ||:yellow_circle:|   |requirement   |p.must-have               |
+------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`nucleus#24`_ As a user, I want to configure a nucleus pipeline               ||:yellow_circle:|   |requirement   |p.must-have               |
+------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`nucleus#27`_ As a user, I want to estimate the cost for a new deployment     ||:yellow_circle:|   |requirement   |p.must-have               |
+------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


`nucleus#41`_ Determine DAG definition standard
+++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+
|Issue                                                                                                |I&T Status          |Level   |Priority / Bug Severity   |
+=====================================================================================================+====================+========+==========================+
|`nucleus#51`_ Evaluate the ability to create Nucleus workflow using CWL (Common Workflow Language)   ||:yellow_circle:|   |task    |unknown                   |
+-----------------------------------------------------------------------------------------------------+--------------------+--------+--------------------------+


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
`operations#364`_ B13.1 Deploy and Release
++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                   |I&T Status          |Priority / Bug Severity   |
+========================================================================================================+====================+==========================+
|`operations#413`_ Monthly Metrics are not generating for EN the (1) tool metrics or (2) other reports   ||:yellow_circle:|   |unknown                   |
+--------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                 |I&T Status          |Priority / Bug Severity   |
+======================================================================================+====================+==========================+
|`operations#414`_ [ldd-request] Create new LDD "mgn"                                  ||:yellow_circle:|   |p.must-have               |
+--------------------------------------------------------------------------------------+--------------------+--------------------------+
|`operations#378`_ Develop script to enhance sitemap with data set landing page URLs   ||:blue_circle:|     |p.should-have             |
+--------------------------------------------------------------------------------------+--------------------+--------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                       |I&T Status          |Priority / Bug Severity   |
+============================================================================+====================+==========================+
|`pds-api#259`_ API search returns 500 for anything besides simple queries   ||:yellow_circle:|   |unknown                   |
+----------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#260`_ PDS API documents are unclear wrt quoting in queries         ||:yellow_circle:|   |unknown                   |
+----------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#262`_ PDS API is not respecting the sort field                     ||:yellow_circle:|   |unknown                   |
+----------------------------------------------------------------------------+--------------------+--------------------------+

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

+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================================================================+====================+==========================+
|`pds4-information-model#667`_ lddtool does not generate the correct closing tag for rule_type = Report   ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds4-information-model#658`_ Bug trying to generate LDD and missing files                               ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds4-information-model#661`_ LDDTool fails for dependent LDDs since v14.2.0                             ||:yellow_circle:|   |s.critical                |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                               |I&T Status          |Priority / Bug Severity   |
+====================================================================+====================+==========================+
|`pds4-information-model#651`_ Add TermMaps to default output JSON   ||:yellow_circle:|   |p.should-have             |
+--------------------------------------------------------------------+--------------------+--------------------------+

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
`portal-tasks#64`_ Fix and Improve pds.nasa.gov SEO
+++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

--------

Portal-wp-tasks
---------------
*PDS Web Design System*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pds-wds>`_
     - `Github Repo <https://github.com/NASA-PDS/portal-wp-tasks>`_
     - `Issue Tracking <https://github.com/NASA-PDS/portal-wp-tasks/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/portal-wp-tasks/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/portal-wp-tasks/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/portal-wp-tasks/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`portal-wp-tasks#37`_ Enhancing Initial Search Prototype Implementation Based Upon User Testing
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

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
`registry#143`_ Preparations for B13.1 Registry Updates
+++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

`registry#186`_ Enhance Terraform Scripts for Continuous Deployment and MCP
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                              |I&T Status        |Priority / Bug Severity   |
+===================================================================+==================+==========================+
|`registry#180`_ Provenance script failing on production registry   ||:blue_circle:|   |s.high                    |
+-------------------------------------------------------------------+------------------+--------------------------+
|`registry#213`_ Increase disk space for ATM opensearch             ||:blue_circle:|   |s.critical                |
+-------------------------------------------------------------------+------------------+--------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                                                           |I&T Status        |Priority / Bug Severity   |
+================================================================================================================+==================+==========================+
|`registry#211`_ As an operator, I want to be notified of when Registry storage capacity exceeds 75% capacity.   ||:blue_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------+------------------+--------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                              |I&T Status          |Priority / Bug Severity   |
+===================================================================================================+====================+==========================+
|`registry-api#349`_ Request for json+pds4 response fails in production                             ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#262`_ the request url in the error message does not make sense                       ||:yellow_circle:|   |s.low                     |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#362`_ field case in response and query have mismatched cases                         ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#277`_ Product summary object has an incomplete "properties" set                      ||:green_circle:|    |s.medium                  |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#341`_ members of a bundle does not work on new test dataset                          ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#355`_ api does not return information that OpenSearch says is public                 ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#356`_ `Accept:*` response not defaulting to valid application/json                   ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#343`_ API falsely reports 10000 hits for hits>10000                                  ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#305`_ API not returning value for NAIF bundles                                       ||:green_circle:|    |s.high                    |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#296`_ API crashes with JVM memory error on data sets with very large labels (>1MB)   ||:green_circle:|    |s.medium                  |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                              |I&T Status          |Priority / Bug Severity   |
+===================================================================================================================================+====================+==========================+
|`registry-api#336`_ As a PDS operator, I want to know the health of the registry API service                                       ||:green_circle:|    |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#361`_ As a user, I want my API request to execute successfully even when the registry contains corrupted documents   ||:yellow_circle:|   |p.could-have              |
+-----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Registry-loader
---------------
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
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                         |I&T Status          |Priority / Bug Severity   |
+==============================================================================+====================+==========================+
|`registry-loader#26`_ Stable Roundup can no longer trigger Imaging workflow   ||:yellow_circle:|   |unknown                   |
+------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Registry-sweepers
-----------------
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
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                 |I&T Status          |Priority / Bug Severity   |
+======================================================================================================================+====================+==========================+
|`registry-sweepers#34`_ Provenance bulk update db writes fail under specific conditions related to presence of CCRs   ||:yellow_circle:|   |s.critical                |
+----------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

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
Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                                                             |I&T Status        |Priority / Bug Severity   |
+==================================================================================================================+==================+==========================+
|`roundup-action#116`_ As a developer, I want the Roundup Action to use the newly split pds-github-util commands   ||:blue_circle:|   |unknown                   |
+------------------------------------------------------------------------------------------------------------------+------------------+--------------------------+

--------

Search-api-notebook
-------------------
*Jupyter notebooks for demonstrating and utilizing the Planetary Data System (PDS) Search API*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/search-api-notebook#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/search-api-notebook>`_
     - `Issue Tracking <https://github.com/NASA-PDS/search-api-notebook/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/search-api-notebook/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/search-api-notebook/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/search-api-notebook/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`search-api-notebook#10`_ Prototype integration of pyWWT and PDS Search API in Jupyter
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

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
`software-issues-repo#63`_ B14.0 Release Planning
+++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

--------

Transform
---------
*Transforms PDS3 and PDS4 product labels and data into various formats.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/transform/>`_
     - `Github Repo <https://github.com/NASA-PDS/transform>`_
     - `Issue Tracking <https://github.com/NASA-PDS/transform/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/transform/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/transform/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/transform/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------+--------------------+--------------------------+
|Issue                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================+====================+==========================+
|`transform#35`_ Examples missing from tar/zip packages   ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------+--------------------+--------------------------+

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
`validate#534`_ B14.0 Content Validation Improvements: Additional Table Types, Additional File Areas
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                                                       |I&T Status          |Level         |Priority / Bug Severity   |
+============================================================================================================+====================+==============+==========================+
|`validate#7`_ Update to support ComplexLSB8 data types and investigate Floating point exception             ||:green_circle:|    |enhancement   |p.should-have             |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#190`_ Validation fails to catch real value in ASCII_NonNegative_Integer field (Table_Delimited)   ||:green_circle:|    |bug           |s.medium                  |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#217`_ As a user, I want to validate content for all possible PDS4 table types                     ||:green_circle:|    |requirement   |p.must-have               |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#343`_ As a user I want to see the name of a table/array in errors, if one is specified            ||:yellow_circle:|   |requirement   |p.could-have              |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#431`_ warning.table.characters_between_fields missing for last record in table                    ||:green_circle:|    |bug           |s.low                     |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#476`_ As a user, I want to check that are no duplicate LIDs/LIDVIDs in a File_Area_Inventory      ||:green_circle:|    |requirement   |p.should-have             |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


`validate#606`_ Support for Encoded Video and Encoded Audio
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                                                        |I&T Status          |Level         |Priority / Bug Severity   |
+=============================================================================================================+====================+==============+==========================+
|`validate#604`_ As a user, I want to validate MP4/H.264 encoded video as observational data                  ||:green_circle:|    |requirement   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#605`_ As a user, I want to validate MP4/H.264/AAC encoded video with audio as observational data   ||:yellow_circle:|   |requirement   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#662`_ As a user, I want to validate WAV encoded audio as observational data                        ||:yellow_circle:|   |requirement   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#663`_ As a user, I want to validate M4A/AAC encoded audio as observational data                    ||:yellow_circle:|   |requirement   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


`validate#607`_ Support for Improved Datetime Checks
++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                          |I&T Status          |Level         |Priority / Bug Severity   |
+===============================================================+====================+==============+==========================+
|`validate#608`_ Update datetime regex for content validation   ||:yellow_circle:|   |enhancement   |p.must-have               |
+---------------------------------------------------------------+--------------------+--------------+--------------------------+


`validate#610`_ B14.0 Enhancements to Initial Version of Registry Referential Integrity Validator
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|Issue                                                                                     |I&T Status         |Level         |Priority / Bug Severity   |
+==========================================================================================+===================+==============+==========================+
|`validate#643`_ Document how to use validate-refs tool in Validate Operation User Guide   ||:green_circle:|   |enhancement   |p.must-have               |
+------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+


`validate#629`_ Add Check for Schematron/Schema Version Mismatch
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+
|Issue                                                                                                                        |I&T Status         |Level         |Priority / Bug Severity   |
+=============================================================================================================================+===================+==============+==========================+
|`validate#628`_ As a user, I want to throw a WARNING when a product's schematron version does not match the schema version   ||:green_circle:|   |requirement   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------+-------------------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                             |I&T Status          |Priority / Bug Severity   |
+==================================================================================================================================+====================+==========================+
|`validate#479`_ validate erroneously flags PDF/A-1a compliant file                                                                ||:green_circle:|    |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#673`_ Validate does not handle Special_Constants valid_minimum and valid_maximum in accordance with information model   ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#649`_ validate does not validate a collection if collection.xml pointed to                                              ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#674`_ validate does not handle special constants with data type of SignedLSB2                                           ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#500`_ Validate does not allow `.arch_h` file name/data type                                                             ||:green_circle:|    |s.low                     |
+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#561`_ Validate incorrectly enforces file naming requirements on bundles/collections                                     ||:green_circle:|    |s.low                     |
+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#631`_ Expected value in validate report for context reference name is not same as value in the context file             ||:green_circle:|    |s.low                     |
+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#652`_ validate 3.3.0 snapshot produces incorrect SKIP/INFO messages                                                     ||:green_circle:|    |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#644`_ Validate gives errors for 'NaN' and 'Inf' values in IEEE754 data                                                  ||:green_circle:|    |s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                      |I&T Status          |Priority / Bug Severity   |
+===========================================================================================================================================+====================+==========================+
|`validate#658`_ As a user, I want the PDF error reports to be output in a user-specified directory                                         ||:yellow_circle:|   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#651`_ As a user, I want to support bit patterns within Special_Constants values                                                  ||:yellow_circle:|   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#617`_ As a user, I would like to enforce browse file extension with encoding type                                                ||:yellow_circle:|   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#462`_ As a user, I want validate to throw an error when a collection inventory contains an invalid secondary product reference   ||:yellow_circle:|   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#599`_ As a user, I want to be able to use both online and local schema/schematron files.                                         ||:yellow_circle:|   |p.could-have              |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                              |I&T Status        |Priority / Bug Severity   |
+===================================================================================+==================+==========================+
|`validate#567`_ Update ArrayObject exceptions to enable improved error messaging   ||:blue_circle:|   |p.could-have              |
+-----------------------------------------------------------------------------------+------------------+--------------------------+

--------

Wds-react
---------
*PDS Web Design System - React Implementation*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/wds-react>`_
     - `Github Repo <https://github.com/NASA-PDS/wds-react>`_
     - `Issue Tracking <https://github.com/NASA-PDS/wds-react/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/wds-react/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/wds-react/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/wds-react/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                       |I&T Status          |Priority / Bug Severity   |
+============================================================+====================+==========================+
|`wds-react#88`_ A debug content shows in the document tab   ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------+--------------------+--------------------------+

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

+-------------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                                |I&T Status        |Priority / Bug Severity   |
+=====================================================================================+==================+==========================+
|`web-analytics#9`_ Dashboard: EN Search Query analytics - queries over time period   ||:blue_circle:|   |p.must-have               |
+-------------------------------------------------------------------------------------+------------------+--------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                                    |I&T Status        |Priority / Bug Severity   |
+=========================================================================================+==================+==========================+
|`web-analytics#3`_ Migrate PDS Web Analytics dashboards in PDS-managed AWS environment   ||:blue_circle:|   |p.should-have             |
+-----------------------------------------------------------------------------------------+------------------+--------------------------+

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
`web-modernization#194`_ Analyze Usability Testing Data
+++++++++++++++++++++++++++++++++++++++++++++++++++++++
No requirements, significant enhancements, or bug fixes identified for this Build. See theme for more details.

Liens
=====

+--------+--------+------------+
|Issue   |Title   |Rationale   |
+========+========+============+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B14.0)`_

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

.. _plan B14.0: https://nasa-pds.github.io/releases/14.0/plan.html
.. _cloud-tasks#29: https://github.com/NASA-PDS/cloud-tasks/issues/29
.. _cloud-tasks#65: https://github.com/NASA-PDS/cloud-tasks/issues/65
.. _data-upload-manager#24: https://github.com/NASA-PDS/data-upload-manager/issues/24
.. _deep-archive#147: https://github.com/NASA-PDS/deep-archive/issues/147
.. _devops#34: https://github.com/NASA-PDS/devops/issues/34
.. _devops#50: https://github.com/NASA-PDS/devops/issues/50
.. _devops#35: https://github.com/NASA-PDS/devops/issues/35
.. _doi-service#408: https://github.com/NASA-PDS/doi-service/issues/408
.. _harvest#124: https://github.com/NASA-PDS/harvest/issues/124
.. _harvest#119: https://github.com/NASA-PDS/harvest/issues/119
.. _nucleus#38: https://github.com/NASA-PDS/nucleus/issues/38
.. _nucleus#39: https://github.com/NASA-PDS/nucleus/issues/39
.. _nucleus#22: https://github.com/NASA-PDS/nucleus/issues/22
.. _nucleus#23: https://github.com/NASA-PDS/nucleus/issues/23
.. _nucleus#24: https://github.com/NASA-PDS/nucleus/issues/24
.. _nucleus#27: https://github.com/NASA-PDS/nucleus/issues/27
.. _nucleus#41: https://github.com/NASA-PDS/nucleus/issues/41
.. _nucleus#51: https://github.com/NASA-PDS/nucleus/issues/51
.. _operations#364: https://github.com/NASA-PDS/operations/issues/364
.. _operations#413: https://github.com/NASA-PDS/operations/issues/413
.. _operations#414: https://github.com/NASA-PDS/operations/issues/414
.. _operations#378: https://github.com/NASA-PDS/operations/issues/378
.. _pds-api#259: https://github.com/NASA-PDS/pds-api/issues/259
.. _pds-api#260: https://github.com/NASA-PDS/pds-api/issues/260
.. _pds-api#262: https://github.com/NASA-PDS/pds-api/issues/262
.. _pds4-information-model#667: https://github.com/NASA-PDS/pds4-information-model/issues/667
.. _pds4-information-model#658: https://github.com/NASA-PDS/pds4-information-model/issues/658
.. _pds4-information-model#661: https://github.com/NASA-PDS/pds4-information-model/issues/661
.. _pds4-information-model#651: https://github.com/NASA-PDS/pds4-information-model/issues/651
.. _portal-tasks#64: https://github.com/NASA-PDS/portal-tasks/issues/64
.. _portal-wp-tasks#37: https://github.com/NASA-PDS/portal-wp-tasks/issues/37
.. _registry#143: https://github.com/NASA-PDS/registry/issues/143
.. _registry#186: https://github.com/NASA-PDS/registry/issues/186
.. _registry#180: https://github.com/NASA-PDS/registry/issues/180
.. _registry#213: https://github.com/NASA-PDS/registry/issues/213
.. _registry#211: https://github.com/NASA-PDS/registry/issues/211
.. _registry-api#349: https://github.com/NASA-PDS/registry-api/issues/349
.. _registry-api#262: https://github.com/NASA-PDS/registry-api/issues/262
.. _registry-api#362: https://github.com/NASA-PDS/registry-api/issues/362
.. _registry-api#277: https://github.com/NASA-PDS/registry-api/issues/277
.. _registry-api#341: https://github.com/NASA-PDS/registry-api/issues/341
.. _registry-api#355: https://github.com/NASA-PDS/registry-api/issues/355
.. _registry-api#356: https://github.com/NASA-PDS/registry-api/issues/356
.. _registry-api#343: https://github.com/NASA-PDS/registry-api/issues/343
.. _registry-api#305: https://github.com/NASA-PDS/registry-api/issues/305
.. _registry-api#296: https://github.com/NASA-PDS/registry-api/issues/296
.. _registry-api#336: https://github.com/NASA-PDS/registry-api/issues/336
.. _registry-api#361: https://github.com/NASA-PDS/registry-api/issues/361
.. _registry-loader#26: https://github.com/NASA-PDS/registry-loader/issues/26
.. _registry-sweepers#34: https://github.com/NASA-PDS/registry-sweepers/issues/34
.. _roundup-action#116: https://github.com/NASA-PDS/roundup-action/issues/116
.. _search-api-notebook#10: https://github.com/NASA-PDS/search-api-notebook/issues/10
.. _software-issues-repo#63: https://github.com/NASA-PDS/software-issues-repo/issues/63
.. _transform#35: https://github.com/NASA-PDS/transform/issues/35
.. _validate#534: https://github.com/NASA-PDS/validate/issues/534
.. _validate#7: https://github.com/NASA-PDS/validate/issues/7
.. _validate#190: https://github.com/NASA-PDS/validate/issues/190
.. _validate#217: https://github.com/NASA-PDS/validate/issues/217
.. _validate#343: https://github.com/NASA-PDS/validate/issues/343
.. _validate#431: https://github.com/NASA-PDS/validate/issues/431
.. _validate#476: https://github.com/NASA-PDS/validate/issues/476
.. _validate#606: https://github.com/NASA-PDS/validate/issues/606
.. _validate#604: https://github.com/NASA-PDS/validate/issues/604
.. _validate#605: https://github.com/NASA-PDS/validate/issues/605
.. _validate#662: https://github.com/NASA-PDS/validate/issues/662
.. _validate#663: https://github.com/NASA-PDS/validate/issues/663
.. _validate#607: https://github.com/NASA-PDS/validate/issues/607
.. _validate#608: https://github.com/NASA-PDS/validate/issues/608
.. _validate#610: https://github.com/NASA-PDS/validate/issues/610
.. _validate#643: https://github.com/NASA-PDS/validate/issues/643
.. _validate#629: https://github.com/NASA-PDS/validate/issues/629
.. _validate#628: https://github.com/NASA-PDS/validate/issues/628
.. _validate#479: https://github.com/NASA-PDS/validate/issues/479
.. _validate#673: https://github.com/NASA-PDS/validate/issues/673
.. _validate#649: https://github.com/NASA-PDS/validate/issues/649
.. _validate#674: https://github.com/NASA-PDS/validate/issues/674
.. _validate#500: https://github.com/NASA-PDS/validate/issues/500
.. _validate#561: https://github.com/NASA-PDS/validate/issues/561
.. _validate#631: https://github.com/NASA-PDS/validate/issues/631
.. _validate#652: https://github.com/NASA-PDS/validate/issues/652
.. _validate#644: https://github.com/NASA-PDS/validate/issues/644
.. _validate#658: https://github.com/NASA-PDS/validate/issues/658
.. _validate#651: https://github.com/NASA-PDS/validate/issues/651
.. _validate#617: https://github.com/NASA-PDS/validate/issues/617
.. _validate#462: https://github.com/NASA-PDS/validate/issues/462
.. _validate#599: https://github.com/NASA-PDS/validate/issues/599
.. _validate#567: https://github.com/NASA-PDS/validate/issues/567
.. _wds-react#88: https://github.com/NASA-PDS/wds-react/issues/88
.. _web-analytics#9: https://github.com/NASA-PDS/web-analytics/issues/9
.. _web-analytics#3: https://github.com/NASA-PDS/web-analytics/issues/3
.. _web-modernization#194: https://github.com/NASA-PDS/web-modernization/issues/194
.. _Software Release Summary (B14.0): https://nasa-pds.github.io/releases/14.0/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
