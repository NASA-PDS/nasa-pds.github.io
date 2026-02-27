========================================
Release Description Document (Build B17)
========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B17`_

The following sections can be found in this document:

.. toctree::
   :glob:
   :maxdepth: 3

   rdd.rst


PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Board
and implemented by the PDS within the latest build period.

+-------------------------------+-------------------------------------------------------------+
| Ref                           | Title                                                       |
+===============================+=============================================================+
| `pds4-information-model#663`_ | Adopt Provenance LDD for Superseded LIDs - CCB-21 (CCB-367) |
+-------------------------------+-------------------------------------------------------------+

Software Changes
================
For each software repository, the changes are listed in 2 categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B17`_).

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
`data-upload-manager#264`_ Sync DUM Metadata with rclone metadata
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================+=================+===========================+
| `data-upload-manager#264`_ Sync DUM Metadata with rclone metadata | |:blue_circle:| | p.could-have              |
+-------------------------------------------------------------------+-----------------+---------------------------+


`data-upload-manager#293`_ B17 DUM Enhancements: High Priority Updates / Bug Fixes / Tasks
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                      | I&T Status      | Priority / Bug Severity   |
+============================================================================================+=================+===========================+
| `data-upload-manager#293`_ B17 DUM Enhancements: High Priority Updates / Bug Fixes / Tasks | |:blue_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------+-----------------+---------------------------+


`data-upload-manager#295`_ Add DUM Support For Handling Files In Archive Buckets
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                         | I&T Status        | Level       | Priority / Bug Severity   |
+===============================================================================================================+===================+=============+===========================+
| `data-upload-manager#100`_ As a user, I want to force an upload of file that is already in the archive bucket | |:yellow_circle:| | requirement | p.must-have               |
+---------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `data-upload-manager#99`_ As a user, I want to skip upload of files that are already in the archive bucket    | |:green_circle:|  | requirement | p.must-have               |
+---------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`data-upload-manager#319`_ New Flag to Skipping Symlinks
++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                           | I&T Status        | Level       | Priority / Bug Severity   |
+=================================================================================================+===================+=============+===========================+
| `data-upload-manager#340`_ As a data provider, I want to skip following symlinks during ingress | |:yellow_circle:| | requirement | p.should-have             |
+-------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`data-upload-manager#329`_ B17 DUM Support:  High Priority Enhancements / Bug Fixes / Tasks
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                                                                              | I&T Status        | Level   | Priority / Bug Severity   |
+====================================================================================================================+===================+=========+===========================+
| `data-upload-manager#318`_ S3 client initialization does not use explicit IAM role credentials                     | |:yellow_circle:| | bug     | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| `data-upload-manager#321`_ S3 operations do not validate bucket ownership leading to Confused Deputy vulnerability | |:yellow_circle:| | bug     | s.high                    |
+--------------------------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| `data-upload-manager#337`_ DUM client MD5 hash generation does not work on FIPS-enabled systems                    | |:yellow_circle:| | bug     | s.high                    |
+--------------------------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| `data-upload-manager#336`_ Upload of gzip files does not happen if it is batched with non-gzip files               | |:yellow_circle:| | bug     | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                         | I&T Status        | Priority / Bug Severity   |
+===============================================================================================================+===================+===========================+
| `data-upload-manager#304`_ Summary table bytes transferred does not calculate correctly with multiple threads | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                    | I&T Status       | Priority / Bug Severity   |
+==========================================================================================================+==================+===========================+
| `data-upload-manager#330`_ As a Node Operator, I want weblogs to be validated as gzipped prior to upload | |:green_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+

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

+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================================+===================+===========================+
| `deep-archive#226`_ MD5 hashing does not work in FIPS mode                                            | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `deep-archive#237`_ Registry transient error not handled gracefully – JSONDecodeError on 500 response | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================+===================+===========================+
| `deep-archive#238`_ Optimize API payload size by requesting only required fields | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------+-------------------+---------------------------+

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

+----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                | I&T Status        | Priority / Bug Severity   |
+======================================================================================================================+===================+===========================+
| `doi-service#510`_ DOI Search is not returning all SBN collections from DataCite for 10.26007                        | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `doi-service#502`_ SFTP roundup script does not run due to missing invoke dependencies on Python 3.13                | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `doi-service#513`_ Tests fail with ModuleNotFoundError for pkg_resources after setuptools 81 release                 | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `doi-service#497`_ FIPS Compliance: MD5 usage in checksum() function still causes ValueError on FIPS-enabled systems | |:blue_circle:|   | s.high                    |
+----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `doi-service#500`_ pds-doi-cmd release fails when there are multiple `List_Author` classes in a label                | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+----------------------------------------------------------+-----------------+---------------------------+
| Issue                                                    | I&T Status      | Priority / Bug Severity   |
+==========================================================+=================+===========================+
| `doi-service#493`_ Remove or ignore use of MD5 from code | |:blue_circle:| | unknown                   |
+----------------------------------------------------------+-----------------+---------------------------+

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

+-----------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                               | I&T Status        | Priority / Bug Severity   |
+=====================================================================================================+===================+===========================+
| `ds-view#60`_ JSP view pages are vulnerable to HTML/link injection via unsanitized parameter output | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Harvest
-------
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
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                  | I&T Status        | Priority / Bug Severity   |
+========================================================================================================================+===================+===========================+
| `harvest#285`_ False positive Duplicate detected by harvest                                                            | |:blue_circle:|   | s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#283`_ Harvest cannot parse Date without time                                                                  | |:green_circle:|  | s.high                    |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#144`_ Harvest setting pds:Time_Coordinates.pds:stop_date_time to bogus value when value is missing from label | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `harvest#279`_ GEO no longer able to harvest data due to cognito issue                                                 | |:yellow_circle:| | s.critical                |
+------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Lasso-issues
------------
*Utilities for wrapping GitHub API for creating specific data structures and reports from GitHub issues*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/lasso-issues#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/lasso-issues>`_
     - `Issue Tracking <https://github.com/NASA-PDS/lasso-issues/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/lasso-issues/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/lasso-issues/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/lasso-issues/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================================================+===================+===========================+
| `lasso-issues#51`_ RDD and markdown reports do not respect ignore flag in products config | |:yellow_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================================================+===================+===========================+
| `lasso-issues#41`_ As a user, I want to automate creation of release theme issues from CSV schedules                            | |:blue_circle:|   | p.could-have              |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `lasso-issues#47`_ As a PDS project manager, I want enhanced issue reporting with component grouping and parent-child hierarchy | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                      | I&T Status      | Priority / Bug Severity   |
+============================================================+=================+===========================+
| `lasso-issues#48`_ Remove ZenHub integration from codebase | |:blue_circle:| | unknown                   |
+------------------------------------------------------------+-----------------+---------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                          | I&T Status        | Priority / Bug Severity   |
+================================================================+===================+===========================+
| `operations#900`_ nssdca-delivery missing from issue templates | |:yellow_circle:| | s.low                     |
+----------------------------------------------------------------+-------------------+---------------------------+

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

+-----------------------------------------------+-------------------+---------------------------+
| Issue                                         | I&T Status        | Priority / Bug Severity   |
+===============================================+===================+===========================+
| `pds-api#296`_ Link to PDF document is broken | |:yellow_circle:| | s.low                     |
+-----------------------------------------------+-------------------+---------------------------+

--------

Pds4-context-products
---------------------
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
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================================+===================+===========================+
| `pds4-context-products#70`_ Invalid XML structure in two context products causes incorrect page types in search | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`pds4-information-model#926`_ Refactor PDS4 Data Dictionary Search to Support Scalability
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`pds4-information-model#965`_ Develop New Product Resource Data Model for Services and Tools
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`pds4-information-model#981`_ B17 SCR Freeze
++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                                                      | I&T Status        | Level   | Priority / Bug Severity   |
+============================================================================================+===================+=========+===========================+
| `pds4-information-model#982`_ The `contributor_type` `DataCurator` has a typo / misdefined | |:yellow_circle:| | bug     | s.medium                  |
+--------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+


`pds4-information-model#983`_ B17 Standards Documents Updates
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`pds4-information-model#984`_ B17 Information Model Delivery to I&T
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`pds4-information-model#985`_ B17 Information Model SCR Implementation and LDDTool Updates
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                                     | I&T Status      | Level       | Priority / Bug Severity   |
+===========================================================================================+=================+=============+===========================+
| `pds4-information-model#663`_ Adopt Provenance LDD for Superseded LIDs - CCB-21 (CCB-367) | |:blue_circle:| | requirement | p.must-have               |
+-------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| `pds4-information-model#990`_ Complete documentation for PROV LDD                         | |:blue_circle:| | enhancement | unknown                   |
+-------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| `pds4-information-model#991`_ Improve PROV LDD with controlled vocabulary                 | |:blue_circle:| | enhancement | unknown                   |
+-------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                        | I&T Status      | Priority / Bug Severity   |
+==============================================================================+=================+===========================+
| `pds4-information-model#976`_ [namespace-registry] add new namespace phoenix | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Peppi
-----
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
~~~~~~~~~~~~~~~
`peppi#121`_ Integrate PDS Registry MCP Server Info with PEPPI
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                          | I&T Status      | Priority / Bug Severity   |
+================================================================+=================+===========================+
| `peppi#121`_ Integrate PDS Registry MCP Server Info with PEPPI | |:blue_circle:| | unknown                   |
+----------------------------------------------------------------+-----------------+---------------------------+


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
`planetary-data-cloud#117`_ Implement Optional Cognito Password Rotation Requirement (Disabled)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#144`_ Develop Egress Management Strategy
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                          | I&T Status      | Priority / Bug Severity   |
+================================================================+=================+===========================+
| `planetary-data-cloud#144`_ Develop Egress Management Strategy | |:blue_circle:| | p.must-have               |
+----------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#147`_ B16 Bi-annual Cloud Resource Housekeeping
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================+=================+===========================+
| `planetary-data-cloud#147`_ B16 Bi-annual Cloud Resource Housekeeping | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#157`_ Egress Management Strategy Phase 1 - Throttling and Monitoring
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#178`_ Plan, Schedule, and Implement First PDC CoP
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================================+=================+===========================+
| `planetary-data-cloud#178`_ Plan, Schedule, and Implement First PDC CoP | |:blue_circle:| | unknown                   |
+-------------------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#183`_ Develop Monthly Cloud Reporting Metrics Spreadsheet and Documentation
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#193`_ B17 Bi-annual Cloud Resource Housekeeping
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#194`_ Complete Migration of ATM Backup
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#195`_ PDC Role Definitions: Tenant EN Platform and Data Engineer Roles
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#199`_ Consolidate DUM and Registry Configurations
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================================+=================+===========================+
| `planetary-data-cloud#199`_ Consolidate DUM and Registry Configurations | |:blue_circle:| | unknown                   |
+-------------------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#202`_ Require and Implement Tagging Across All Component Terraforms
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#205`_ Support PDC Migration to SCIP
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#206`_ Develop Risk List
+++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#207`_ Data Storage Management Strategy Phase 1 - Tool Trade, Dashboards, Thresholds, Alerts
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

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
`registry#266`_ Implement design for alternate data file paths / file path updates
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry#333`_ Add S3 URIs to Registry Metadata
++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry#432`_ Onboard IPDA Partner: ISRO
++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry#436`_ B17 Registry Support: High Priority Enhancements / Bug Fixes / Tasks
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------+-----------------+---------+---------------------------+
| Issue                                                                     | I&T Status      | Level   | Priority / Bug Severity   |
+===========================================================================+=================+=========+===========================+
| `registry#466`_ Can no longer load data into en-registry from staging EC2 | |:blue_circle:| | bug     | s.critical                |
+---------------------------------------------------------------------------+-----------------+---------+---------------------------+


`registry#451`_ Trade Study and Cost Analysis of AOSS vs. Managed OpenSearch vs. Self-managed Cluster
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------+-------------------+---------------------------+
| Issue                                                | I&T Status        | Priority / Bug Severity   |
+======================================================+===================+===========================+
| `registry#456`_ Some properties return "null" values | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                     | I&T Status      | Priority / Bug Severity   |
+===========================================================================+=================+===========================+
| `registry#460`_ Document and script the monthly legacy registry statusing | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------------+-----------------+---------------------------+

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
`registry-api#715`_ Complete Design for Supporting Registration and Search of Mirrored Archives
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#622`_ Add Search Functionality to Find When Class / Attribute Has Been Used / Exists
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                             | I&T Status        | Level       | Priority / Bug Severity   |
+===================================================================================================================+===================+=============+===========================+
| `registry-api#406`_ As a user, I want to query for documents where a specific search field exists in the document | |:yellow_circle:| | requirement | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`registry-api#632`_ Add Support for Searching Full PDS4 Structured Metadata
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                       | I&T Status        | Level       | Priority / Bug Severity   |
+=============================================================================================================+===================+=============+===========================+
| `registry-api#611`_ As a user, I want to search by a full/unique hierarchical path for a specific attribute | |:yellow_circle:| | requirement | p.must-have               |
+-------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`registry-api#689`_ Develop OPS LDD
+++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#698`_ Refactor Registry API Functionality for `/products/{identifier}/members/members`
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                                                                                              | I&T Status      | Level       | Priority / Bug Severity   |
+====================================================================================================================================================+=================+=============+===========================+
| `registry-api#699`_ Update registry API `/members/members` algorithm per deprecation of `parent_bundle_identifier` metadata non-aggregate products | |:blue_circle:| | enhancement | unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


`registry-api#706`_ B17 Search API Support: High Priority Enhancements / Bug Fixes / Tasks
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                      | I&T Status      | Priority / Bug Severity   |
+============================================================================================+=================+===========================+
| `registry-api#706`_ B17 Search API Support: High Priority Enhancements / Bug Fixes / Tasks | |:blue_circle:| | p.could-have              |
+--------------------------------------------------------------------------------------------+-----------------+---------------------------+


`registry-api#709`_ Enable Metrics, Logging, and Monitoring for Registry API
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-api#721`_ B17 Registry API Support: High Priority Enhancements / Bug Fixes / Tasks
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                                                             | I&T Status        | Level   | Priority / Bug Severity   |
+===================================================================================================+===================+=========+===========================+
| `registry-api#705`_ Inconsistent support for `application/vnd.nasa.pds.pds4+json` response format | |:green_circle:|  | bug     | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| `registry-api#716`_ API in production is unstable and returns 500 errors                          | |:yellow_circle:| | bug     | s.critical                |
+---------------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+


`registry-api#729`_ Update Functionality To Find When Class / Attribute Has Been Used / Exists
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

--------

Registry-legacy-solr
--------------------
*Legacy Registry Software components leveraging Apache Solr. Includes Legacy Harvest Tool, Registry Manager, PDS3 Catalog Tool, and Search Core library. These components provide the capabilities for loading PDS3 and PDS4 data into the Legacy Solr Registry, driving the PDS keyword search.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-legacy-solr#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-legacy-solr>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-legacy-solr/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-legacy-solr/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-legacy-solr/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-legacy-solr/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`registry-legacy-solr#162`_ Load IPDA Partner Agency Bundles, Collections, and Context Products into Legacy Registry
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-legacy-solr#241`_ B17 Registry Legacy Support: High Priority Enhancements / Bug Fixes / Tasks
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                                                         | I&T Status        | Level   | Priority / Bug Severity   |
+===============================================================================================+===================+=========+===========================+
| `registry-legacy-solr#243`_ Unexpected `Internal Reference` And `Reference` Page Types Values | |:yellow_circle:| | bug     | s.medium                  |
+-----------------------------------------------------------------------------------------------+-------------------+---------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================================+===================+===========================+
| `registry-legacy-solr#237`_ harvest-solr XML flattening does not preserve relationships between nested elements | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`registry-loader#11`_ Combine registry-common/harvest/registry-mgr into one registry-loader repo
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                            | I&T Status      | Priority / Bug Severity   |
+==================================================================================================+=================+===========================+
| `registry-loader#11`_ Combine registry-common/harvest/registry-mgr into one registry-loader repo | |:blue_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------+-----------------+---------------------------+


`registry-loader#49`_ Develop Harvest and Registry Manager Test Framework
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------+-------------------+---------------------------+
| Issue                                       | I&T Status        | Priority / Bug Severity   |
+=============================================+===================+===========================+
| `registry-loader#44`_ Remove error from log | |:yellow_circle:| | s.medium                  |
+---------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                      | I&T Status        | Priority / Bug Severity   |
+============================================================================================================+===================+===========================+
| `registry-loader#42`_ As a Harvest user, I want both the file path and the lidvid included in log messages | |:yellow_circle:| | p.should-have             |
+------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================================+=================+===========================+
| `registry-loader#41`_ Merge registry-common, registry-mgr, harvest into one uber repo | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`registry-sweepers#186`_ Optimize Sweepers Performance - Part 2
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                                       | I&T Status      | Level       | Priority / Bug Severity   |
+=============================================================================================+=================+=============+===========================+
| `registry-sweepers#187`_ Update ancestry handling for handling members of collection LIDVID | |:blue_circle:| | enhancement | unknown                   |
+---------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


`registry-sweepers#189`_ Update sweepers to support new structured metadata
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry-sweepers#201`_ Implement Handling of Partial Collections Uploads and Orphan Products
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================================+===================+===========================+
| `registry-sweepers#192`_ Docker container does not run with non-root user | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                         | I&T Status      | Priority / Bug Severity   |
+===============================================================================================+=================+===========================+
| `registry-sweepers#185`_ Remove `parent_bundle_identifier` support for non-aggregate products | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`software-issues-repo#119`_ 2026 Annual Contingency Plan Review and Test
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                    | I&T Status      | Priority / Bug Severity   |
+==========================================================================+=================+===========================+
| `software-issues-repo#119`_ 2026 Annual Contingency Plan Review and Test | |:blue_circle:| | unknown                   |
+--------------------------------------------------------------------------+-----------------+---------------------------+


`software-issues-repo#120`_ B16 Security Code Scans
+++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------+-----------------+---------------------------+
| Issue                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================+=================+===========================+
| `software-issues-repo#120`_ B16 Security Code Scans | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------+-----------------+---------------------------+


`software-issues-repo#121`_ B16 Prep for I&T
++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------+-----------------+---------------------------+
| Issue                                        | I&T Status      | Priority / Bug Severity   |
+==============================================+=================+===========================+
| `software-issues-repo#121`_ B16 Prep for I&T | |:blue_circle:| | unknown                   |
+----------------------------------------------+-----------------+---------------------------+


`software-issues-repo#142`_ B17 Security Code Scans
+++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`software-issues-repo#143`_ B17 Prep for I&T
++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`software-issues-repo#155`_ B17 Release Planning
++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------+-----------------+---------------------------+
| Issue                                            | I&T Status      | Priority / Bug Severity   |
+==================================================+=================+===========================+
| `software-issues-repo#155`_ B17 Release Planning | |:blue_circle:| | unknown                   |
+--------------------------------------------------+-----------------+---------------------------+


`software-issues-repo#156`_ B17 Triage Security Code Scans
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`software-issues-repo#157`_ Close our PDS Security Plan
+++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================================================================================+=================+===========================+
| `software-issues-repo#140`_ Add automation with GitHub Actions for integrating label selections and GitHub Projects | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

--------

System-i-n-t
------------
*Repo for PDS EN System I&T scripts and issue tracking*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/system-i-n-t#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/system-i-n-t>`_
     - `Issue Tracking <https://github.com/NASA-PDS/system-i-n-t/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/system-i-n-t/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/system-i-n-t/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/system-i-n-t/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`system-i-n-t#68`_ B16 Standards Document Review
++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------+-----------------+---------------------------+
| Issue                                            | I&T Status      | Priority / Bug Severity   |
+==================================================+=================+===========================+
| `system-i-n-t#68`_ B16 Standards Document Review | |:blue_circle:| | unknown                   |
+--------------------------------------------------+-----------------+---------------------------+


`system-i-n-t#70`_ B16 System Integration & Test
++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------+-----------------+---------------------------+
| Issue                                            | I&T Status      | Priority / Bug Severity   |
+==================================================+=================+===========================+
| `system-i-n-t#70`_ B16 System Integration & Test | |:blue_circle:| | unknown                   |
+--------------------------------------------------+-----------------+---------------------------+


`system-i-n-t#71`_ B16 Deployment and Release
+++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------+-----------------+---------------------------+
| Issue                                         | I&T Status      | Priority / Bug Severity   |
+===============================================+=================+===========================+
| `system-i-n-t#71`_ B16 Deployment and Release | |:blue_circle:| | unknown                   |
+-----------------------------------------------+-----------------+---------------------------+


`system-i-n-t#72`_ B16 Delivery & Deployment Review (DDR)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------+-----------------+---------------------------+
| Issue                                                     | I&T Status      | Priority / Bug Severity   |
+===========================================================+=================+===========================+
| `system-i-n-t#72`_ B16 Delivery & Deployment Review (DDR) | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------+-----------------+---------------------------+


`system-i-n-t#76`_ B17 dLDD Integration & Test
++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`system-i-n-t#77`_ B17 Standards Document Review
++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`system-i-n-t#78`_ B17 System Integration & Test 
+++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`system-i-n-t#79`_ B17 Information Model I&T
++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`system-i-n-t#80`_ B17 Delivery & Deployment Review (DDR)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`system-i-n-t#81`_ B17 Deployment and Release
+++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

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
`validate#1473`_ B17 Validate Support: High Priority Enhancements / Bug Fixes / Tasks
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------+---------------------------+
| Issue                                                                                                                                          | I&T Status       | Level   | Priority / Bug Severity   |
+================================================================================================================================================+==================+=========+===========================+
| `validate#1316`_ Encoded_Audio encoding_standard_id = WAV gives MP4 error in Validate 3.7.1                                                    | |:green_circle:| | bug     | s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------+---------------------------+
| `validate#1241`_ Validating large data file (150GB) is trying to write the entire file to local temp space - error upon not enough local space | |:blue_circle:|  | bug     | s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------+---------------------------+
| `validate#1408`_ JSON reports duplicates messages per product specified                                                                        | |:blue_circle:|  | bug     | s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================================================================+===================+===========================+
| `validate#1453`_ new/updated context objects have not been incorporated into the validator for 2 months   | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1423`_ Running validate 4.0.4 on terminal produces lots of new line characters while processing | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1294`_ validate does not handle Special Constants for UnsignedMSB4                              | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Web-analytics
-------------
*None*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/web-analytics>`_
     - `Github Repo <https://github.com/NASA-PDS/web-analytics>`_
     - `Issue Tracking <https://github.com/NASA-PDS/web-analytics/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/web-analytics/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/web-analytics/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/web-analytics/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`web-analytics#63`_ Onboard Nodes to Upload Web Logs With DUM
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                               | I&T Status        | Priority / Bug Severity   |
+=====================================================================+===================+===========================+
| `web-analytics#66`_ Terraform mistakenly expires logs after 30 days | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------+-------------------+---------------------------+

Release Summary Metrics
=======================
This section provides a summary of the issues addressed in this release, organized by issue type.


+------------------------+--------+----------------+----------------+---------+----------+---------+
| Component/Repo         | Bugs   | Enhancements   | Requirements   | Tasks   | Themes   | Total   |
+========================+========+================+================+=========+==========+=========+
| data-upload-manager    | 5      | 0              | 4              | 0       | 5        | 14      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| deep-archive           | 2      | 1              | 0              | 0       | 0        | 3       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| doi-service            | 5      | 1              | 0              | 0       | 0        | 6       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| ds-view                | 1      | 0              | 0              | 0       | 0        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| harvest                | 4      | 0              | 0              | 0       | 0        | 4       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| lasso-issues           | 1      | 1              | 2              | 0       | 0        | 4       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| operations             | 1      | 0              | 0              | 0       | 0        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| pds-api                | 1      | 0              | 0              | 0       | 0        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| pds4-context-products  | 1      | 0              | 0              | 0       | 0        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| pds4-information-model | 1      | 3              | 1              | 0       | 6        | 11      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| peppi                  | 0      | 0              | 0              | 0       | 1        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| planetary-data-cloud   | 0      | 0              | 0              | 0       | 14       | 14      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry               | 2      | 1              | 0              | 0       | 5        | 8       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-api           | 2      | 1              | 2              | 0       | 9        | 14      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-legacy-solr   | 2      | 0              | 0              | 0       | 2        | 4       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-loader        | 1      | 1              | 1              | 0       | 2        | 5       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-sweepers      | 1      | 2              | 0              | 0       | 3        | 6       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| software-issues-repo   | 0      | 1              | 0              | 0       | 8        | 9       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| system-i-n-t           | 0      | 0              | 0              | 0       | 10       | 10      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| validate               | 6      | 0              | 0              | 0       | 1        | 7       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| web-analytics          | 1      | 0              | 0              | 0       | 1        | 2       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| **TOTAL**              | **37** | **12**         | **10**         | **0**   | **67**   | **126** |
+------------------------+--------+----------------+----------------+---------+----------+---------+


Liens
=====

+---------+---------+-------------+
| Issue   | Title   | Rationale   |
+=========+=========+=============+
+---------+---------+-------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B17)`_

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

.. _plan B17: https://nasa-pds.github.io/releases/17/plan.html
.. _pds4-information-model#663: https://github.com/NASA-PDS/pds4-information-model/issues/663
.. _data-upload-manager#264: https://github.com/NASA-PDS/data-upload-manager/issues/264
.. _data-upload-manager#293: https://github.com/NASA-PDS/data-upload-manager/issues/293
.. _data-upload-manager#295: https://github.com/NASA-PDS/data-upload-manager/issues/295
.. _data-upload-manager#100: https://github.com/NASA-PDS/data-upload-manager/issues/100
.. _data-upload-manager#99: https://github.com/NASA-PDS/data-upload-manager/issues/99
.. _data-upload-manager#319: https://github.com/NASA-PDS/data-upload-manager/issues/319
.. _data-upload-manager#340: https://github.com/NASA-PDS/data-upload-manager/issues/340
.. _data-upload-manager#329: https://github.com/NASA-PDS/data-upload-manager/issues/329
.. _data-upload-manager#318: https://github.com/NASA-PDS/data-upload-manager/issues/318
.. _data-upload-manager#321: https://github.com/NASA-PDS/data-upload-manager/issues/321
.. _data-upload-manager#337: https://github.com/NASA-PDS/data-upload-manager/issues/337
.. _data-upload-manager#336: https://github.com/NASA-PDS/data-upload-manager/issues/336
.. _data-upload-manager#304: https://github.com/NASA-PDS/data-upload-manager/issues/304
.. _data-upload-manager#330: https://github.com/NASA-PDS/data-upload-manager/issues/330
.. _deep-archive#226: https://github.com/NASA-PDS/deep-archive/issues/226
.. _deep-archive#237: https://github.com/NASA-PDS/deep-archive/issues/237
.. _deep-archive#238: https://github.com/NASA-PDS/deep-archive/issues/238
.. _doi-service#510: https://github.com/NASA-PDS/doi-service/issues/510
.. _doi-service#502: https://github.com/NASA-PDS/doi-service/issues/502
.. _doi-service#513: https://github.com/NASA-PDS/doi-service/issues/513
.. _doi-service#497: https://github.com/NASA-PDS/doi-service/issues/497
.. _doi-service#500: https://github.com/NASA-PDS/doi-service/issues/500
.. _doi-service#493: https://github.com/NASA-PDS/doi-service/issues/493
.. _ds-view#60: https://github.com/NASA-PDS/ds-view/issues/60
.. _harvest#285: https://github.com/NASA-PDS/harvest/issues/285
.. _harvest#283: https://github.com/NASA-PDS/harvest/issues/283
.. _harvest#144: https://github.com/NASA-PDS/harvest/issues/144
.. _harvest#279: https://github.com/NASA-PDS/harvest/issues/279
.. _lasso-issues#51: https://github.com/NASA-PDS/lasso-issues/issues/51
.. _lasso-issues#41: https://github.com/NASA-PDS/lasso-issues/issues/41
.. _lasso-issues#47: https://github.com/NASA-PDS/lasso-issues/issues/47
.. _lasso-issues#48: https://github.com/NASA-PDS/lasso-issues/issues/48
.. _operations#900: https://github.com/NASA-PDS/operations/issues/900
.. _pds-api#296: https://github.com/NASA-PDS/pds-api/issues/296
.. _pds4-context-products#70: https://github.com/NASA-PDS/pds4-context-products/issues/70
.. _pds4-information-model#926: https://github.com/NASA-PDS/pds4-information-model/issues/926
.. _pds4-information-model#965: https://github.com/NASA-PDS/pds4-information-model/issues/965
.. _pds4-information-model#981: https://github.com/NASA-PDS/pds4-information-model/issues/981
.. _pds4-information-model#982: https://github.com/NASA-PDS/pds4-information-model/issues/982
.. _pds4-information-model#983: https://github.com/NASA-PDS/pds4-information-model/issues/983
.. _pds4-information-model#984: https://github.com/NASA-PDS/pds4-information-model/issues/984
.. _pds4-information-model#985: https://github.com/NASA-PDS/pds4-information-model/issues/985
.. _pds4-information-model#663: https://github.com/NASA-PDS/pds4-information-model/issues/663
.. _pds4-information-model#990: https://github.com/NASA-PDS/pds4-information-model/issues/990
.. _pds4-information-model#991: https://github.com/NASA-PDS/pds4-information-model/issues/991
.. _pds4-information-model#976: https://github.com/NASA-PDS/pds4-information-model/issues/976
.. _peppi#121: https://github.com/NASA-PDS/peppi/issues/121
.. _planetary-data-cloud#117: https://github.com/NASA-PDS/planetary-data-cloud/issues/117
.. _planetary-data-cloud#144: https://github.com/NASA-PDS/planetary-data-cloud/issues/144
.. _planetary-data-cloud#147: https://github.com/NASA-PDS/planetary-data-cloud/issues/147
.. _planetary-data-cloud#157: https://github.com/NASA-PDS/planetary-data-cloud/issues/157
.. _planetary-data-cloud#178: https://github.com/NASA-PDS/planetary-data-cloud/issues/178
.. _planetary-data-cloud#183: https://github.com/NASA-PDS/planetary-data-cloud/issues/183
.. _planetary-data-cloud#193: https://github.com/NASA-PDS/planetary-data-cloud/issues/193
.. _planetary-data-cloud#194: https://github.com/NASA-PDS/planetary-data-cloud/issues/194
.. _planetary-data-cloud#195: https://github.com/NASA-PDS/planetary-data-cloud/issues/195
.. _planetary-data-cloud#199: https://github.com/NASA-PDS/planetary-data-cloud/issues/199
.. _planetary-data-cloud#202: https://github.com/NASA-PDS/planetary-data-cloud/issues/202
.. _planetary-data-cloud#205: https://github.com/NASA-PDS/planetary-data-cloud/issues/205
.. _planetary-data-cloud#206: https://github.com/NASA-PDS/planetary-data-cloud/issues/206
.. _planetary-data-cloud#207: https://github.com/NASA-PDS/planetary-data-cloud/issues/207
.. _registry#266: https://github.com/NASA-PDS/registry/issues/266
.. _registry#333: https://github.com/NASA-PDS/registry/issues/333
.. _registry#432: https://github.com/NASA-PDS/registry/issues/432
.. _registry#436: https://github.com/NASA-PDS/registry/issues/436
.. _registry#466: https://github.com/NASA-PDS/registry/issues/466
.. _registry#451: https://github.com/NASA-PDS/registry/issues/451
.. _registry#456: https://github.com/NASA-PDS/registry/issues/456
.. _registry#460: https://github.com/NASA-PDS/registry/issues/460
.. _registry-api#715: https://github.com/NASA-PDS/registry-api/issues/715
.. _registry-api#622: https://github.com/NASA-PDS/registry-api/issues/622
.. _registry-api#406: https://github.com/NASA-PDS/registry-api/issues/406
.. _registry-api#632: https://github.com/NASA-PDS/registry-api/issues/632
.. _registry-api#611: https://github.com/NASA-PDS/registry-api/issues/611
.. _registry-api#689: https://github.com/NASA-PDS/registry-api/issues/689
.. _registry-api#698: https://github.com/NASA-PDS/registry-api/issues/698
.. _registry-api#699: https://github.com/NASA-PDS/registry-api/issues/699
.. _registry-api#706: https://github.com/NASA-PDS/registry-api/issues/706
.. _registry-api#709: https://github.com/NASA-PDS/registry-api/issues/709
.. _registry-api#721: https://github.com/NASA-PDS/registry-api/issues/721
.. _registry-api#705: https://github.com/NASA-PDS/registry-api/issues/705
.. _registry-api#716: https://github.com/NASA-PDS/registry-api/issues/716
.. _registry-api#729: https://github.com/NASA-PDS/registry-api/issues/729
.. _registry-legacy-solr#162: https://github.com/NASA-PDS/registry-legacy-solr/issues/162
.. _registry-legacy-solr#241: https://github.com/NASA-PDS/registry-legacy-solr/issues/241
.. _registry-legacy-solr#243: https://github.com/NASA-PDS/registry-legacy-solr/issues/243
.. _registry-legacy-solr#237: https://github.com/NASA-PDS/registry-legacy-solr/issues/237
.. _registry-loader#11: https://github.com/NASA-PDS/registry-loader/issues/11
.. _registry-loader#49: https://github.com/NASA-PDS/registry-loader/issues/49
.. _registry-loader#44: https://github.com/NASA-PDS/registry-loader/issues/44
.. _registry-loader#42: https://github.com/NASA-PDS/registry-loader/issues/42
.. _registry-loader#41: https://github.com/NASA-PDS/registry-loader/issues/41
.. _registry-sweepers#186: https://github.com/NASA-PDS/registry-sweepers/issues/186
.. _registry-sweepers#187: https://github.com/NASA-PDS/registry-sweepers/issues/187
.. _registry-sweepers#189: https://github.com/NASA-PDS/registry-sweepers/issues/189
.. _registry-sweepers#201: https://github.com/NASA-PDS/registry-sweepers/issues/201
.. _registry-sweepers#192: https://github.com/NASA-PDS/registry-sweepers/issues/192
.. _registry-sweepers#185: https://github.com/NASA-PDS/registry-sweepers/issues/185
.. _software-issues-repo#119: https://github.com/NASA-PDS/software-issues-repo/issues/119
.. _software-issues-repo#120: https://github.com/NASA-PDS/software-issues-repo/issues/120
.. _software-issues-repo#121: https://github.com/NASA-PDS/software-issues-repo/issues/121
.. _software-issues-repo#142: https://github.com/NASA-PDS/software-issues-repo/issues/142
.. _software-issues-repo#143: https://github.com/NASA-PDS/software-issues-repo/issues/143
.. _software-issues-repo#155: https://github.com/NASA-PDS/software-issues-repo/issues/155
.. _software-issues-repo#156: https://github.com/NASA-PDS/software-issues-repo/issues/156
.. _software-issues-repo#157: https://github.com/NASA-PDS/software-issues-repo/issues/157
.. _software-issues-repo#140: https://github.com/NASA-PDS/software-issues-repo/issues/140
.. _system-i-n-t#68: https://github.com/NASA-PDS/system-i-n-t/issues/68
.. _system-i-n-t#70: https://github.com/NASA-PDS/system-i-n-t/issues/70
.. _system-i-n-t#71: https://github.com/NASA-PDS/system-i-n-t/issues/71
.. _system-i-n-t#72: https://github.com/NASA-PDS/system-i-n-t/issues/72
.. _system-i-n-t#76: https://github.com/NASA-PDS/system-i-n-t/issues/76
.. _system-i-n-t#77: https://github.com/NASA-PDS/system-i-n-t/issues/77
.. _system-i-n-t#78: https://github.com/NASA-PDS/system-i-n-t/issues/78
.. _system-i-n-t#79: https://github.com/NASA-PDS/system-i-n-t/issues/79
.. _system-i-n-t#80: https://github.com/NASA-PDS/system-i-n-t/issues/80
.. _system-i-n-t#81: https://github.com/NASA-PDS/system-i-n-t/issues/81
.. _validate#1473: https://github.com/NASA-PDS/validate/issues/1473
.. _validate#1316: https://github.com/NASA-PDS/validate/issues/1316
.. _validate#1241: https://github.com/NASA-PDS/validate/issues/1241
.. _validate#1408: https://github.com/NASA-PDS/validate/issues/1408
.. _validate#1453: https://github.com/NASA-PDS/validate/issues/1453
.. _validate#1423: https://github.com/NASA-PDS/validate/issues/1423
.. _validate#1294: https://github.com/NASA-PDS/validate/issues/1294
.. _web-analytics#63: https://github.com/NASA-PDS/web-analytics/issues/63
.. _web-analytics#66: https://github.com/NASA-PDS/web-analytics/issues/66
.. _Software Release Summary (B17): https://nasa-pds.github.io/releases/17/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md