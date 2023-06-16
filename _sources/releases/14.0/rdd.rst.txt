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

+-------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                |I&T Status          |Priority / Bug Severity   |
+=====================================================================================+====================+==========================+
|`devops#35`_ As a EN team member, I want to check the API test reports in testrail   ||:yellow_circle:|   |unknown                   |
+-------------------------------------------------------------------------------------+--------------------+--------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                         |I&T Status          |Priority / Bug Severity   |
+==============================================================================+====================+==========================+
|`nucleus#22`_ As a user, I want to deploy a baseline nucleus automatically.   ||:yellow_circle:|   |p.should-have             |
+------------------------------------------------------------------------------+--------------------+--------------------------+
|`nucleus#24`_ As a user, I want to configure a nucleus pipeline               ||:yellow_circle:|   |p.must-have               |
+------------------------------------------------------------------------------+--------------------+--------------------------+
|`nucleus#23`_ As a user, I want to monitor a nucleus workflow execution       ||:yellow_circle:|   |p.must-have               |
+------------------------------------------------------------------------------+--------------------+--------------------------+
|`nucleus#27`_ As a user, I want to estimate the cost for a new deployment     ||:yellow_circle:|   |p.must-have               |
+------------------------------------------------------------------------------+--------------------+--------------------------+

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
|`pds-api#260`_ PDS API documents are unclear wrt quoting in queries         ||:yellow_circle:|   |unknown                   |
+----------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#262`_ PDS API is not respecting the sort field                     ||:yellow_circle:|   |unknown                   |
+----------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#259`_ API search returns 500 for anything besides simple queries   ||:yellow_circle:|   |unknown                   |
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

+-------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                          |I&T Status          |Priority / Bug Severity   |
+===============================================================================+====================+==========================+
|`pds4-information-model#658`_ Bug trying to generate LDD and missing files     ||:yellow_circle:|   |s.high                    |
+-------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds4-information-model#661`_ LDDTool fails for dependent LDDs since v14.2.0   ||:yellow_circle:|   |s.critical                |
+-------------------------------------------------------------------------------+--------------------+--------------------------+

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

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                              |I&T Status        |Priority / Bug Severity   |
+===================================================================+==================+==========================+
|`registry#180`_ Provenance script failing on production registry   ||:blue_circle:|   |s.high                    |
+-------------------------------------------------------------------+------------------+--------------------------+

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
|`registry-api#296`_ API crashes with JVM memory error on data sets with very large labels (>1MB)   ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#305`_ API not returning value for NAIF bundles                                       ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#277`_ Product summary object has an incomplete "properties" set                      ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------+--------------------+--------------------------+

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
|`validate#7`_ Update to support ComplexLSB8 data types and investigate Floating point exception             ||:yellow_circle:|   |enhancement   |p.should-have             |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#190`_ Validation fails to catch real value in ASCII_NonNegative_Integer field (Table_Delimited)   ||:yellow_circle:|   |bug           |s.medium                  |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#217`_ As a user, I want to validate content for all possible PDS4 table types                     ||:yellow_circle:|   |requirement   |p.must-have               |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#343`_ As a user I want to see the name of a table/array in errors, if one is specified            ||:yellow_circle:|   |requirement   |p.could-have              |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#431`_ warning.table.characters_between_fields missing for last record in table                    ||:yellow_circle:|   |bug           |s.low                     |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#476`_ As a user, I want to check that are no duplicate LIDs/LIDVIDs in a File_Area_Inventory      ||:yellow_circle:|   |requirement   |p.should-have             |
+------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


`validate#607`_ Support for Improved Datetime Checks
++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                          |I&T Status          |Level         |Priority / Bug Severity   |
+===============================================================+====================+==============+==========================+
|`validate#608`_ Update datetime regex for content validation   ||:yellow_circle:|   |enhancement   |p.must-have               |
+---------------------------------------------------------------+--------------------+--------------+--------------------------+


`validate#629`_ Add Check for Schematron/Schema Version Mismatch
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                                                                        |I&T Status          |Level         |Priority / Bug Severity   |
+=============================================================================================================================+====================+==============+==========================+
|`validate#628`_ As a user, I want to throw a WARNING when a product's schematron version does not match the schema version   ||:yellow_circle:|   |requirement   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                   |I&T Status          |Priority / Bug Severity   |
+========================================================================================================================+====================+==========================+
|`validate#649`_ validate does not validate a collection if collection.xml pointed to                                    ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#644`_ Validate gives errors for 'NaN' and 'Inf' values in IEEE754 data                                        ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#561`_ Validate incorrectly enforces file naming requirements on bundles/collections                           ||:yellow_circle:|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#500`_ Validate does not allow `.arch_h` file name/data type                                                   ||:yellow_circle:|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#631`_ Expected value in validate report for context reference name is not same as value in the context file   ||:yellow_circle:|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#652`_ validate 3.3.0 snapshot produces incorrect SKIP/INFO messages                                           ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                      |I&T Status          |Priority / Bug Severity   |
+===========================================================================================================================================+====================+==========================+
|`validate#599`_ As a user, I want to be able to use both online and local schema/schematron files.                                         ||:yellow_circle:|   |p.could-have              |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#462`_ As a user, I want validate to throw an error when a collection inventory contains an invalid secondary product reference   ||:yellow_circle:|   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#604`_ As a user, I want to validate MP4/H.264 encoded video as observational data                                                ||:yellow_circle:|   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#617`_ As a user, I would like to enforce browse file extension with encoding type                                                ||:yellow_circle:|   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#605`_ As a user, I want to validate MP4/H.264/AAC encoded video with audio as observational data                                 ||:yellow_circle:|   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                              |I&T Status        |Priority / Bug Severity   |
+===================================================================================+==================+==========================+
|`validate#567`_ Update ArrayObject exceptions to enable improved error messaging   ||:blue_circle:|   |p.could-have              |
+-----------------------------------------------------------------------------------+------------------+--------------------------+

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
.. _deep-archive#147: https://github.com/NASA-PDS/deep-archive/issues/147
.. _devops#34: https://github.com/NASA-PDS/devops/issues/34
.. _devops#35: https://github.com/NASA-PDS/devops/issues/35
.. _nucleus#22: https://github.com/NASA-PDS/nucleus/issues/22
.. _nucleus#24: https://github.com/NASA-PDS/nucleus/issues/24
.. _nucleus#23: https://github.com/NASA-PDS/nucleus/issues/23
.. _nucleus#27: https://github.com/NASA-PDS/nucleus/issues/27
.. _pds-api#260: https://github.com/NASA-PDS/pds-api/issues/260
.. _pds-api#262: https://github.com/NASA-PDS/pds-api/issues/262
.. _pds-api#259: https://github.com/NASA-PDS/pds-api/issues/259
.. _pds4-information-model#658: https://github.com/NASA-PDS/pds4-information-model/issues/658
.. _pds4-information-model#661: https://github.com/NASA-PDS/pds4-information-model/issues/661
.. _registry#143: https://github.com/NASA-PDS/registry/issues/143
.. _registry#180: https://github.com/NASA-PDS/registry/issues/180
.. _registry-api#296: https://github.com/NASA-PDS/registry-api/issues/296
.. _registry-api#305: https://github.com/NASA-PDS/registry-api/issues/305
.. _registry-api#277: https://github.com/NASA-PDS/registry-api/issues/277
.. _registry-loader#26: https://github.com/NASA-PDS/registry-loader/issues/26
.. _software-issues-repo#63: https://github.com/NASA-PDS/software-issues-repo/issues/63
.. _validate#534: https://github.com/NASA-PDS/validate/issues/534
.. _validate#7: https://github.com/NASA-PDS/validate/issues/7
.. _validate#190: https://github.com/NASA-PDS/validate/issues/190
.. _validate#217: https://github.com/NASA-PDS/validate/issues/217
.. _validate#343: https://github.com/NASA-PDS/validate/issues/343
.. _validate#431: https://github.com/NASA-PDS/validate/issues/431
.. _validate#476: https://github.com/NASA-PDS/validate/issues/476
.. _validate#607: https://github.com/NASA-PDS/validate/issues/607
.. _validate#608: https://github.com/NASA-PDS/validate/issues/608
.. _validate#629: https://github.com/NASA-PDS/validate/issues/629
.. _validate#628: https://github.com/NASA-PDS/validate/issues/628
.. _validate#649: https://github.com/NASA-PDS/validate/issues/649
.. _validate#644: https://github.com/NASA-PDS/validate/issues/644
.. _validate#561: https://github.com/NASA-PDS/validate/issues/561
.. _validate#500: https://github.com/NASA-PDS/validate/issues/500
.. _validate#631: https://github.com/NASA-PDS/validate/issues/631
.. _validate#652: https://github.com/NASA-PDS/validate/issues/652
.. _validate#599: https://github.com/NASA-PDS/validate/issues/599
.. _validate#462: https://github.com/NASA-PDS/validate/issues/462
.. _validate#604: https://github.com/NASA-PDS/validate/issues/604
.. _validate#617: https://github.com/NASA-PDS/validate/issues/617
.. _validate#605: https://github.com/NASA-PDS/validate/issues/605
.. _validate#567: https://github.com/NASA-PDS/validate/issues/567
.. _web-analytics#3: https://github.com/NASA-PDS/web-analytics/issues/3
.. _web-modernization#194: https://github.com/NASA-PDS/web-modernization/issues/194
.. _Software Release Summary (B14.0): https://nasa-pds.github.io/releases/14.0/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
