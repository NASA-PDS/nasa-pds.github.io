==========================================
Release Description Document (Build B14.1)
==========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B14.1`_

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
For each software repository, the changes are listed in 2 categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B14.1`_).

The 'Other Updates' occurs during the build cycle without being planned or attached to a theme. They are organized by
types (bug, enhancements, requirements, tasks). Any updates that require a de-scope of planned tasks are reviewed by the
PDS Software Working Group.

The deliveries are validated by the development team and go through an additional Integration & Test process, as
applicable, as indicated by the ```Testing Status``` column in the tables below. There are 3 possible statuses for
testing:

- |:blue_circle:| Skip Testing - Testing is not needed for this ticket. These are determined at the discretion of the team based upon the technical or operational nature of the closed task.
- |:yellow_circle:| Testing Needed
- |:green_circle:| Testing Complete - Initial testing complete, and test cases/results documented.

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

+-------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================================+====================+==========================+
|`deep-archive#151`_ Installation instructions don't work on Windows 11   ||:yellow_circle:|   |s.medium                  |
+-------------------------------------------------------------------------+--------------------+--------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                  |I&T Status          |Priority / Bug Severity   |
+=======================================================================================================================+====================+==========================+
|`doi-ui#215`_ When the cognito token is expired, the UI fails and returns a misleading/badly formatted error message   ||:yellow_circle:|   |s.high                    |
+-----------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Ds-view
-------
*Data Set View application (pds.nasa.gov/ds-view)*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/ds-view#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/ds-view>`_
     - `Issue Tracking <https://github.com/NASA-PDS/ds-view/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/ds-view/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/ds-view/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/ds-view/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                   |I&T Status          |Priority / Bug Severity   |
+========================================================================+====================+==========================+
|`ds-view#14`_ Memory leak in Solr connections leading to Tomcat crash   ||:yellow_circle:|   |s.critical                |
+------------------------------------------------------------------------+--------------------+--------------------------+
|`ds-view#12`_ v2.14.2 does not work for resource links                  ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                     |I&T Status          |Priority / Bug Severity   |
+==========================================================================================+====================+==========================+
|`ds-view#3`_ Upgrade Dataset View and dependencies to support Harvest/Registry upgrades   ||:yellow_circle:|   |p.must-have               |
+------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`ds-view#8`_ Upgrade to latest Solr 9.3.x                                                 ||:blue_circle:|     |unknown                   |
+------------------------------------------------------------------------------------------+--------------------+--------------------------+

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
`harvest#129`_ Add Support for LBLX File Extension
++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                                                |I&T Status          |Level         |Priority / Bug Severity   |
+=====================================================================================================+====================+==============+==========================+
|`harvest#130`_ As a user, I want to ingest data products with labels having `.lblx` file extension   ||:yellow_circle:|   |requirement   |p.must-have               |
+-----------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------+--------------------+--------------------------+
|Issue                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================+====================+==========================+
|`harvest#134`_ `Too many requests` error to OpenSearch   ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------+--------------------+--------------------------+

--------

Mi-label
--------
*Metadata Injector for PDS Labels (MILabel) provides a command-line interface for generating PDS4 Labels using a user provided PDS4 XML template and input (source) data products.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/mi-label/>`_
     - `Github Repo <https://github.com/NASA-PDS/mi-label>`_
     - `Issue Tracking <https://github.com/NASA-PDS/mi-label/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/mi-label/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/mi-label/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/mi-label/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------+--------------------+--------------------------+
|Issue                                                      |I&T Status          |Priority / Bug Severity   |
+===========================================================+====================+==========================+
|`mi-label#46`_ Jackson-databind vulnerability identified   ||:yellow_circle:|   |s.high                    |
+-----------------------------------------------------------+--------------------+--------------------------+

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
Requirements
++++++++++++

+-------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================================+====================+==========================+
|`pds4-information-model#709`_ Add KARI as a new agency `urn:kari:kpds`   ||:yellow_circle:|   |p.must-have               |
+-------------------------------------------------------------------------+--------------------+--------------------------+

--------

Planetary-data-engine
---------------------
*Free-text search capability for planetary data, services, tools, and information*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/planetary-data-engine#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/planetary-data-engine>`_
     - `Issue Tracking <https://github.com/NASA-PDS/planetary-data-engine/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/planetary-data-engine/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/planetary-data-engine/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/planetary-data-engine/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`planetary-data-engine#5`_ Complete Sinequa Useability Analysis
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the link in
    this section title for details.

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------+------------------+--------------------------+
|Issue                                                |I&T Status        |Priority / Bug Severity   |
+=====================================================+==================+==========================+
|`registry#234`_ Missing NAIF from Legacy Dashboard   ||:blue_circle:|   |s.low                     |
+-----------------------------------------------------+------------------+--------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                       |I&T Status          |Priority / Bug Severity   |
+============================================================================+====================+==========================+
|`registry#176`_ As a user, I want the registry to have 99.9999999% uptime   ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------+--------------------+--------------------------+

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

+--------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                         |I&T Status          |Priority / Bug Severity   |
+==============================================================+====================+==========================+
|`registry-api#229`_ api is not returning consistent answer    ||:yellow_circle:|   |s.medium                  |
+--------------------------------------------------------------+--------------------+--------------------------+

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

+-------------------------------------------------+--------------------+--------------------------+
|Issue                                            |I&T Status          |Priority / Bug Severity   |
+=================================================+====================+==========================+
|`registry-common#40`_ Fix code scanning alerts   ||:yellow_circle:|   |s.high                    |
+-------------------------------------------------+--------------------+--------------------------+

--------

Registry-harvest-legacy
-----------------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-harvest-legacy#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-harvest-legacy>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-harvest-legacy/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-harvest-legacy/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-harvest-legacy/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-harvest-legacy/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                  |I&T Status          |Priority / Bug Severity   |
+=======================================================================================================+====================+==========================+
|`registry-harvest-legacy#8`_ As a user, I want to ingest Product_External products into the Registry   ||:yellow_circle:|   |p.must-have               |
+-------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Registry-mgr-legacy
-------------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-mgr-legacy#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-mgr-legacy>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-mgr-legacy/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-mgr-legacy/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-mgr-legacy/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-mgr-legacy/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+---------------------------------------------------------+--------------------+--------------------------+
|Issue                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================+====================+==========================+
|`registry-mgr-legacy#17`_ Upgrade to latest Solr 9.3.x   ||:yellow_circle:|   |unknown                   |
+---------------------------------------------------------+--------------------+--------------------------+

--------

Registry-pds3-catalog
---------------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-pds3-catalog#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-pds3-catalog>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-pds3-catalog/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-pds3-catalog/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-pds3-catalog/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-pds3-catalog/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+--------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                   |I&T Status          |Priority / Bug Severity   |
+========================================================================================================+====================+==========================+
|`registry-pds3-catalog#6`_ Upgrade to latest Solr 9.3.x                                                 ||:yellow_circle:|   |p.must-have               |
+--------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-pds3-catalog#4`_ Upgrade Catalog Tool and dependencies to support Harvest/Registry upgrades   ||:yellow_circle:|   |p.must-have               |
+--------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

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

+---------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                  |I&T Status          |Priority / Bug Severity   |
+=======================================================================================+====================+==========================+
|`roundup-action#124`_ Roundup pushes version update prior to completion of execution   ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------+--------------------+--------------------------+

--------

Search-ui-legacy
----------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/search-ui-legacy#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/search-ui-legacy>`_
     - `Issue Tracking <https://github.com/NASA-PDS/search-ui-legacy/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/search-ui-legacy/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/search-ui-legacy/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/search-ui-legacy/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                |I&T Status          |Priority / Bug Severity   |
+=====================================================================================================+====================+==========================+
|`search-ui-legacy#1`_ Upgrade Keyword Search and dependencies to support Harvest/Registry upgrades   ||:yellow_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------+--------------------+--------------------------+

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

+--------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                 |I&T Status          |Priority / Bug Severity   |
+======================================================================================+====================+==========================+
|`transform#45`_ Broken download link and Windows JAVA settings in installation docs   ||:yellow_circle:|   |s.medium                  |
+--------------------------------------------------------------------------------------+--------------------+--------------------------+
|`transform#30`_ [SECURITY] Upgrade to log4j-core/log4j-api                            ||:yellow_circle:|   |s.low                     |
+--------------------------------------------------------------------------------------+--------------------+--------------------------+
|`transform#46`_ NoClassDefFoundError exception when transforming XML to PDS3 label    ||:yellow_circle:|   |s.medium                  |
+--------------------------------------------------------------------------------------+--------------------+--------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                     |I&T Status          |Priority / Bug Severity   |
+==========================================================================================================================================+====================+==========================+
|`validate#754`_ Validate 3.3.0 erroneously reports data objects out of offset order                                                       ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#427`_ validate does not work correct when path name contains a space on mac                                                     ||:yellow_circle:|   |s.low                     |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#748`_ Buffer limit IOException thrown with validate-refs                                                                        ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#763`_ Validate.bat does not execute on Windows                                                                                  ||:yellow_circle:|   |s.critical                |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#739`_ Intermittent network failures attempting repeated downloads of schemas/schematrons                                        ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#475`_ Validate crashes on invalid # of records, and spurious file left behind                                                   ||:yellow_circle:|   |p.wont-have               |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#432`_ Requirement #308 does not appear to be working for checking referential integrity from products to others in the bundle   ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#723`_ Installation instructions need updates for Windows                                                                        ||:yellow_circle:|   |unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#760`_ Uncaught exception thrown when only 1 of schemas/schematrons are provided via command-line                                ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#761`_ Validate gives errors for 'NaN' values in IEEE754 data                                                                    ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#747`_ validate flags IEEE 754 "infinity" values as invalid                                                                      ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#698`_ Investigate and Fix code scanning alert for potential improvements                                                        ||:blue_circle:|     |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#750`_ Validate-refs with manifest of file paths does not seem to read the files correctly                                       ||:yellow_circle:|   |s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#681`_ Validate incorrectly throws precision mismatch error for Table_Delimited                                                  ||:yellow_circle:|   |s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                                      |I&T Status          |Priority / Bug Severity   |
+===========================================================================================================================================================+====================+==========================+
|`validate#308`_ As a user, I want to check that all Internal References are valid references to other PDS4 products within the current validating bundle   ||:yellow_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#741`_ As a user, I want validate's referential integrity tool to read a manifest of files and check referential integrity                        ||:yellow_circle:|   |p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Liens
=====

+--------+--------+------------+
|Issue   |Title   |Rationale   |
+========+========+============+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B14.1)`_

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

.. _plan B14.1: https://nasa-pds.github.io/releases/14.1/plan.html
.. _deep-archive#151: https://github.com/NASA-PDS/deep-archive/issues/151
.. _doi-ui#215: https://github.com/NASA-PDS/doi-ui/issues/215
.. _ds-view#14: https://github.com/NASA-PDS/ds-view/issues/14
.. _ds-view#12: https://github.com/NASA-PDS/ds-view/issues/12
.. _ds-view#3: https://github.com/NASA-PDS/ds-view/issues/3
.. _ds-view#8: https://github.com/NASA-PDS/ds-view/issues/8
.. _harvest#129: https://github.com/NASA-PDS/harvest/issues/129
.. _harvest#130: https://github.com/NASA-PDS/harvest/issues/130
.. _harvest#134: https://github.com/NASA-PDS/harvest/issues/134
.. _mi-label#46: https://github.com/NASA-PDS/mi-label/issues/46
.. _pds4-information-model#709: https://github.com/NASA-PDS/pds4-information-model/issues/709
.. _planetary-data-engine#5: https://github.com/NASA-PDS/planetary-data-engine/issues/5
.. _registry#234: https://github.com/NASA-PDS/registry/issues/234
.. _registry#176: https://github.com/NASA-PDS/registry/issues/176
.. _registry-api#229: https://github.com/NASA-PDS/registry-api/issues/229
.. _registry-common#40: https://github.com/NASA-PDS/registry-common/issues/40
.. _registry-harvest-legacy#8: https://github.com/NASA-PDS/registry-harvest-legacy/issues/8
.. _registry-mgr-legacy#17: https://github.com/NASA-PDS/registry-mgr-legacy/issues/17
.. _registry-pds3-catalog#6: https://github.com/NASA-PDS/registry-pds3-catalog/issues/6
.. _registry-pds3-catalog#4: https://github.com/NASA-PDS/registry-pds3-catalog/issues/4
.. _roundup-action#124: https://github.com/NASA-PDS/roundup-action/issues/124
.. _search-ui-legacy#1: https://github.com/NASA-PDS/search-ui-legacy/issues/1
.. _transform#45: https://github.com/NASA-PDS/transform/issues/45
.. _transform#30: https://github.com/NASA-PDS/transform/issues/30
.. _transform#46: https://github.com/NASA-PDS/transform/issues/46
.. _validate#754: https://github.com/NASA-PDS/validate/issues/754
.. _validate#427: https://github.com/NASA-PDS/validate/issues/427
.. _validate#748: https://github.com/NASA-PDS/validate/issues/748
.. _validate#763: https://github.com/NASA-PDS/validate/issues/763
.. _validate#739: https://github.com/NASA-PDS/validate/issues/739
.. _validate#475: https://github.com/NASA-PDS/validate/issues/475
.. _validate#432: https://github.com/NASA-PDS/validate/issues/432
.. _validate#723: https://github.com/NASA-PDS/validate/issues/723
.. _validate#760: https://github.com/NASA-PDS/validate/issues/760
.. _validate#761: https://github.com/NASA-PDS/validate/issues/761
.. _validate#747: https://github.com/NASA-PDS/validate/issues/747
.. _validate#698: https://github.com/NASA-PDS/validate/issues/698
.. _validate#750: https://github.com/NASA-PDS/validate/issues/750
.. _validate#681: https://github.com/NASA-PDS/validate/issues/681
.. _validate#308: https://github.com/NASA-PDS/validate/issues/308
.. _validate#741: https://github.com/NASA-PDS/validate/issues/741
.. _Software Release Summary (B14.1): https://nasa-pds.github.io/releases/14.1/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
