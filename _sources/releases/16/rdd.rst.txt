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

+-------------------------------+------------------------------------------------------------------------------------------------------------+
| Ref                           | Title                                                                                                      |
+===============================+============================================================================================================+
| `pds4-information-model#663`_ | Adopt Provenance LDD for Superseded LIDs - CCB-21 (CCB-367)                                                |
+-------------------------------+------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#945`_ | CCB-60:  New permissible value for File_Area_Observational.Header.parsing_standard_id: "CDF 3.9 ISTP/IACG" |
+-------------------------------+------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#946`_ | CCB-59: funding_year only allows the value "9999"                                                          |
+-------------------------------+------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#949`_ | CCB-62: Transfer_Manifest class should enforce data types for its two mandatory columns                    |
+-------------------------------+------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#967`_ | CCB-28: As a user, I want validate to allow delimited tables with whitespace-only numeric fields           |
+-------------------------------+------------------------------------------------------------------------------------------------------------+

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
`data-upload-manager#207`_ Improvements to Support LRO Uploads
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| Issue                                                                                              | I&T Status       | Level       | Priority / Bug Severity   |
+====================================================================================================+==================+=============+===========================+
| `data-upload-manager#221`_ As a user, I want to support upload of files >5GB                       | |:green_circle:| | requirement | p.must-have               |
+----------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `data-upload-manager#224`_ Verify scalability of manifest file usage for archives >5 million files | |:blue_circle:|  | theme       | unknown                   |
+----------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `data-upload-manager#264`_ Sync DUM Metadata with rclone metadata                                  | |:blue_circle:|  | theme       | p.could-have              |
+----------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+


`data-upload-manager#224`_ Verify scalability of manifest file usage for archives >5 million files
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                              | I&T Status      | Priority / Bug Severity   |
+====================================================================================================+=================+===========================+
| `data-upload-manager#224`_ Verify scalability of manifest file usage for archives >5 million files | |:blue_circle:| | unknown                   |
+----------------------------------------------------------------------------------------------------+-----------------+---------------------------+


`data-upload-manager#231`_ Support Upload of Web Logs
+++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| Issue                                                                                     | I&T Status       | Level       | Priority / Bug Severity   |
+===========================================================================================+==================+=============+===========================+
| `data-upload-manager#232`_ As a user, I want to load web logs to the web analytics bucket | |:green_circle:| | requirement | p.should-have             |
+-------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+


`data-upload-manager#256`_ Update DUM to Support Integration with rclone
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                                                                              | I&T Status      | Level       | Priority / Bug Severity   |
+====================================================================================================================================+=================+=============+===========================+
| `data-upload-manager#209`_ As a user, I can read rclone-generated checksums when checking for existing files in the staging bucket | |:blue_circle:| | requirement | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


`data-upload-manager#264`_ Sync DUM Metadata with rclone metadata
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================+=================+===========================+
| `data-upload-manager#264`_ Sync DUM Metadata with rclone metadata | |:blue_circle:| | p.could-have              |
+-------------------------------------------------------------------+-----------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                          | I&T Status      | Priority / Bug Severity   |
+================================================================================================+=================+===========================+
| `data-upload-manager#282`_ During DUM load, undocumented message about "Backing off"           | |:blue_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `data-upload-manager#241`_ When DUM crashes, the report it generates falsely indicates success | |:blue_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `data-upload-manager#271`_ DUM output has typo                                                 | |:blue_circle:| | s.low                     |
+------------------------------------------------------------------------------------------------+-----------------+---------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                      | I&T Status       | Priority / Bug Severity   |
+============================================================================================================+==================+===========================+
| `data-upload-manager#99`_ As a user, I want to skip upload of files that are already in the archive bucket | |:green_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                       | I&T Status      | Priority / Bug Severity   |
+=============================================================+=================+===========================+
| `data-upload-manager#289`_ Enable Python 3.12 compatibility | |:blue_circle:| | p.must-have               |
+-------------------------------------------------------------+-----------------+---------------------------+

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

+-------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| Issue                                                                               | I&T Status       | Level       | Priority / Bug Severity   |
+=====================================================================================+==================+=============+===========================+
| `deep-archive#157`_ As a user, I want deep archive to support LBLX label extensions | |:green_circle:| | requirement | p.should-have             |
+-------------------------------------------------------------------------------------+------------------+-------------+---------------------------+


`deep-archive#210`_ B16 Deep Archive Maintenance Tasks
++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                                                    | I&T Status      | Level       | Priority / Bug Severity   |
+==========================================================================================================+=================+=============+===========================+
| `deep-archive#208`_ Output manifest .tab files do not use forward slashes on Windows                     | |:blue_circle:| | bug         | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| `deep-archive#136`_ As a user, I want to know that the software is still executing on long running jobs. | |:blue_circle:| | requirement | p.could-have              |
+----------------------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                           | I&T Status       | Priority / Bug Severity   |
+=================================================================================================================+==================+===========================+
| `deep-archive#213`_ pds-deep-registry-archive does not include all collections within a bundle in SIP/AIP files | |:green_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+------------------------------------------------------+-----------------+---------------------------+
| Issue                                                | I&T Status      | Priority / Bug Severity   |
+======================================================+=================+===========================+
| `deep-archive#218`_ Enable Python 3.12 compatibility | |:blue_circle:| | p.must-have               |
+------------------------------------------------------+-----------------+---------------------------+

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
`devops#81`_ Enable Continuous Deployment for Portal
++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------+-----------------+---------------------------+
| Issue                                                | I&T Status      | Priority / Bug Severity   |
+======================================================+=================+===========================+
| `devops#81`_ Enable Continuous Deployment for Portal | |:blue_circle:| | p.must-have               |
+------------------------------------------------------+-----------------+---------------------------+


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

+---------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================================================+=================+===========================+
| `doi-service#455`_ SBN DOIs contain unexpected metadata that is breaking our database load script | |:blue_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `doi-service#466`_ DOI service does not properly process UTF-16 in a JSON label                   | |:blue_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `doi-service#456`_ Large majority of units tests failing                                          | |:blue_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `doi-service#476`_ Tests do not run successfully on windows                                       | |:blue_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------+-----------------+---------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                                                       | I&T Status       | Priority / Bug Severity   |
+=============================================================================================================================================================+==================+===========================+
| `doi-service#478`_ As a user, I want to support labels with lblx suffix                                                                                     | |:blue_circle:|  | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `doi-service#432`_ As a user, I want to submit a label utilizing the updated author/contributor metadata (`List_Author`, `List_Contributor`, `List_Editor`) | |:green_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------+-----------------+---------------------------+
| Issue                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================+=================+===========================+
| `doi-service#485`_ Enable Python 3.12 compatibility | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------+-----------------+---------------------------+

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

+---------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================================+=================+===========================+
| `ds-view#56`_ Fix potential XSS security vulnerability on ds-view   | |:blue_circle:| | s.high                    |
+---------------------------------------------------------------------+-----------------+---------------------------+
| `ds-view#53`_ DOIs are not properly resolving on some landing pages | |:blue_circle:| | s.medium                  |
+---------------------------------------------------------------------+-----------------+---------------------------+

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
`EdWG#28`_ Develop Service and Tools Context Products
+++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`EdWG#53`_ Phase 1: PDS Website Page Content Migration
++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`EdWG#85`_ Gather Investigation Imagery
+++++++++++++++++++++++++++++++++++++++

+-----------------------------------------+-----------------+---------------------------+
| Issue                                   | I&T Status      | Priority / Bug Severity   |
+=========================================+=================+===========================+
| `EdWG#85`_ Gather Investigation Imagery | |:blue_circle:| | p.could-have              |
+-----------------------------------------+-----------------+---------------------------+


`EdWG#86`_ Context Updates Phase 1: Facilities and Telescopes
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                         | I&T Status      | Priority / Bug Severity   |
+===============================================================+=================+===========================+
| `EdWG#86`_ Context Updates Phase 1: Facilities and Telescopes | |:blue_circle:| | p.should-have             |
+---------------------------------------------------------------+-----------------+---------------------------+


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

+------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                  | I&T Status       | Priority / Bug Severity   |
+========================================================================+==================+===========================+
| `harvest#283`_ Harvest cannot parse Date without time                  | |:green_circle:| | s.high                    |
+------------------------------------------------------------------------+------------------+---------------------------+
| `harvest#285`_ False positive Duplicate detected by harvest            | |:blue_circle:|  | s.medium                  |
+------------------------------------------------------------------------+------------------+---------------------------+
| `harvest#239`_ Harvest failing due to AOSS OCU limits without retrying | |:blue_circle:|  | s.high                    |
+------------------------------------------------------------------------+------------------+---------------------------+

Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                    | I&T Status       | Priority / Bug Severity   |
+==========================================================================================================================+==================+===========================+
| `harvest#261`_ As a user, I want harvest to raise an error if an attribute is not found in a local data dictionary (LDD) | |:green_circle:| | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `harvest#262`_ As a user, I want to ingest all XML attribute values (not PDS4 attributes) as string, by default          | |:blue_circle:|  | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

--------

Lasso-releasers
---------------
*Automatic "release" of software to artifact repositories, publishing packages for general availability*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/lasso-releasers#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/lasso-releasers>`_
     - `Issue Tracking <https://github.com/NASA-PDS/lasso-releasers/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/lasso-releasers/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/lasso-releasers/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/lasso-releasers/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                       | I&T Status      | Priority / Bug Severity   |
+=============================================================================================+=================+===========================+
| `lasso-releasers#5`_ Stable releases of ds-view are not publishing releases or their assets | |:blue_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`nucleus#127`_ [SBN] CSS: Deploy Nucleus to Prod and Kickoff Processing
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`nucleus#131`_ Update Architecture and Implement Separate EFS Per Node Baseline DAG
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================================================+=================+===========================+
| `nucleus#131`_ Update Architecture and Implement Separate EFS Per Node Baseline DAG | |:blue_circle:| | p.could-have              |
+-------------------------------------------------------------------------------------+-----------------+---------------------------+


`nucleus#138`_ [IMG] Onboard IMG Team to Monitor Nucleus LRO Processing
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`nucleus#142`_ Support Data Backlog Use Case
++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------+-----------------+---------------------------+
| Issue                                        | I&T Status      | Priority / Bug Severity   |
+==============================================+=================+===========================+
| `nucleus#142`_ Support Data Backlog Use Case | |:blue_circle:| | unknown                   |
+----------------------------------------------+-----------------+---------------------------+


`nucleus#147`_ Design and Prototype New Tracking Service
++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------+-----------------+---------------------------+
| Issue                                                    | I&T Status      | Priority / Bug Severity   |
+==========================================================+=================+===========================+
| `nucleus#147`_ Design and Prototype New Tracking Service | |:blue_circle:| | unknown                   |
+----------------------------------------------------------+-----------------+---------------------------+


`nucleus#149`_ Upgrade Nucleus to the latest 2.x version in MWAA
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                            | I&T Status      | Priority / Bug Severity   |
+==================================================================+=================+===========================+
| `nucleus#149`_ Upgrade Nucleus to the latest 2.x version in MWAA | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------+-----------------+---------------------------+


`nucleus#156`_ Develop a DAG Task Library
+++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------+-----------------+---------------------------+
| Issue                                     | I&T Status      | Priority / Bug Severity   |
+===========================================+=================+===========================+
| `nucleus#156`_ Develop a DAG Task Library | |:blue_circle:| | unknown                   |
+-------------------------------------------+-----------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================+=================+===========================+
| `nucleus#159`_ Invalid creation of archive buckets with terraform | |:blue_circle:| | s.medium                  |
+-------------------------------------------------------------------+-----------------+---------------------------+

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
`pds4-information-model#917`_ B16 Information Model SCR Implementation and LDDTool Updates
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                                  | I&T Status        | Level       | Priority / Bug Severity   |
+========================================================================================================================================================+===================+=============+===========================+
| `pds4-information-model#939`_ As a user, I want to know both the IM and LDD version applicable to a given attribute/class in the WebHelp documentation | |:green_circle:|  | requirement | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `pds4-information-model#938`_ Current WebHelp documentation (1O00/1.24.0.0) does not reflect latest Rings LDD                                          | |:blue_circle:|   | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `pds4-information-model#948`_ As a user, I want to override the default namespace version used by LDDTool                                              | |:green_circle:|  | requirement | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `pds4-information-model#967`_ CCB-28: As a user, I want validate to allow delimited tables with whitespace-only numeric fields                         | |:yellow_circle:| | task        | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `pds4-information-model#968`_ Upgrade to Java 17 for compatibility with validate dependency                                                            | |:blue_circle:|   | enhancement | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`pds4-information-model#920`_ B16 Information Model Delivery to I&T
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================================+=================+===========================+
| `pds4-information-model#920`_ B16 Information Model Delivery to I&T | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------+-----------------+---------------------------+


`pds4-information-model#921`_ B16 SCR Freeze
++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------+-----------------+---------------------------+
| Issue                                        | I&T Status      | Priority / Bug Severity   |
+==============================================+=================+===========================+
| `pds4-information-model#921`_ B16 SCR Freeze | |:blue_circle:| | p.must-have               |
+----------------------------------------------+-----------------+---------------------------+


`pds4-information-model#922`_ B16 Standards Documents Updates
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                         | I&T Status      | Priority / Bug Severity   |
+===============================================================+=================+===========================+
| `pds4-information-model#922`_ B16 Standards Documents Updates | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------+-----------------+---------------------------+


`pds4-information-model#926`_ Refactor PDS4 Data Dictionary Search to Support Scalability
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                      | I&T Status      | Priority / Bug Severity   |
+============================================================================================================+=================+===========================+
| `pds4-information-model#947`_ LDD generator is not generating valid LDDs                                   | |:blue_circle:| | s.high                    |
+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#951`_ PDS4 Instrument class (Product_Context) lists attributes that cannot be used | |:blue_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                                    | I&T Status       | Priority / Bug Severity   |
+==========================================================================================================================================+==================+===========================+
| `pds4-information-model#949`_ CCB-62: Transfer_Manifest class should enforce data types for its two mandatory columns                    | |:green_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `pds4-information-model#663`_ Adopt Provenance LDD for Superseded LIDs - CCB-21 (CCB-367)                                                | |:blue_circle:|  | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `pds4-information-model#946`_ CCB-59: funding_year only allows the value "9999"                                                          | |:green_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `pds4-information-model#945`_ CCB-60:  New permissible value for File_Area_Observational.Header.parsing_standard_id: "CDF 3.9 ISTP/IACG" | |:green_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                          | I&T Status      | Priority / Bug Severity   |
+================================================================================+=================+===========================+
| `pds4-information-model#953`_ [namespace-registry] add new namespace "galileo" | |:blue_circle:| | p.must-have               |
+--------------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#935`_ [namespace-registry] add new namespace "dscovr"  | |:blue_circle:| | p.must-have               |
+--------------------------------------------------------------------------------+-----------------+---------------------------+
| `pds4-information-model#958`_ [namespace-registry] add new namespace "prov"    | |:blue_circle:| | p.must-have               |
+--------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Pdsen-maven-parent
------------------
*PDS Engineering Node Maven Parent POM*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/pdsen-maven-parent#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/pdsen-maven-parent>`_
     - `Issue Tracking <https://github.com/NASA-PDS/pdsen-maven-parent/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/pdsen-maven-parent/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/pdsen-maven-parent/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/pdsen-maven-parent/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================================================+=================+===========================+
| `pdsen-maven-parent#70`_ Manually push 1.20.0 to maven central to enable update of registry tools | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------+------------------+---------------------------+
| Issue                                            | I&T Status       | Priority / Bug Severity   |
+==================================================+==================+===========================+
| `peppi#104`_ Simple Peppi query has long runtime | |:green_circle:| | s.medium                  |
+--------------------------------------------------+------------------+---------------------------+
| `peppi#102`_ as_dataframe method fails           | |:green_circle:| | s.high                    |
+--------------------------------------------------+------------------+---------------------------+

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
`planetary-data-cloud#87`_ Develop PDC User Engagement Strategy
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                           | I&T Status      | Priority / Bug Severity   |
+=================================================================+=================+===========================+
| `planetary-data-cloud#87`_ Develop PDC User Engagement Strategy | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#100`_ Phase 2 Migration of Existing Production JPL AWS Infra to MCP
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                     | I&T Status      | Priority / Bug Severity   |
+===========================================================================================+=================+===========================+
| `planetary-data-cloud#100`_ Phase 2 Migration of Existing Production JPL AWS Infra to MCP | |:blue_circle:| | unknown                   |
+-------------------------------------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#159`_ [IMG] LROC MVP: Setup IMG Prod Env, Replicate Data, Deploy Nucleus, and Kickoff Processing
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                                                    | I&T Status      | Level       | Priority / Bug Severity   |
+==========================================================================================================+=================+=============+===========================+
| `planetary-data-cloud#153`_ As a user, I need a lambda function to tag S3 objects based upon file suffix | |:blue_circle:| | requirement | p.must-have               |
+----------------------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


`planetary-data-cloud#117`_ Implement Optional Cognito Password Rotation Requirement (Disabled)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#139`_ Define Tagging Strategy for Planetary Data Cloud
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                        | I&T Status      | Priority / Bug Severity   |
+==============================================================================+=================+===========================+
| `planetary-data-cloud#139`_ Define Tagging Strategy for Planetary Data Cloud | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#144`_ Develop Egress Management Strategy
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                          | I&T Status      | Priority / Bug Severity   |
+================================================================+=================+===========================+
| `planetary-data-cloud#144`_ Develop Egress Management Strategy | |:blue_circle:| | p.must-have               |
+----------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#145`_ Develop Data Management and Storage Strategy
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                    | I&T Status      | Priority / Bug Severity   |
+==========================================================================+=================+===========================+
| `planetary-data-cloud#145`_ Develop Data Management and Storage Strategy | |:blue_circle:| | p.must-have               |
+--------------------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#146`_ B16 Cost Model Iteration with SMD Team
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                              | I&T Status      | Priority / Bug Severity   |
+====================================================================+=================+===========================+
| `planetary-data-cloud#146`_ B16 Cost Model Iteration with SMD Team | |:blue_circle:| | p.could-have              |
+--------------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#147`_ B16 Bi-annual Cloud Resource Housekeeping
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================+=================+===========================+
| `planetary-data-cloud#147`_ B16 Bi-annual Cloud Resource Housekeeping | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#164`_ Develop Process for Enabling Direct Public Access to S3 Buckets
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#165`_ Define PDC Assumed User Roles
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------+-----------------+---------------------------+
| Issue                                                     | I&T Status      | Priority / Bug Severity   |
+===========================================================+=================+===========================+
| `planetary-data-cloud#165`_ Define PDC Assumed User Roles | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#166`_ Update Data Backup Plan to Include OpenSearch and Cognito
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#184`_ Document Requirements and Guidelines for Archives to Support Cloud Infra
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`planetary-data-cloud#188`_ Document Archive Management Guidelines and Constraints
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                              | I&T Status      | Priority / Bug Severity   |
+====================================================================================+=================+===========================+
| `planetary-data-cloud#188`_ Document Archive Management Guidelines and Constraints | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------------+-----------------+---------------------------+


`planetary-data-cloud#193`_ B17 Bi-annual Cloud Resource Housekeeping
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================================================================+=================+===========================+
| `planetary-data-cloud#171`_ Cloudfront caching of API requests causing confusion with user expectations | |:blue_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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

+-------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================================================================+=================+===========================+
| `portal-tasks#123`_ Data release item details (data_product_information.cfm?) does not display on testing machine | |:blue_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `portal-tasks#129`_ ColdFusion applications do not fully function with MCP                                        | |:blue_circle:| | s.low                     |
+-------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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

`registry#370`_ Resurrect Legacy Registry Dashboards
++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------+-----------------+---------------------------+
| Issue                                                | I&T Status      | Priority / Bug Severity   |
+======================================================+=================+===========================+
| `registry#370`_ Resurrect Legacy Registry Dashboards | |:blue_circle:| | p.must-have               |
+------------------------------------------------------+-----------------+---------------------------+


`registry#371`_ Adapt Harvest to Support Using Inventories for Data File Metadata
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`registry#381`_ B16 Registry Maintenance: High Priority Enhancements / Bug Fixes / Tasks
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                                   | I&T Status      | Level       | Priority / Bug Severity   |
+=========================================================================================+=================+=============+===========================+
| `registry#380`_ CSV response not returning the values associated with `fields` argument | |:blue_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| `registry#375`_ product has date for sweeper index but is listed as not indexed         | |:blue_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| `registry#360`_ Fix GEO node products which ops:Harvest_Info/ops:node_name: geo         | |:blue_circle:| | enhancement | p.must-have               |
+-----------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| `registry#403`_ members of GEO bundle/collection collection not found                   | |:blue_circle:| | bug         | s.high                    |
+-----------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| `registry#440`_ Error `FIPS mode: only SunJSSE TrustManagers may be used`               | |:blue_circle:| | bug         | s.high                    |
+-----------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                    | I&T Status       | Priority / Bug Severity   |
+==========================================================================================================+==================+===========================+
| `registry#404`_ Registry is not accepting date time with leap second, e.g. `2015-06-30T23:59:60.862Z`    | |:green_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry#423`_ lid and pds:Identification_Area.pds:logical_identifier do not behave the same in the API | |:blue_circle:|  | s.medium                  |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry#422`_ Some of product urn:nasa:pds:lro_diviner_derived2::1.0's fields are not indexed          | |:blue_circle:|  | s.high                    |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Requirements
++++++++++++

+------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                              | I&T Status       | Priority / Bug Severity   |
+====================================================================================================================================+==================+===========================+
| `registry#113`_ As a node operator, I want the the registry schema to update autonomously / dynamically when new data is ingested. | |:blue_circle:|  | p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry#424`_ As a user, I want to receive an alert when my registry credentials are readable by someone else than myself        | |:green_circle:| | p.should-have             |
+------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry#396`_ As a node user, I want to have multiple cognito groups and still have the main cognito node group to be effective  | |:green_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

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

+----------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                              | I&T Status      | Priority / Bug Severity   |
+====================================================================================================+=================+===========================+
| `registry-api#622`_ Add Search Functionality to Find When Class / Attribute Has Been Used / Exists | |:blue_circle:| | unknown                   |
+----------------------------------------------------------------------------------------------------+-----------------+---------------------------+


`registry-api#623`_ Implement Registry API Performance Improvements
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================================+=================+===========================+
| `registry-api#623`_ Implement Registry API Performance Improvements | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------+-----------------+---------------------------+


`registry-api#632`_ Add Support for Searching Full PDS4 Structured Metadata
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                       | I&T Status        | Level       | Priority / Bug Severity   |
+=============================================================================================================+===================+=============+===========================+
| `registry-api#611`_ As a user, I want to search by a full/unique hierarchical path for a specific attribute | |:yellow_circle:| | requirement | p.must-have               |
+-------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`registry-api#633`_ Prototype Semantic Search Using AI / LLMs
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                         | I&T Status      | Priority / Bug Severity   |
+===============================================================+=================+===========================+
| `registry-api#633`_ Prototype Semantic Search Using AI / LLMs | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------+-----------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                               | I&T Status       | Priority / Bug Severity   |
+=====================================================================================================================================+==================+===========================+
| `registry-api#638`_ The API fails when no Accept header is provided                                                                 | |:green_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry-api#677`_ API search results using "search-after" returns empty [data] block even though I can find the product by lidvid | |:green_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry-api#705`_ Inconsistent support for `application/vnd.nasa.pds.pds4+json` response format                                   | |:green_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

--------

Registry-client
---------------
*A simple PDS Registry Client which authenticates users with PDS SSO and signs requests to the serverless OpenSearch (AOSS) hosting the Registry database.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://nasa-pds.github.io/registry-client>`_
     - `Github Repo <https://github.com/NASA-PDS/registry-client>`_
     - `Issue Tracking <https://github.com/NASA-PDS/registry-client/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/registry-client/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/registry-client/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/registry-client/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+--------------------------------------------------------+-----------------+---------------------------+
| Issue                                                  | I&T Status      | Priority / Bug Severity   |
+========================================================+=================+===========================+
| `registry-client#34`_ Enable Python 3.12 compatibility | |:blue_circle:| | p.must-have               |
+--------------------------------------------------------+-----------------+---------------------------+

--------

Registry-common
---------------
*Version<=2 of the library utilized by tools that manage and load data into the PDS Registry, including Harvest, Registry Manager, and Supplementer. Version 3+ is now managed through https://github.com/NASA-PDS/registry-loader/.*

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
Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                       | I&T Status      | Priority / Bug Severity   |
+=============================================================================================+=================+===========================+
| `registry-common#149`_ Default to throwing an error when an attribute is missing from a LDD | |:blue_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`registry-legacy-solr#200`_ B16 Registry Legacy Maintenance
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                       | I&T Status      | Priority / Bug Severity   |
+=============================================================+=================+===========================+
| `registry-legacy-solr#200`_ B16 Registry Legacy Maintenance | |:blue_circle:| | p.could-have              |
+-------------------------------------------------------------+-----------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+----------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                        | I&T Status      | Priority / Bug Severity   |
+==============================================================================================+=================+===========================+
| `registry-legacy-solr#217`_ Auto-restart the registry legacy docker container unless stopped | |:blue_circle:| | unknown                   |
+----------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`registry-loader#49`_ Develop Harvest and Registry Manager Test Framework
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+---------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================================+=================+===========================+
| `registry-loader#41`_ Merge registry-common, registry-mgr, harvest into one uber repo | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Registry-mgr
------------
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
~~~~~~~~~~~~~~~
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                            | I&T Status       | Priority / Bug Severity   |
+==================================================================================================================================+==================+===========================+
| `registry-mgr#134`_ registry-manager is incorrectly changing the archive_status of collection versions not in the bundle version | |:green_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `registry-mgr#137`_ set-archive-status is changing the status of more products than are in the bundle                            | |:green_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

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
`registry-sweepers#166`_ Optimize Sweepers Performance - Part 1
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                           | I&T Status      | Priority / Bug Severity   |
+=================================================================+=================+===========================+
| `registry-sweepers#166`_ Optimize Sweepers Performance - Part 1 | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------------+-----------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================+=================+===========================+
| `registry-sweepers#164`_ ATM Registry-Sweeper ECS task is failing | |:blue_circle:| | s.critical                |
+-------------------------------------------------------------------+-----------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------+-----------------+---------------------------+
| Issue                                                     | I&T Status      | Priority / Bug Severity   |
+===========================================================+=================+===========================+
| `registry-sweepers#181`_ Enable Python 3.12 compatibility | |:blue_circle:| | p.must-have               |
+-----------------------------------------------------------+-----------------+---------------------------+

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

+-------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================================================================================================+=================+===========================+
| `roundup-action#154`_ All stable builds are not tagging Releases in GitHub                                                                            | |:blue_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `roundup-action#157`_ Doc generation conflicting if package uses Sphinx extensions not in the GitHub actions base and tox generates conflicting files | |:blue_circle:| | s.medium                  |
+-------------------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

--------

Search-ui-legacy
----------------
*Legacy Keyword Search UI querying the Legacy Registry through Apache Solr.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://pds.nasa.gov/datasearch/keyword-search/>`_
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
Bugs
++++

+---------------------------------------------------+-----------------+---------------------------+
| Issue                                             | I&T Status      | Priority / Bug Severity   |
+===================================================+=================+===========================+
| `search-ui-legacy#59`_ Bug with XSS vulnerability | |:blue_circle:| | s.high                    |
+---------------------------------------------------+-----------------+---------------------------+

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
`software-issues-repo#118`_ 2025 Annual A&A Assessment Prep and Review
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                  | I&T Status      | Priority / Bug Severity   |
+========================================================================+=================+===========================+
| `software-issues-repo#118`_ 2025 Annual A&A Assessment Prep and Review | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------------+-----------------+---------------------------+


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


`software-issues-repo#122`_ B16 Code Freeze
+++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------+-----------------+---------------------------+
| Issue                                       | I&T Status      | Priority / Bug Severity   |
+=============================================+=================+===========================+
| `software-issues-repo#122`_ B16 Code Freeze | |:blue_circle:| | unknown                   |
+---------------------------------------------+-----------------+---------------------------+


`software-issues-repo#124`_ Re-imagine Data Release and DOI Processes in GitHub
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                           | I&T Status      | Priority / Bug Severity   |
+=================================================================================+=================+===========================+
| `software-issues-repo#124`_ Re-imagine Data Release and DOI Processes in GitHub | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------------------+-----------------+---------------------------+


`software-issues-repo#125`_ Complete ISA with NSSDCA
++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------+-----------------+---------------------------+
| Issue                                                | I&T Status      | Priority / Bug Severity   |
+======================================================+=================+===========================+
| `software-issues-repo#125`_ Complete ISA with NSSDCA | |:blue_circle:| | p.must-have               |
+------------------------------------------------------+-----------------+---------------------------+


`software-issues-repo#128`_ Upgrade Java Repos to use Maven Central Portal from OSSRH
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================================+=================+===========================+
| `software-issues-repo#128`_ Upgrade Java Repos to use Maven Central Portal from OSSRH | |:blue_circle:| | unknown                   |
+---------------------------------------------------------------------------------------+-----------------+---------------------------+


`software-issues-repo#139`_ Add Google Analytics to GitHub Sites
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                            | I&T Status      | Priority / Bug Severity   |
+==================================================================+=================+===========================+
| `software-issues-repo#139`_ Add Google Analytics to GitHub Sites | |:blue_circle:| | p.must-have               |
+------------------------------------------------------------------+-----------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+-------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================================================+=================+===========================+
| `software-issues-repo#135`_ Update LDD off-nominal release process to include regeneration of WebHelp | |:blue_circle:| | unknown                   |
+-------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `software-issues-repo#113`_ Create tool to generate SLOC reports for software deliveries              | |:blue_circle:| | unknown                   |
+-------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`system-i-n-t#67`_ B16 dLDD Integration & Test
++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------+-----------------+---------------------------+
| Issue                                          | I&T Status      | Priority / Bug Severity   |
+================================================+=================+===========================+
| `system-i-n-t#67`_ B16 dLDD Integration & Test | |:blue_circle:| | unknown                   |
+------------------------------------------------+-----------------+---------------------------+


`system-i-n-t#68`_ B16 Standards Document Review
++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------+-----------------+---------------------------+
| Issue                                            | I&T Status      | Priority / Bug Severity   |
+==================================================+=================+===========================+
| `system-i-n-t#68`_ B16 Standards Document Review | |:blue_circle:| | unknown                   |
+--------------------------------------------------+-----------------+---------------------------+


`system-i-n-t#69`_ B16 Test Readiness Review (TRR)
++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------+-----------------+---------------------------+
| Issue                                              | I&T Status      | Priority / Bug Severity   |
+====================================================+=================+===========================+
| `system-i-n-t#69`_ B16 Test Readiness Review (TRR) | |:blue_circle:| | unknown                   |
+----------------------------------------------------+-----------------+---------------------------+


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


`system-i-n-t#73`_ B16 Information Model I&T
++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------+-----------------+---------------------------+
| Issue                                        | I&T Status      | Priority / Bug Severity   |
+==============================================+=================+===========================+
| `system-i-n-t#73`_ B16 Information Model I&T | |:blue_circle:| | unknown                   |
+----------------------------------------------+-----------------+---------------------------+


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
`template-repo-python#104`_ Enable Code Coverage for Python repos
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                             | I&T Status      | Priority / Bug Severity   |
+===================================================================+=================+===========================+
| `template-repo-python#104`_ Enable Code Coverage for Python repos | |:blue_circle:| | p.could-have              |
+-------------------------------------------------------------------+-----------------+---------------------------+


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

+------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| Issue                                                                                                | I&T Status       | Level       | Priority / Bug Severity   |
+======================================================================================================+==================+=============+===========================+
| `validate#970`_ As a user, I want to includes titles and aliases in context product name validation  | |:green_circle:| | requirement | p.could-have              |
+------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#967`_ validate configuration includes context product names that do not match the products | |:green_circle:| | bug         | s.medium                  |
+------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+


`validate#1203`_ B16 High Priority Bug Fixes and Updated Standards Implementations
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| Issue                                                                                                                          | I&T Status       | Level       | Priority / Bug Severity   |
+================================================================================================================================+==================+=============+===========================+
| `validate#1201`_ As a user, I want validate to report empty (blank) PDS4 labels                                                | |:green_circle:| | requirement | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1234`_ validate does not raise a warning when a table has more records than label says it has                        | |:green_circle:| | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1276`_ `--strict-field-checks` not working as expected                                                               | |:green_circle:| | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1149`_ `validate-bundle` has no default value for `--report-dir`                                                     | |:blue_circle:|  | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1331`_ `validate-bundle` does not find same files as `validate` (uppercase label filenames)                          | |:blue_circle:|  | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1332`_ Validate Incorrectly Reports Overlap Error If Initial Bits Are Not Specified in Packed_Data_Fields            | |:green_circle:| | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1357`_ Encoded_External/encoding_standard_id does not allow NetCDF                                                   | |:green_circle:| | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1358`_ Validate doesn't correctly handle an integer value of valid_maximum associated with floating point data array | |:green_circle:| | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1359`_ Validate does not allow LIDVID for external products                                                          | |:green_circle:| | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1379`_ missing_constant treated differently to valid_minimim/valid_maximum                                           | |:green_circle:| | bug         | s.medium                  |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#1391`_ As a validate user, I want validate to allow delimited tables with whitespace-only numeric fields (CCB-28)    | |:green_circle:| | requirement | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                                                          | I&T Status       | Priority / Bug Severity   |
+================================================================================================================================================+==================+===========================+
| `validate#1408`_ JSON reports duplicates messages per product specified                                                                        | |:blue_circle:|  | s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#1241`_ Validating large data file (150GB) is trying to write the entire file to local temp space - error upon not enough local space | |:blue_circle:|  | s.high                    |
+------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#1316`_ Encoded_Audio encoding_standard_id = WAV gives MP4 error in Validate 3.7.1                                                    | |:green_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                            | I&T Status       | Priority / Bug Severity   |
+==================================================================================================+==================+===========================+
| `validate#1370`_ As a Validate user, I want to include the lidvid for each label in all reports  | |:blue_circle:|  | p.should-have             |
+--------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#1137`_ As a user, I want to know how much progress is being made during a validate run | |:green_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+-------------------------------------+-----------------+---------------------------+
| Issue                               | I&T Status      | Priority / Bug Severity   |
+=====================================+=================+===========================+
| `validate#1424`_ Upgrade to Java 17 | |:blue_circle:| | unknown                   |
+-------------------------------------+-----------------+---------------------------+

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
`web-analytics#50`_ Deploy Web Analytics System in Production
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                                      | I&T Status      | Level       | Priority / Bug Severity   |
+============================================================================================+=================+=============+===========================+
| `web-analytics#53`_ As a user, I want to automatically deploy all web analytics components | |:blue_circle:| | requirement | p.must-have               |
+--------------------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


`web-analytics#57`_ Complete Logstash Wrapper Tools for Prod Deployment
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================================+=================+===========================+
| `web-analytics#57`_ Complete Logstash Wrapper Tools for Prod Deployment | |:blue_circle:| | unknown                   |
+-------------------------------------------------------------------------+-----------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                 | I&T Status      | Priority / Bug Severity   |
+=======================================================================+=================+===========================+
| `web-analytics#51`_ `en-web-analytics` is locked up and unable to use | |:blue_circle:| | s.high                    |
+-----------------------------------------------------------------------+-----------------+---------------------------+

Enhancements
++++++++++++

+------------------------------------------------------+-----------------+---------------------------+
| Issue                                                | I&T Status      | Priority / Bug Severity   |
+======================================================+=================+===========================+
| `web-analytics#61`_ Enable Python 3.12 compatibility | |:blue_circle:| | p.must-have               |
+------------------------------------------------------+-----------------+---------------------------+

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

+-----------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                           | I&T Status      | Priority / Bug Severity   |
+=================================================================+=================+===========================+
| `web-modernization#257`_ Design Instrument Package Portal Pages | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------------+-----------------+---------------------------+


`web-modernization#258`_ Design Learning Hub Page
+++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------+-----------------+---------------------------+
| Issue                                             | I&T Status      | Priority / Bug Severity   |
+===================================================+=================+===========================+
| `web-modernization#258`_ Design Learning Hub Page | |:blue_circle:| | p.must-have               |
+---------------------------------------------------+-----------------+---------------------------+


`web-modernization#259`_ Design-System Housekeeping
+++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------+-----------------+---------------------------+
| Issue                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================+=================+===========================+
| `web-modernization#259`_ Design-System Housekeeping | |:blue_circle:| | unknown                   |
+-----------------------------------------------------+-----------------+---------------------------+


`web-modernization#260`_ Prototype Using LLMs for Training Support
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`web-modernization#261`_ Update Data Portal Pages to Better Support Programmatic and Cloud-enabled Access
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

`web-modernization#265`_ Design new Data Release Pages
++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No closed sub-issues identified for this theme in the current build yet. Click on the link in this section title for
    details.

Release Summary Metrics
=======================
This section provides a summary of the issues addressed in this release, organized by issue type.


+------------------------+--------+----------------+----------------+---------+----------+---------+
| Component/Repo         | Bugs   | Enhancements   | Requirements   | Tasks   | Themes   | Total   |
+========================+========+================+================+=========+==========+=========+
| EdWG                   | 0      | 0              | 0              | 0       | 4        | 4       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| data-upload-manager    | 3      | 1              | 4              | 0       | 5        | 13      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| deep-archive           | 2      | 1              | 2              | 0       | 2        | 7       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| devops                 | 0      | 0              | 0              | 0       | 1        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| doi-service            | 4      | 1              | 2              | 0       | 0        | 7       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| ds-view                | 2      | 0              | 0              | 0       | 0        | 2       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| harvest                | 3      | 0              | 2              | 0       | 0        | 5       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| lasso-releasers        | 1      | 0              | 0              | 0       | 0        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| nucleus                | 1      | 0              | 0              | 0       | 7        | 8       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| pds4-information-model | 3      | 4              | 6              | 0       | 5        | 18      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| pdsen-maven-parent     | 0      | 1              | 0              | 0       | 0        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| peppi                  | 2      | 0              | 0              | 0       | 0        | 2       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| planetary-data-cloud   | 1      | 0              | 1              | 0       | 15       | 17      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| portal-tasks           | 2      | 0              | 0              | 0       | 0        | 2       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry               | 7      | 1              | 3              | 0       | 5        | 16      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-api           | 3      | 0              | 1              | 0       | 5        | 9       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-client        | 0      | 1              | 0              | 0       | 0        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-common        | 0      | 1              | 0              | 0       | 0        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-legacy-solr   | 0      | 1              | 0              | 0       | 1        | 2       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-loader        | 0      | 1              | 0              | 0       | 1        | 2       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-mgr           | 2      | 0              | 0              | 0       | 0        | 2       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| registry-sweepers      | 1      | 1              | 0              | 0       | 1        | 3       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| roundup-action         | 2      | 0              | 0              | 0       | 0        | 2       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| search-ui-legacy       | 1      | 0              | 0              | 0       | 0        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| software-issues-repo   | 0      | 2              | 0              | 0       | 8        | 10      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| system-i-n-t           | 0      | 0              | 0              | 0       | 7        | 7       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| template-repo-python   | 0      | 0              | 0              | 0       | 1        | 1       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| validate               | 13     | 1              | 5              | 0       | 2        | 21      |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| web-analytics          | 1      | 1              | 1              | 0       | 2        | 5       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| web-modernization      | 0      | 0              | 0              | 0       | 6        | 6       |
+------------------------+--------+----------------+----------------+---------+----------+---------+
| **TOTAL**              | **54** | **18**         | **27**         | **0**   | **78**   | **177** |
+------------------------+--------+----------------+----------------+---------+----------+---------+


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
.. _pds4-information-model#663: https://github.com/NASA-PDS/pds4-information-model/issues/663
.. _pds4-information-model#945: https://github.com/NASA-PDS/pds4-information-model/issues/945
.. _pds4-information-model#946: https://github.com/NASA-PDS/pds4-information-model/issues/946
.. _pds4-information-model#949: https://github.com/NASA-PDS/pds4-information-model/issues/949
.. _pds4-information-model#967: https://github.com/NASA-PDS/pds4-information-model/issues/967
.. _data-upload-manager#207: https://github.com/NASA-PDS/data-upload-manager/issues/207
.. _data-upload-manager#221: https://github.com/NASA-PDS/data-upload-manager/issues/221
.. _data-upload-manager#224: https://github.com/NASA-PDS/data-upload-manager/issues/224
.. _data-upload-manager#264: https://github.com/NASA-PDS/data-upload-manager/issues/264
.. _data-upload-manager#224: https://github.com/NASA-PDS/data-upload-manager/issues/224
.. _data-upload-manager#231: https://github.com/NASA-PDS/data-upload-manager/issues/231
.. _data-upload-manager#232: https://github.com/NASA-PDS/data-upload-manager/issues/232
.. _data-upload-manager#256: https://github.com/NASA-PDS/data-upload-manager/issues/256
.. _data-upload-manager#209: https://github.com/NASA-PDS/data-upload-manager/issues/209
.. _data-upload-manager#264: https://github.com/NASA-PDS/data-upload-manager/issues/264
.. _data-upload-manager#282: https://github.com/NASA-PDS/data-upload-manager/issues/282
.. _data-upload-manager#241: https://github.com/NASA-PDS/data-upload-manager/issues/241
.. _data-upload-manager#271: https://github.com/NASA-PDS/data-upload-manager/issues/271
.. _data-upload-manager#99: https://github.com/NASA-PDS/data-upload-manager/issues/99
.. _data-upload-manager#289: https://github.com/NASA-PDS/data-upload-manager/issues/289
.. _deep-archive#204: https://github.com/NASA-PDS/deep-archive/issues/204
.. _deep-archive#157: https://github.com/NASA-PDS/deep-archive/issues/157
.. _deep-archive#210: https://github.com/NASA-PDS/deep-archive/issues/210
.. _deep-archive#208: https://github.com/NASA-PDS/deep-archive/issues/208
.. _deep-archive#136: https://github.com/NASA-PDS/deep-archive/issues/136
.. _deep-archive#213: https://github.com/NASA-PDS/deep-archive/issues/213
.. _deep-archive#218: https://github.com/NASA-PDS/deep-archive/issues/218
.. _devops#81: https://github.com/NASA-PDS/devops/issues/81
.. _doi-service#455: https://github.com/NASA-PDS/doi-service/issues/455
.. _doi-service#466: https://github.com/NASA-PDS/doi-service/issues/466
.. _doi-service#456: https://github.com/NASA-PDS/doi-service/issues/456
.. _doi-service#476: https://github.com/NASA-PDS/doi-service/issues/476
.. _doi-service#478: https://github.com/NASA-PDS/doi-service/issues/478
.. _doi-service#432: https://github.com/NASA-PDS/doi-service/issues/432
.. _doi-service#485: https://github.com/NASA-PDS/doi-service/issues/485
.. _ds-view#56: https://github.com/NASA-PDS/ds-view/issues/56
.. _ds-view#53: https://github.com/NASA-PDS/ds-view/issues/53
.. _EdWG#28: https://github.com/NASA-PDS/EdWG/issues/28
.. _EdWG#53: https://github.com/NASA-PDS/EdWG/issues/53
.. _EdWG#85: https://github.com/NASA-PDS/EdWG/issues/85
.. _EdWG#86: https://github.com/NASA-PDS/EdWG/issues/86
.. _harvest#283: https://github.com/NASA-PDS/harvest/issues/283
.. _harvest#285: https://github.com/NASA-PDS/harvest/issues/285
.. _harvest#239: https://github.com/NASA-PDS/harvest/issues/239
.. _harvest#261: https://github.com/NASA-PDS/harvest/issues/261
.. _harvest#262: https://github.com/NASA-PDS/harvest/issues/262
.. _lasso-releasers#5: https://github.com/NASA-PDS/lasso-releasers/issues/5
.. _nucleus#127: https://github.com/NASA-PDS/nucleus/issues/127
.. _nucleus#131: https://github.com/NASA-PDS/nucleus/issues/131
.. _nucleus#138: https://github.com/NASA-PDS/nucleus/issues/138
.. _nucleus#142: https://github.com/NASA-PDS/nucleus/issues/142
.. _nucleus#147: https://github.com/NASA-PDS/nucleus/issues/147
.. _nucleus#149: https://github.com/NASA-PDS/nucleus/issues/149
.. _nucleus#156: https://github.com/NASA-PDS/nucleus/issues/156
.. _nucleus#159: https://github.com/NASA-PDS/nucleus/issues/159
.. _pds4-information-model#917: https://github.com/NASA-PDS/pds4-information-model/issues/917
.. _pds4-information-model#939: https://github.com/NASA-PDS/pds4-information-model/issues/939
.. _pds4-information-model#938: https://github.com/NASA-PDS/pds4-information-model/issues/938
.. _pds4-information-model#948: https://github.com/NASA-PDS/pds4-information-model/issues/948
.. _pds4-information-model#967: https://github.com/NASA-PDS/pds4-information-model/issues/967
.. _pds4-information-model#968: https://github.com/NASA-PDS/pds4-information-model/issues/968
.. _pds4-information-model#920: https://github.com/NASA-PDS/pds4-information-model/issues/920
.. _pds4-information-model#921: https://github.com/NASA-PDS/pds4-information-model/issues/921
.. _pds4-information-model#922: https://github.com/NASA-PDS/pds4-information-model/issues/922
.. _pds4-information-model#926: https://github.com/NASA-PDS/pds4-information-model/issues/926
.. _pds4-information-model#947: https://github.com/NASA-PDS/pds4-information-model/issues/947
.. _pds4-information-model#951: https://github.com/NASA-PDS/pds4-information-model/issues/951
.. _pds4-information-model#949: https://github.com/NASA-PDS/pds4-information-model/issues/949
.. _pds4-information-model#663: https://github.com/NASA-PDS/pds4-information-model/issues/663
.. _pds4-information-model#946: https://github.com/NASA-PDS/pds4-information-model/issues/946
.. _pds4-information-model#945: https://github.com/NASA-PDS/pds4-information-model/issues/945
.. _pds4-information-model#953: https://github.com/NASA-PDS/pds4-information-model/issues/953
.. _pds4-information-model#935: https://github.com/NASA-PDS/pds4-information-model/issues/935
.. _pds4-information-model#958: https://github.com/NASA-PDS/pds4-information-model/issues/958
.. _pdsen-maven-parent#70: https://github.com/NASA-PDS/pdsen-maven-parent/issues/70
.. _peppi#104: https://github.com/NASA-PDS/peppi/issues/104
.. _peppi#102: https://github.com/NASA-PDS/peppi/issues/102
.. _planetary-data-cloud#87: https://github.com/NASA-PDS/planetary-data-cloud/issues/87
.. _planetary-data-cloud#100: https://github.com/NASA-PDS/planetary-data-cloud/issues/100
.. _planetary-data-cloud#159: https://github.com/NASA-PDS/planetary-data-cloud/issues/159
.. _planetary-data-cloud#153: https://github.com/NASA-PDS/planetary-data-cloud/issues/153
.. _planetary-data-cloud#117: https://github.com/NASA-PDS/planetary-data-cloud/issues/117
.. _planetary-data-cloud#139: https://github.com/NASA-PDS/planetary-data-cloud/issues/139
.. _planetary-data-cloud#144: https://github.com/NASA-PDS/planetary-data-cloud/issues/144
.. _planetary-data-cloud#145: https://github.com/NASA-PDS/planetary-data-cloud/issues/145
.. _planetary-data-cloud#146: https://github.com/NASA-PDS/planetary-data-cloud/issues/146
.. _planetary-data-cloud#147: https://github.com/NASA-PDS/planetary-data-cloud/issues/147
.. _planetary-data-cloud#164: https://github.com/NASA-PDS/planetary-data-cloud/issues/164
.. _planetary-data-cloud#165: https://github.com/NASA-PDS/planetary-data-cloud/issues/165
.. _planetary-data-cloud#166: https://github.com/NASA-PDS/planetary-data-cloud/issues/166
.. _planetary-data-cloud#184: https://github.com/NASA-PDS/planetary-data-cloud/issues/184
.. _planetary-data-cloud#188: https://github.com/NASA-PDS/planetary-data-cloud/issues/188
.. _planetary-data-cloud#193: https://github.com/NASA-PDS/planetary-data-cloud/issues/193
.. _planetary-data-cloud#171: https://github.com/NASA-PDS/planetary-data-cloud/issues/171
.. _portal-tasks#123: https://github.com/NASA-PDS/portal-tasks/issues/123
.. _portal-tasks#129: https://github.com/NASA-PDS/portal-tasks/issues/129
.. _registry#266: https://github.com/NASA-PDS/registry/issues/266
.. _registry#333: https://github.com/NASA-PDS/registry/issues/333
.. _registry#370: https://github.com/NASA-PDS/registry/issues/370
.. _registry#371: https://github.com/NASA-PDS/registry/issues/371
.. _registry#381: https://github.com/NASA-PDS/registry/issues/381
.. _registry#380: https://github.com/NASA-PDS/registry/issues/380
.. _registry#375: https://github.com/NASA-PDS/registry/issues/375
.. _registry#360: https://github.com/NASA-PDS/registry/issues/360
.. _registry#403: https://github.com/NASA-PDS/registry/issues/403
.. _registry#440: https://github.com/NASA-PDS/registry/issues/440
.. _registry#404: https://github.com/NASA-PDS/registry/issues/404
.. _registry#423: https://github.com/NASA-PDS/registry/issues/423
.. _registry#422: https://github.com/NASA-PDS/registry/issues/422
.. _registry#113: https://github.com/NASA-PDS/registry/issues/113
.. _registry#424: https://github.com/NASA-PDS/registry/issues/424
.. _registry#396: https://github.com/NASA-PDS/registry/issues/396
.. _registry-api#715: https://github.com/NASA-PDS/registry-api/issues/715
.. _registry-api#622: https://github.com/NASA-PDS/registry-api/issues/622
.. _registry-api#623: https://github.com/NASA-PDS/registry-api/issues/623
.. _registry-api#632: https://github.com/NASA-PDS/registry-api/issues/632
.. _registry-api#611: https://github.com/NASA-PDS/registry-api/issues/611
.. _registry-api#633: https://github.com/NASA-PDS/registry-api/issues/633
.. _registry-api#638: https://github.com/NASA-PDS/registry-api/issues/638
.. _registry-api#677: https://github.com/NASA-PDS/registry-api/issues/677
.. _registry-api#705: https://github.com/NASA-PDS/registry-api/issues/705
.. _registry-client#34: https://github.com/NASA-PDS/registry-client/issues/34
.. _registry-common#149: https://github.com/NASA-PDS/registry-common/issues/149
.. _registry-legacy-solr#200: https://github.com/NASA-PDS/registry-legacy-solr/issues/200
.. _registry-legacy-solr#217: https://github.com/NASA-PDS/registry-legacy-solr/issues/217
.. _registry-loader#49: https://github.com/NASA-PDS/registry-loader/issues/49
.. _registry-loader#41: https://github.com/NASA-PDS/registry-loader/issues/41
.. _registry-mgr#134: https://github.com/NASA-PDS/registry-mgr/issues/134
.. _registry-mgr#137: https://github.com/NASA-PDS/registry-mgr/issues/137
.. _registry-sweepers#166: https://github.com/NASA-PDS/registry-sweepers/issues/166
.. _registry-sweepers#164: https://github.com/NASA-PDS/registry-sweepers/issues/164
.. _registry-sweepers#181: https://github.com/NASA-PDS/registry-sweepers/issues/181
.. _roundup-action#154: https://github.com/NASA-PDS/roundup-action/issues/154
.. _roundup-action#157: https://github.com/NASA-PDS/roundup-action/issues/157
.. _search-ui-legacy#59: https://github.com/NASA-PDS/search-ui-legacy/issues/59
.. _software-issues-repo#118: https://github.com/NASA-PDS/software-issues-repo/issues/118
.. _software-issues-repo#120: https://github.com/NASA-PDS/software-issues-repo/issues/120
.. _software-issues-repo#121: https://github.com/NASA-PDS/software-issues-repo/issues/121
.. _software-issues-repo#122: https://github.com/NASA-PDS/software-issues-repo/issues/122
.. _software-issues-repo#124: https://github.com/NASA-PDS/software-issues-repo/issues/124
.. _software-issues-repo#125: https://github.com/NASA-PDS/software-issues-repo/issues/125
.. _software-issues-repo#128: https://github.com/NASA-PDS/software-issues-repo/issues/128
.. _software-issues-repo#139: https://github.com/NASA-PDS/software-issues-repo/issues/139
.. _software-issues-repo#135: https://github.com/NASA-PDS/software-issues-repo/issues/135
.. _software-issues-repo#113: https://github.com/NASA-PDS/software-issues-repo/issues/113
.. _system-i-n-t#67: https://github.com/NASA-PDS/system-i-n-t/issues/67
.. _system-i-n-t#68: https://github.com/NASA-PDS/system-i-n-t/issues/68
.. _system-i-n-t#69: https://github.com/NASA-PDS/system-i-n-t/issues/69
.. _system-i-n-t#70: https://github.com/NASA-PDS/system-i-n-t/issues/70
.. _system-i-n-t#71: https://github.com/NASA-PDS/system-i-n-t/issues/71
.. _system-i-n-t#72: https://github.com/NASA-PDS/system-i-n-t/issues/72
.. _system-i-n-t#73: https://github.com/NASA-PDS/system-i-n-t/issues/73
.. _template-repo-python#104: https://github.com/NASA-PDS/template-repo-python/issues/104
.. _validate#1184: https://github.com/NASA-PDS/validate/issues/1184
.. _validate#970: https://github.com/NASA-PDS/validate/issues/970
.. _validate#967: https://github.com/NASA-PDS/validate/issues/967
.. _validate#1203: https://github.com/NASA-PDS/validate/issues/1203
.. _validate#1201: https://github.com/NASA-PDS/validate/issues/1201
.. _validate#1234: https://github.com/NASA-PDS/validate/issues/1234
.. _validate#1276: https://github.com/NASA-PDS/validate/issues/1276
.. _validate#1149: https://github.com/NASA-PDS/validate/issues/1149
.. _validate#1331: https://github.com/NASA-PDS/validate/issues/1331
.. _validate#1332: https://github.com/NASA-PDS/validate/issues/1332
.. _validate#1357: https://github.com/NASA-PDS/validate/issues/1357
.. _validate#1358: https://github.com/NASA-PDS/validate/issues/1358
.. _validate#1359: https://github.com/NASA-PDS/validate/issues/1359
.. _validate#1379: https://github.com/NASA-PDS/validate/issues/1379
.. _validate#1391: https://github.com/NASA-PDS/validate/issues/1391
.. _validate#1408: https://github.com/NASA-PDS/validate/issues/1408
.. _validate#1241: https://github.com/NASA-PDS/validate/issues/1241
.. _validate#1316: https://github.com/NASA-PDS/validate/issues/1316
.. _validate#1370: https://github.com/NASA-PDS/validate/issues/1370
.. _validate#1137: https://github.com/NASA-PDS/validate/issues/1137
.. _validate#1424: https://github.com/NASA-PDS/validate/issues/1424
.. _web-analytics#50: https://github.com/NASA-PDS/web-analytics/issues/50
.. _web-analytics#53: https://github.com/NASA-PDS/web-analytics/issues/53
.. _web-analytics#57: https://github.com/NASA-PDS/web-analytics/issues/57
.. _web-analytics#51: https://github.com/NASA-PDS/web-analytics/issues/51
.. _web-analytics#61: https://github.com/NASA-PDS/web-analytics/issues/61
.. _web-modernization#257: https://github.com/NASA-PDS/web-modernization/issues/257
.. _web-modernization#258: https://github.com/NASA-PDS/web-modernization/issues/258
.. _web-modernization#259: https://github.com/NASA-PDS/web-modernization/issues/259
.. _web-modernization#260: https://github.com/NASA-PDS/web-modernization/issues/260
.. _web-modernization#261: https://github.com/NASA-PDS/web-modernization/issues/261
.. _web-modernization#265: https://github.com/NASA-PDS/web-modernization/issues/265
.. _Software Release Summary (B16): https://nasa-pds.github.io/releases/16/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md