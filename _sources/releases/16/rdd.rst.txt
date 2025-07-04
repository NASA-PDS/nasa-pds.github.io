========================================
Release Description Document (Build B16)
========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B16`_

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
PDS Software Working Group (see `Plan B16`_).

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

+------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                        | I&T Status        | Priority / Bug Severity   |
+==============================================================================+===================+===========================+
| `data-upload-manager#221`_ As a user, I want to support upload of files >5GB | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------------------------+-------------------+---------------------------+

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
`deep-archive#204`_ Add Support for Labels with LBLX file suffix
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                | I&T Status        | Priority / Bug Severity   |
+======================================================================================+===================+===========================+
| `deep-archive#208`_ Output manifest .tab files do not use forward slashes on Windows | |:yellow_circle:| | s.medium                  |
+--------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                               | I&T Status        | Priority / Bug Severity   |
+=====================================================================================+===================+===========================+
| `deep-archive#157`_ As a user, I want deep archive to support LBLX label extensions | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+----------------------------------------------------------+-------------------+---------------------------+
| Issue                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================+===================+===========================+
| `doi-service#456`_ Large majority of units tests failing | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------+-------------------+---------------------------+

--------

Edwg
----
*PDS Editorial Working Group Working Area*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/EdWG#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/EdWG>`_
     - `Issue Tracking <https://github.com/NASA-PDS/EdWG/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/EdWG/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/EdWG/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/EdWG/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`EdWG#86`_ Context Updates Phase 1: Facilities and Telescopes
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

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

+------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                  | I&T Status        | Priority / Bug Severity   |
+========================================================================+===================+===========================+
| `harvest#239`_ Harvest failing due to AOSS OCU limits without retrying | |:yellow_circle:| | s.high                    |
+------------------------------------------------------------------------+-------------------+---------------------------+

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
`nucleus#131`_ Update Architecture and Implement Separate EFS Per Node Baseline DAG
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`nucleus#142`_ Support Data Backlog Use Case
++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`nucleus#149`_ Upgrade Nucleus to the latest 2.x version in MWAA
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

--------

Planetary-data-cloud
--------------------
*PDS Cloud Migration documentation, issue, tracking and simple tools for assisting in the PDS hybrid cloud study and migration efforts.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/planetary-data-cloud#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/planetary-data-cloud>`_
     - `Issue Tracking <https://github.com/NASA-PDS/planetary-data-cloud/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/planetary-data-cloud/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/planetary-data-cloud/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/planetary-data-cloud/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`planetary-data-cloud#139`_ Define Tagging Strategy for Planetary Data Cloud
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                    | I&T Status      | Priority / Bug Severity   |
+==========================================================================================================+=================+===========================+
| `planetary-data-cloud#153`_ As a user, I need a lambda function to tag S3 objects based upon file suffix | |:blue_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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

+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================================+===================+===========================+
| `registry#404`_ Registry is not accepting date time with leap second, e.g. `2015-06-30T23:59:60.862Z` | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================================================================+===================+===========================+
| `registry#396`_ As a node user, I want to have multiple cognito groups and still have the main cognito node group to be effective | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                           | I&T Status      | Priority / Bug Severity   |
+=================================================================================+=================+===========================+
| `registry#360`_ Fix GEO node products which ops:Harvest_Info/ops:node_name: geo | |:blue_circle:| | p.must-have               |
+---------------------------------------------------------------------------------+-----------------+---------------------------+

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
`registry-api#623`_ Implement Registry API Performance Improvements
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                               | I&T Status        | Priority / Bug Severity   |
+=====================================================================+===================+===========================+
| `registry-api#638`_ The API fails when no Accept header is provided | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------+-------------------+---------------------------+

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

+-------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================+=================+===========================+
| `registry-sweepers#164`_ ATM Registry-Sweeper ECS task is failing | |:blue_circle:| | s.critical                |
+-------------------------------------------------------------------+-----------------+---------------------------+

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
`software-issues-repo#125`_ Complete ISA with NSSDCA
++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                    | I&T Status      | Priority / Bug Severity   |
+==========================================================================================+=================+===========================+
| `software-issues-repo#113`_ Create tool to generate SLOC reports for software deliveries | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`validate#1184`_ Update Context Metadata Quality Checks to Support Aliases
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================================+===================+===========================+
| `validate#967`_ validate configuration includes context product names that do not match the products    | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1234`_ validate does not raise a warning when a table has more records than label says it has | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1276`_ `--strict-field-checks` not working as expected                                        | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1149`_ `validate-bundle` has no default value for `--report-dir`                              | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                               | I&T Status        | Priority / Bug Severity   |
+=====================================================================================================+===================+===========================+
| `validate#970`_ As a user, I want to includes titles and aliases in context product name validation | |:yellow_circle:| | p.could-have              |
+-----------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1137`_ As a user, I want to know how much progress is being made during a validate run    | |:yellow_circle:| | p.should-have             |
+-----------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1201`_ As a user, I want validate to report empty (blank) PDS4 labels                     | |:yellow_circle:| | p.should-have             |
+-----------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`web-analytics#57`_ Complete Logstash Wrapper Tools for Prod Deployment
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================+===================+===========================+
| `web-analytics#51`_ `en-web-analytics` is locked up and unable to use | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------+-------------------+---------------------------+

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
`web-modernization#257`_ Design Instrument Package Portal Pages
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Liens
=====

+---------+---------+-------------+
| Issue   | Title   | Rationale   |
+=========+=========+=============+
+---------+---------+-------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B16)`_

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

.. _plan B16: https://nasa-pds.github.io/releases/16/plan.html
.. _data-upload-manager#221: https://github.com/NASA-PDS/data-upload-manager/issues/221
.. _deep-archive#204: https://github.com/NASA-PDS/deep-archive/issues/204
.. _deep-archive#208: https://github.com/NASA-PDS/deep-archive/issues/208
.. _deep-archive#157: https://github.com/NASA-PDS/deep-archive/issues/157
.. _doi-service#456: https://github.com/NASA-PDS/doi-service/issues/456
.. _EdWG#86: https://github.com/NASA-PDS/EdWG/issues/86
.. _harvest#239: https://github.com/NASA-PDS/harvest/issues/239
.. _nucleus#131: https://github.com/NASA-PDS/nucleus/issues/131
.. _nucleus#142: https://github.com/NASA-PDS/nucleus/issues/142
.. _nucleus#149: https://github.com/NASA-PDS/nucleus/issues/149
.. _planetary-data-cloud#139: https://github.com/NASA-PDS/planetary-data-cloud/issues/139
.. _planetary-data-cloud#153: https://github.com/NASA-PDS/planetary-data-cloud/issues/153
.. _registry#404: https://github.com/NASA-PDS/registry/issues/404
.. _registry#396: https://github.com/NASA-PDS/registry/issues/396
.. _registry#360: https://github.com/NASA-PDS/registry/issues/360
.. _registry-api#623: https://github.com/NASA-PDS/registry-api/issues/623
.. _registry-api#638: https://github.com/NASA-PDS/registry-api/issues/638
.. _registry-sweepers#164: https://github.com/NASA-PDS/registry-sweepers/issues/164
.. _software-issues-repo#125: https://github.com/NASA-PDS/software-issues-repo/issues/125
.. _software-issues-repo#113: https://github.com/NASA-PDS/software-issues-repo/issues/113
.. _validate#1184: https://github.com/NASA-PDS/validate/issues/1184
.. _validate#967: https://github.com/NASA-PDS/validate/issues/967
.. _validate#1234: https://github.com/NASA-PDS/validate/issues/1234
.. _validate#1276: https://github.com/NASA-PDS/validate/issues/1276
.. _validate#1149: https://github.com/NASA-PDS/validate/issues/1149
.. _validate#970: https://github.com/NASA-PDS/validate/issues/970
.. _validate#1137: https://github.com/NASA-PDS/validate/issues/1137
.. _validate#1201: https://github.com/NASA-PDS/validate/issues/1201
.. _web-analytics#57: https://github.com/NASA-PDS/web-analytics/issues/57
.. _web-analytics#51: https://github.com/NASA-PDS/web-analytics/issues/51
.. _web-modernization#257: https://github.com/NASA-PDS/web-modernization/issues/257
.. _Software Release Summary (B16): https://nasa-pds.github.io/releases/16/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md