==========================================
Release Description Document (Build B15.0)
==========================================
This release of the PDS4 System is intended as an operational release of the system components to date.
The original plan for this release can be found here: `plan B15.0`_

The following sections can be found in this document:

.. toctree::
   :glob:
   :maxdepth: 3

   rdd.rst


PDS4 Standards and Information Model Changes
============================================
This section details the changes to the PDS4 Standards and Information Model approved by the PDS4 Change Control Board
and implemented by the PDS within the latest build period.

+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| Ref                           | Title                                                                                                                               |
+===============================+=====================================================================================================================================+
| `pds4-information-model#753`_ | CCB-16: Allow micro amps and nano amps as units of current                                                                          |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#782`_ | CCB-26: Fix definition of Units_of_Amount_of_Substance                                                                              |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#784`_ | CCB-18: Complete JIRA-CCB-325 lien implementation for Browse and Ancillary products                                                 |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#795`_ | CCB-7: Missing schematron rule - bundle_to_targets                                                                                  |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#816`_ | CCB-29: Incorrect schematron rules for Bundle (type:External), Collection (type:External), and Product_External logical_identifiers |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#823`_ | CCB-27: DOI requires at least an author or editor                                                                                   |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#824`_ | CCB-24: Replaced all of the unit_id standard value definitions                                                                      |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#829`_ | CCB-38: Added mrad/pixel to Units_of_Pixel_Resolution_Angular                                                                       |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#830`_ | CCB-47: Add permissible value W/cm**2/sr/μm to Units_of_Spectral_Radiance                                                           |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#831`_ | CCB-42: Add Array_1D_Spectrum to File_Area_Ancillary, File_Area_Browse, and File_Area_Observational_Supplemental                    |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#838`_ | CCB-10: Schematron/Schema Version Conflict (PDS-JIRA-366)                                                                           |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
| `pds4-information-model#839`_ | CCB-19: Never finished CCB-325 documentation updates (Title: Support for video and audio as product observational)                  |
+-------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+

Software Changes
================
For each software repository, the changes are listed in 2 categories:

- Planned Updates
- Other Updates

The 'Planned Updates' are organized by 'Themes' (or 'Release Themes'), which are defined in advance and approved by the
PDS Software Working Group (see `Plan B15.0`_).

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
`data-upload-manager#51`_ Add User-Defined Object Metadata
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                                     | I&T Status        | Level       | Priority / Bug Severity   |
+===========================================================================================================================================================+===================+=============+===========================+
| `data-upload-manager#50`_ As a user, I want to include a MD5 checksum in the the user-defined object metadata being sent in the upload payload            | |:yellow_circle:| | requirement | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `data-upload-manager#87`_ As a user, I want to include the modification datetime in the the user-defined object metadata being sent in the upload payload | |:yellow_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`data-upload-manager#84`_ Improve DUM Upload Performance and Avoid Replication of Files in the Cloud
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                          | I&T Status        | Level       | Priority / Bug Severity   |
+================================================================================================================+===================+=============+===========================+
| `data-upload-manager#92`_ As a user, I want to skip upload of files already in S3 (nucleus staging bucket)     | |:yellow_circle:| | requirement | p.must-have               |
+----------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `data-upload-manager#98`_ As a user, I want an end summary report in logs to show statistics of files uploaded | |:yellow_circle:| | requirement | p.should-have             |
+----------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================================================================+===================+===========================+
| `data-upload-manager#110`_ DUM Client does not properly sanitize double-quotes from INI config                        | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `data-upload-manager#116`_ DUM Lambda Service can return pre-signed S3 URL's to non-existing buckets                  | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `data-upload-manager#136`_ Backoff/Retry logic not firing for certain error codes                                     | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `data-upload-manager#135`_ DUM Client script does not respect configured logging level after a transfer failure/retry | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+----------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================+===================+===========================+
| `deep-archive#178`_ Issues with manifests after multiple slash update fix (#162) | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------+-------------------+---------------------------+
| `deep-archive#171`_ Failing build due to deprecated config                       | |:blue_circle:|   | s.high                    |
+----------------------------------------------------------------------------------+-------------------+---------------------------+
| `deep-archive#186`_ AIP now fails validation after #178 update                   | |:blue_circle:|   | s.high                    |
+----------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                        | I&T Status        | Priority / Bug Severity   |
+==============================================================================================================+===================+===========================+
| `deep-archive#162`_ As a data custodian, I want the Deep Archive to work around invalid URLs in the Registry | |:yellow_circle:| | p.must-have               |
+--------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                                                    | I&T Status      | Priority / Bug Severity   |
+==========================================================================================================================================+=================+===========================+
| `doi-service#430`_ Installation instructions are not entirely clear, and come back with issues about incompatible libraries in python 11 | |:blue_circle:| | unknown                   |
+------------------------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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
`EdWG#6`_ Phase 1: Context Product Scrub
++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+--------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                              | I&T Status      | Priority / Bug Severity   |
+====================================================================+=================+===========================+
| `EdWG#15`_ Update context products with latest production versions | |:blue_circle:| | p.must-have               |
+--------------------------------------------------------------------+-----------------+---------------------------+

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
`harvest#131`_ Enhance support for searching lid/lidvid references
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                                              | I&T Status        | Level   | Priority / Bug Severity   |
+====================================================================================+===================+=========+===========================+
| `harvest#127`_ ref_lid_* fields are not added to the Registry schema prior to load | |:yellow_circle:| | bug     | s.medium                  |
+------------------------------------------------------------------------------------+-------------------+---------+---------------------------+


`harvest#135`_ As a user, I want the default archive_status for loaded products to be configurable
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                         | I&T Status        | Priority / Bug Severity   |
+===============================================================================================================+===================+===========================+
| `harvest#158`_ As a data custodian, I want to load URLs / file paths without unnecessary / additional slashes | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Monitoring
----------
*Monitoring configuration for PDS EN system, currently based on AWS CloudWatch*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/monitoring#readme>`_
     - `Github Repo <https://github.com/NASA-PDS/monitoring>`_
     - `Issue Tracking <https://github.com/NASA-PDS/monitoring/issues>`_ 
     - `Requirements <https://github.com/NASA-PDS/monitoring/tree/main/docs/requirements>`_ 
     - `Stable Release <https://github.com/NASA-PDS/monitoring/releases/latest>`_ 
     - `Dev Release <https://github.com/NASA-PDS/monitoring/releases>`_ 


Planned Updates
~~~~~~~~~~~~~~~
`monitoring#15`_ Develop MCP OU Structure, Cost Monitoring, and Cost Management Policies
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------+-----------------+-------------+---------------------------+
| Issue                                                                            | I&T Status      | Level       | Priority / Bug Severity   |
+==================================================================================+=================+=============+===========================+
| `monitoring#14`_ As a user, I want a daily budget reports sent to my email inbox | |:blue_circle:| | requirement | p.should-have             |
+----------------------------------------------------------------------------------+-----------------+-------------+---------------------------+


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
`nucleus#91`_ Implement Warm Backup Storage Solution (Data Backup Plan)
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                            | I&T Status        | Level       | Priority / Bug Severity   |
+==================================================================================================+===================+=============+===========================+
| `nucleus#73`_ As a user, I want to store a copy of my archive data in AWS Deep Archive / Glacier | |:yellow_circle:| | requirement | p.must-have               |
+--------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`nucleus#93`_ CSS MVP: Deploy Baseline Nucleus for Catalina Sky Survey in Test and Production Environments
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+--------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                            | I&T Status        | Level       | Priority / Bug Severity   |
+==================================================================================================+===================+=============+===========================+
| `nucleus#73`_ As a user, I want to store a copy of my archive data in AWS Deep Archive / Glacier | |:yellow_circle:| | requirement | p.must-have               |
+--------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+--------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                | I&T Status        | Priority / Bug Severity   |
+======================================================================================+===================+===========================+
| `nucleus#101`_ Nucleus MWAA DAG tasks are unable to read remote logs from Cloudwatch | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`pds4-information-model#701`_ Initial Implementation of Cucumber Framework for PDS4 IM Repo
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#728`_ B15.0 SCR Freeze
++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#729`_ B15.0 Standards Documents Updates
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#730`_ B15.0 Information Model Delivery to I&T
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds4-information-model#731`_ B15.0 Information Model SCR Implementation
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| Issue                                                                            | I&T Status       | Level       | Priority / Bug Severity   |
+==================================================================================+==================+=============+===========================+
| `pds4-information-model#795`_ CCB-7: Missing schematron rule - bundle_to_targets | |:green_circle:| | requirement | p.must-have               |
+----------------------------------------------------------------------------------+------------------+-------------+---------------------------+


`pds4-information-model#732`_ B15.0 Planetary Systems Target Ontology: Rings, Satellites Small Bodies Phase 1
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================================================================+===================+===========================+
| `pds4-information-model#818`_ LDDTool does not resolve the JUICE namespaces with IM 1J00                                         | |:blue_circle:|   | s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#776`_ Unable to build LDDs for 1E00                                                                      | |:blue_circle:|   | s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#797`_ GEOM LDD schematron rules are not executing as expected `<kernel_type>` validation                 | |:yellow_circle:| | s.critical                |
+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#801`_ Lack of object initialization in the code leads to infinite when trying to run main more than once | |:blue_circle:|   | s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#770`_ ERROR 11179 data dictionary class is missing for overwrite                                         | |:blue_circle:|   | s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#819`_ Regression in schematron improvements for references (#795)                                        | |:blue_circle:|   | s.critical                |
+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================================================================================================+===================+===========================+
| `pds4-information-model#838`_ CCB-10: Schematron/Schema Version Conflict (PDS-JIRA-366)                                                                           | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#753`_ CCB-16: Allow micro amps and nano amps as units of current                                                                          | |:green_circle:|  | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#829`_ CCB-38: Added mrad/pixel to Units_of_Pixel_Resolution_Angular                                                                       | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#816`_ CCB-29: Incorrect schematron rules for Bundle (type:External), Collection (type:External), and Product_External logical_identifiers | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#823`_ CCB-27: DOI requires at least an author or editor                                                                                   | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#839`_ CCB-19: Never finished CCB-325 documentation updates (Title: Support for video and audio as product observational)                  | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#824`_ CCB-24: Replaced all of the unit_id standard value definitions                                                                      | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#831`_ CCB-42: Add Array_1D_Spectrum to File_Area_Ancillary, File_Area_Browse, and File_Area_Observational_Supplemental                    | |:green_circle:|  | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#830`_ CCB-47: Add permissible value W/cm**2/sr/μm to Units_of_Spectral_Radiance                                                           | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#782`_ CCB-26: Fix definition of Units_of_Amount_of_Substance                                                                              | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                               | I&T Status       | Priority / Bug Severity   |
+=====================================================================================+==================+===========================+
| `pds4-information-model#803`_ [namespace-registry] add new namespace juice          | |:blue_circle:|  | p.must-have               |
+-------------------------------------------------------------------------------------+------------------+---------------------------+
| `pds4-information-model#794`_ [namespace-registry] add new namespace `vikinglander` | |:green_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------+------------------+---------------------------+

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
Requirements
++++++++++++

+---------------------------------------------------------+-----------------+---------------------------+
| Issue                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================+=================+===========================+
| `pds4-jparser#142`_ As a user, I want to read 4D arrays | |:blue_circle:| | p.should-have             |
+---------------------------------------------------------+-----------------+---------------------------+

--------

Peppi
-----
*Planetary Data Explorere: Python (PEPPi) library (pds.peppi) to access Planetary Data from the Planetary Data System (formerly known as updart)*

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
Requirements
++++++++++++

+------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                        | I&T Status        | Priority / Bug Severity   |
+==============================================================================+===================+===========================+
| `peppi#7`_ As a user, I want to support search-after pagination              | |:yellow_circle:| | p.should-have             |
+------------------------------------------------------------------------------+-------------------+---------------------------+
| `peppi#29`_ As a user, I want to search for products based upon a target LID | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------------------------+-------------------+---------------------------+

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
`planetary-data-cloud#73`_ ATLAS MVP: Support Development of Initial Migration Plan and Architecture for ATLAS Survey Data
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-cloud#103`_ B15.0 Bi-annual Cloud Resource Housekeeping
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================+===================+===========================+
| `planetary-data-cloud#108`_ [SECURITY] Ensure CloudFront distributions have logging enabled-PDS | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+-----------------------------------------------------+-----------------+---------------------------+
| Issue                                               | I&T Status      | Priority / Bug Severity   |
+=====================================================+=================+===========================+
| `planetarydata.org#25`_ Typo                        | |:blue_circle:| | s.medium                  |
+-----------------------------------------------------+-----------------+---------------------------+
| `planetarydata.org#23`_ Updates to web site content | |:blue_circle:| | s.low                     |
+-----------------------------------------------------+-----------------+---------------------------+
| `planetarydata.org#24`_ Old link to PSA             | |:blue_circle:| | s.medium                  |
+-----------------------------------------------------+-----------------+---------------------------+

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

+----------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                      | I&T Status      | Priority / Bug Severity   |
+============================================================================+=================+===========================+
| `portal-tasks#95`_ Broken links for 1.21.0.0 and 1.22.0.0                  | |:blue_circle:| | s.high                    |
+----------------------------------------------------------------------------+-----------------+---------------------------+
| `portal-tasks#96`_ Bug with Tool Registry with new Registry                | |:blue_circle:| | s.high                    |
+----------------------------------------------------------------------------+-----------------+---------------------------+
| `portal-tasks#97`_ Tool Registry no longer works with new Registry Servlet | |:blue_circle:| | s.critical                |
+----------------------------------------------------------------------------+-----------------+---------------------------+

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
`portal-wp-tasks#58`_ Phase 1: Search Implementation
++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`portal-wp-tasks#59`_ Phase 1: Investigations Directory Page Module Implementation
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`portal-wp-tasks#60`_ Phase 1: Investigation Landing Page Module Implementation
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

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
`registry#185`_ Implement Registry Multi-tenancy with Cognito in the loop
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                              | I&T Status        | Priority / Bug Severity   |
+====================================================================================================+===================+===========================+
| `registry#292`_ Secret detection is broken on branch titan_treks_utility_script                    | |:blue_circle:|   | s.medium                  |
+----------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry#276`_ harvest created archive_status as an array and registry-mgr updates it as a string | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`registry-api#424`_ API MVP to utilize Amazon OpenSearch Serverless
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`registry-api#428`_ Implement expected `latest` functionality for all endpoints
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                                                                  | I&T Status        | Level       | Priority / Bug Severity   |
+========================================================================================================================================================================================+===================+=============+===========================+
| `registry-api#435`_ As a user, by default, I want to resolve the latest version of a product when given a product logical_identifier (LID) (`/products/{logical_identifier}` endpoint) | |:yellow_circle:| | requirement | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`registry-api#505`_ Multi-tenancy Migration MVP Tasks
+++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                         | I&T Status      | Priority / Bug Severity   |
+===============================================================================+=================+===========================+
| `registry-api#431`_ Investigate sporadic 500 and 504 errors with registry API | |:blue_circle:| | s.medium                  |
+-------------------------------------------------------------------------------+-----------------+---------------------------+
| `registry-api#522`_ Fix code scanning alerts per logging                      | |:blue_circle:| | s.high                    |
+-------------------------------------------------------------------------------+-----------------+---------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                                         | I&T Status        | Priority / Bug Severity   |
+===============================================================================================================================================================================+===================+===========================+
| `registry-api#426`_ As a user, by default, I want to search only for the latest versions of all products on the `/products` endpoint                                          | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#491`_ As a user, I want to apply an additional query filter (`q=`) to the `/products/{identifier}/member-of` result set                                         | |:green_circle:|  | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#488`_ As a user, by default, I want to search for the latest versions of all products on the `/classes/{class}` endpoint unless explicitly requested            | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#486`_ As a user, by default, I want to search for only the latest versions of all products on the `/products/{identifier}/member-of` endpoint                   | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#506`_ As a user, I want to know what are all the possible properties I can search against (`/properties`)                                                       | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#436`_ As a user, I want to get all product versions associated to one lid                                                                                       | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#490`_ As a user, I want to apply an additional query filter (`q=`) to members of the members of an aggregate product (`/products/{identifier}/members/members`) | |:green_circle:|  | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#497`_ As a user, I want to receive metadata only in the API responses (no binary blobs)                                                                         | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#485`_ As a user, by default, I want to search for only the latest versions of all products on the `/products/{identifier}/members/members` endpoint             | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#493`_ As a user, I want to apply an additional query filter (`q=`) to the `/classes/{class}` result set                                                         | |:green_circle:|  | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#484`_ As a user, by default, I want to search for only the latest versions of all products on the `/products/{identifier}/members` endpoint                     | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#495`_ As a user, I want to filter the products by any available PDS4 property by combining comparison operators using logical operators                         | |:green_circle:|  | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#516`_ As a user, I want to get a description of the API when I request it from its base URL in a web browser                                                    | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#492`_ As a user, I want to apply an additional query filter (`q=`) to the `/products/{identifier}/member-of/member-of` result set                               | |:green_circle:|  | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#469`_ As a user, I want to filter the products by any available PDS4 property using a combination of comparison, logical, and precedence grouping operators     | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#434`_ As a user, I want to get a product description given a lidvid                                                                                             | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#511`_ As a user, I want to get all the products for a specific PDS4 product class                                                                               | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#494`_ As a user, I want to filter the products by any available PDS4 property using comparison operators                                                        | |:green_circle:|  | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#298`_ As a user, I want to apply an additional query filter (`q=`) to members of an aggregate product (`/products/{identifier}/members`)                        | |:green_circle:|  | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#487`_ As a user, by default, I want to search only for the latest versions of all products on the `/products/{identifier}/member-of/member-of` endpoint         | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
Bugs
++++

+--------------------------------------------------+------------------+---------------------------+
| Issue                                            | I&T Status       | Priority / Bug Severity   |
+==================================================+==================+===========================+
| `registry-client#3`_ pypi installation is broken | |:green_circle:| | s.high                    |
+--------------------------------------------------+------------------+---------------------------+

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

+-----------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================================================+=================+===========================+
| `registry-common#50`_ Update registry-common library to support change to AWS interface | |:blue_circle:| | s.critical                |
+-----------------------------------------------------------------------------------------+-----------------+---------------------------+
| `registry-common#53`_ Update OpenSearch API call to use `search()` instead of `get()`   | |:blue_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------+-----------------+---------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                         | I&T Status      | Priority / Bug Severity   |
+===============================================================================+=================+===========================+
| `registry-legacy-solr#130`_ Unable to set custom facet fields (`facet.field`) | |:blue_circle:| | s.critical                |
+-------------------------------------------------------------------------------+-----------------+---------------------------+

Enhancements
++++++++++++

+-----------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                     | I&T Status      | Priority / Bug Severity   |
+===========================================================================================================+=================+===========================+
| `registry-legacy-solr#76`_ Refactor legacy search-core dependencies to include classes explicitly in repo | |:blue_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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

+----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                          | I&T Status        | Priority / Bug Severity   |
+================================================================================================================+===================+===========================+
| `registry-mgr#78`_ set-archive-status and delete-data subcommand do not work on OpenSearch serverless Registry | |:yellow_circle:| | s.critical                |
+----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                      | I&T Status        | Priority / Bug Severity   |
+============================================================================+===================+===========================+
| `registry-mgr#69`_ As a user, I want to set archive-status using packageId | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------+-------------------+---------------------------+

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

+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================================================+===================+===========================+
| `roundup-action#138`_ Maven deploy no longer works due to Maven central upgrade                                         | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `roundup-action#142`_ Roundup failing on tagging stable release for pds4-information-model                              | |:blue_circle:|   | s.high                    |
+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `roundup-action#139`_ Unstable Pipeline failing with unsatisfiable install dependency on Data Upload Manager repository | |:yellow_circle:| | s.high                    |
+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

S3-browser-cloudfront
---------------------
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
~~~~~~~~~~~~~~~
`s3-browser-cloudfront#23`_ Adapt S3 Browser to work for PDC and ODR buckets
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                        | I&T Status        | Level       | Priority / Bug Severity   |
+==============================================================================================+===================+=============+===========================+
| `s3-browser-cloudfront#22`_ As a data user, I want to view ODR S3 bucket with S3 browser app | |:yellow_circle:| | requirement | p.must-have               |
+----------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                 | I&T Status        | Priority / Bug Severity   |
+=======================================================================+===================+===========================+
| `s3-browser-cloudfront#113`_ Links to data or label files  are broken | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================================================================================+=================+===========================+
| `s3-browser-cloudfront#68`_ As a manager, I want the S3-browser to be deployable and accessible from a '/some_path' URL | |:blue_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

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

+-------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                         | I&T Status      | Priority / Bug Severity   |
+===============================================================================+=================+===========================+
| `search-ui-legacy#30`_ Fix code scanning alert per Log Injection              | |:blue_circle:| | s.critical                |
+-------------------------------------------------------------------------------+-----------------+---------------------------+
| `search-ui-legacy#35`_ Faceting no longer works since XssUtils was introduced | |:blue_circle:| | s.critical                |
+-------------------------------------------------------------------------------+-----------------+---------------------------+

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
`software-issues-repo#76`_ Distribute ISAs for Signature Cycle
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#86`_ Complete Tasks and Artifacts Supporting NASA A&A Process
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#98`_ B15.0 Release Planning
+++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#99`_ B15.0 Prep for I&T
+++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#100`_ B15.0 Code Freeze
+++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

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
`system-i-n-t#52`_ B15.0 Delivery & Deployment Review Preparation
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`system-i-n-t#54`_ B15.0 System Integration & Test
++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`system-i-n-t#55`_ B15.0 Test Readiness Review (TRR)
++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

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
`validate#696`_ Use New Registry API for Context Product Validation
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                  | I&T Status        | Level       | Priority / Bug Severity   |
+========================================================================================+===================+=============+===========================+
| `validate#675`_ Cutover to using new Registry API for generating context products json | |:yellow_circle:| | enhancement | p.must-have               |
+----------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`validate#832`_ Review Handling of Special Constants, Field Formats, and High Priority Bug Fixes
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| Issue                                                                                                                                         | I&T Status       | Level       | Priority / Bug Severity   |
+===============================================================================================================================================+==================+=============+===========================+
| `validate#816`_ As a user, I want a WARNING to be thrown when a delimited or character table value does not match the expected `field_format` | |:green_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#817`_ As a user, I want an ERROR to be thrown when a character table value does not match the expected `validation_format`          | |:green_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#831`_ validate incorrectly handles special constant high_instrument_saturation                                                      | |:green_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#837`_ In text tables, validate attempts to match pattern associated with `data_type` before checking `Special_Constants`            | |:green_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#849`_ Validate stalls when validating collection inventory file with duplicates records                                             | |:green_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#873`_ Validate 3.5.0-snapshot Giving Unexpected Errors for Matching Filenames in Separate Directories                               | |:green_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#874`_ SXXP0003 Error when running on PDS3 data sets for v3.3.3 or v3.4.1                                                            | |:blue_circle:|  | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#903`_ Validate not retrying on sch load failure                                                                                     | |:blue_circle:|  | bug         | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#905`_ Validate 3.5.0-snapshot gives error when encountering Document objects/files used in other Document products.                 | |:green_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+


`validate#860`_ Add Warning Messages for Context Product Name Mismatches
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| Issue                                                                                                                                                     | I&T Status       | Level       | Priority / Bug Severity   |
+===========================================================================================================================================================+==================+=============+===========================+
| `validate#857`_ As a user, I want to receive a WARNING message when the `Observing_System_Component.name` does not match the value in the context product | |:green_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+
| `validate#861`_ As a user, I want to receive a WARNING message when the `Target_Identification.name` does not match the value in the context product      | |:green_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+------------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| Issue                                                                                                    | I&T Status       | Priority / Bug Severity   |
+==========================================================================================================+==================+===========================+
| `validate#915`_ `context_ref_mismatch` check only executes when -R pds4.label                            | |:green_circle:| | s.low                     |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#822`_ Check for unlabeled files no longer works                                                | |:green_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#936`_ Validate does not show correct filename for PDF/A failures when validating a directory   | |:blue_circle:|  | s.medium                  |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#902`_ Validate error during JPEG content validation                                            | |:green_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#1034`_ `validate --update-context-products` no longer works with Solr upgrade                  | |:green_circle:| | s.critical                |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#923`_ Configuration file parser does not reject incorrect options                              | |:blue_circle:|  | s.medium                  |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#1054`_ `validate.bat` no executes correctly on windows                                         | |:blue_circle:|  | s.critical                |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#950`_ `--disable-context-mismatch-warnings` only works for rule `pds4.label`                   | |:green_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#919`_ Validate throws an error when UnsignedBitString has 61 bits                              | |:green_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#826`_ validate is slow or runs out of memory when validating a bundle                          | |:blue_circle:|  | s.medium                  |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#933`_ Missing operation documentation                                                          | |:green_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#969`_ Slow performance with all content and product validation turned off                      | |:blue_circle:|  | s.medium                  |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+
| `validate#823`_ Validate V.3.4.1 reports file read errors on products which read correctly under V.3.2.0 | |:green_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+------------------+---------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------+------------------+---------------------------+
| Issue                                                       | I&T Status       | Priority / Bug Severity   |
+=============================================================+==================+===========================+
| `validate#824`_ Check for PDF/A-1a only if Product_Document | |:green_circle:| | p.should-have             |
+-------------------------------------------------------------+------------------+---------------------------+

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
`web-analytics#30`_ Automate Log Sync to S3 and Athena
++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`web-analytics#32`_ Document Strategy for Web Analytics System Migration to MCP
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                            | I&T Status      | Priority / Bug Severity   |
+==================================================================+=================+===========================+
| `web-analytics#12`_ Sync script fails silently if aws call fails | |:blue_circle:| | s.medium                  |
+------------------------------------------------------------------+-----------------+---------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| Issue                                                                                                                   | I&T Status      | Priority / Bug Severity   |
+=========================================================================================================================+=================+===========================+
| `web-analytics#39`_ update repo with template files                                                                     | |:blue_circle:| | unknown                   |
+-------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+
| `web-analytics#24`_ As a user, I want a mission-specific dashboard showing instrument and product type download metrics | |:blue_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------+-----------------+---------------------------+

Liens
=====

+---------+---------+-------------+
| Issue   | Title   | Rationale   |
+=========+=========+=============+
+---------+---------+-------------+

Engineering Node Software Catalog
=================================
The Engineering Node Software resources are listed in the `Software Release Summary (B15.0)`_

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

.. _plan B15.0: https://nasa-pds.github.io/releases/15.0/plan.html
.. _pds4-information-model#753: https://github.com/NASA-PDS/pds4-information-model/issues/753
.. _pds4-information-model#782: https://github.com/NASA-PDS/pds4-information-model/issues/782
.. _pds4-information-model#784: https://github.com/NASA-PDS/pds4-information-model/issues/784
.. _pds4-information-model#795: https://github.com/NASA-PDS/pds4-information-model/issues/795
.. _pds4-information-model#816: https://github.com/NASA-PDS/pds4-information-model/issues/816
.. _pds4-information-model#823: https://github.com/NASA-PDS/pds4-information-model/issues/823
.. _pds4-information-model#824: https://github.com/NASA-PDS/pds4-information-model/issues/824
.. _pds4-information-model#829: https://github.com/NASA-PDS/pds4-information-model/issues/829
.. _pds4-information-model#830: https://github.com/NASA-PDS/pds4-information-model/issues/830
.. _pds4-information-model#831: https://github.com/NASA-PDS/pds4-information-model/issues/831
.. _pds4-information-model#838: https://github.com/NASA-PDS/pds4-information-model/issues/838
.. _pds4-information-model#839: https://github.com/NASA-PDS/pds4-information-model/issues/839
.. _data-upload-manager#51: https://github.com/NASA-PDS/data-upload-manager/issues/51
.. _data-upload-manager#50: https://github.com/NASA-PDS/data-upload-manager/issues/50
.. _data-upload-manager#87: https://github.com/NASA-PDS/data-upload-manager/issues/87
.. _data-upload-manager#84: https://github.com/NASA-PDS/data-upload-manager/issues/84
.. _data-upload-manager#92: https://github.com/NASA-PDS/data-upload-manager/issues/92
.. _data-upload-manager#98: https://github.com/NASA-PDS/data-upload-manager/issues/98
.. _data-upload-manager#110: https://github.com/NASA-PDS/data-upload-manager/issues/110
.. _data-upload-manager#116: https://github.com/NASA-PDS/data-upload-manager/issues/116
.. _data-upload-manager#136: https://github.com/NASA-PDS/data-upload-manager/issues/136
.. _data-upload-manager#135: https://github.com/NASA-PDS/data-upload-manager/issues/135
.. _deep-archive#178: https://github.com/NASA-PDS/deep-archive/issues/178
.. _deep-archive#171: https://github.com/NASA-PDS/deep-archive/issues/171
.. _deep-archive#186: https://github.com/NASA-PDS/deep-archive/issues/186
.. _deep-archive#162: https://github.com/NASA-PDS/deep-archive/issues/162
.. _doi-service#430: https://github.com/NASA-PDS/doi-service/issues/430
.. _EdWG#6: https://github.com/NASA-PDS/EdWG/issues/6
.. _EdWG#15: https://github.com/NASA-PDS/EdWG/issues/15
.. _harvest#131: https://github.com/NASA-PDS/harvest/issues/131
.. _harvest#127: https://github.com/NASA-PDS/harvest/issues/127
.. _harvest#135: https://github.com/NASA-PDS/harvest/issues/135
.. _harvest#158: https://github.com/NASA-PDS/harvest/issues/158
.. _monitoring#15: https://github.com/NASA-PDS/monitoring/issues/15
.. _monitoring#14: https://github.com/NASA-PDS/monitoring/issues/14
.. _nucleus#91: https://github.com/NASA-PDS/nucleus/issues/91
.. _nucleus#73: https://github.com/NASA-PDS/nucleus/issues/73
.. _nucleus#93: https://github.com/NASA-PDS/nucleus/issues/93
.. _nucleus#73: https://github.com/NASA-PDS/nucleus/issues/73
.. _nucleus#101: https://github.com/NASA-PDS/nucleus/issues/101
.. _pds4-information-model#701: https://github.com/NASA-PDS/pds4-information-model/issues/701
.. _pds4-information-model#728: https://github.com/NASA-PDS/pds4-information-model/issues/728
.. _pds4-information-model#729: https://github.com/NASA-PDS/pds4-information-model/issues/729
.. _pds4-information-model#730: https://github.com/NASA-PDS/pds4-information-model/issues/730
.. _pds4-information-model#731: https://github.com/NASA-PDS/pds4-information-model/issues/731
.. _pds4-information-model#795: https://github.com/NASA-PDS/pds4-information-model/issues/795
.. _pds4-information-model#732: https://github.com/NASA-PDS/pds4-information-model/issues/732
.. _pds4-information-model#818: https://github.com/NASA-PDS/pds4-information-model/issues/818
.. _pds4-information-model#776: https://github.com/NASA-PDS/pds4-information-model/issues/776
.. _pds4-information-model#797: https://github.com/NASA-PDS/pds4-information-model/issues/797
.. _pds4-information-model#801: https://github.com/NASA-PDS/pds4-information-model/issues/801
.. _pds4-information-model#770: https://github.com/NASA-PDS/pds4-information-model/issues/770
.. _pds4-information-model#819: https://github.com/NASA-PDS/pds4-information-model/issues/819
.. _pds4-information-model#838: https://github.com/NASA-PDS/pds4-information-model/issues/838
.. _pds4-information-model#753: https://github.com/NASA-PDS/pds4-information-model/issues/753
.. _pds4-information-model#829: https://github.com/NASA-PDS/pds4-information-model/issues/829
.. _pds4-information-model#816: https://github.com/NASA-PDS/pds4-information-model/issues/816
.. _pds4-information-model#823: https://github.com/NASA-PDS/pds4-information-model/issues/823
.. _pds4-information-model#839: https://github.com/NASA-PDS/pds4-information-model/issues/839
.. _pds4-information-model#824: https://github.com/NASA-PDS/pds4-information-model/issues/824
.. _pds4-information-model#831: https://github.com/NASA-PDS/pds4-information-model/issues/831
.. _pds4-information-model#830: https://github.com/NASA-PDS/pds4-information-model/issues/830
.. _pds4-information-model#782: https://github.com/NASA-PDS/pds4-information-model/issues/782
.. _pds4-information-model#803: https://github.com/NASA-PDS/pds4-information-model/issues/803
.. _pds4-information-model#794: https://github.com/NASA-PDS/pds4-information-model/issues/794
.. _pds4-jparser#142: https://github.com/NASA-PDS/pds4-jparser/issues/142
.. _peppi#7: https://github.com/NASA-PDS/peppi/issues/7
.. _peppi#29: https://github.com/NASA-PDS/peppi/issues/29
.. _planetary-data-cloud#73: https://github.com/NASA-PDS/planetary-data-cloud/issues/73
.. _planetary-data-cloud#103: https://github.com/NASA-PDS/planetary-data-cloud/issues/103
.. _planetary-data-cloud#108: https://github.com/NASA-PDS/planetary-data-cloud/issues/108
.. _planetarydata.org#25: https://github.com/NASA-PDS/planetarydata.org/issues/25
.. _planetarydata.org#23: https://github.com/NASA-PDS/planetarydata.org/issues/23
.. _planetarydata.org#24: https://github.com/NASA-PDS/planetarydata.org/issues/24
.. _portal-tasks#95: https://github.com/NASA-PDS/portal-tasks/issues/95
.. _portal-tasks#96: https://github.com/NASA-PDS/portal-tasks/issues/96
.. _portal-tasks#97: https://github.com/NASA-PDS/portal-tasks/issues/97
.. _portal-wp-tasks#58: https://github.com/NASA-PDS/portal-wp-tasks/issues/58
.. _portal-wp-tasks#59: https://github.com/NASA-PDS/portal-wp-tasks/issues/59
.. _portal-wp-tasks#60: https://github.com/NASA-PDS/portal-wp-tasks/issues/60
.. _registry#185: https://github.com/NASA-PDS/registry/issues/185
.. _registry#292: https://github.com/NASA-PDS/registry/issues/292
.. _registry#276: https://github.com/NASA-PDS/registry/issues/276
.. _registry-api#424: https://github.com/NASA-PDS/registry-api/issues/424
.. _registry-api#428: https://github.com/NASA-PDS/registry-api/issues/428
.. _registry-api#435: https://github.com/NASA-PDS/registry-api/issues/435
.. _registry-api#505: https://github.com/NASA-PDS/registry-api/issues/505
.. _registry-api#431: https://github.com/NASA-PDS/registry-api/issues/431
.. _registry-api#522: https://github.com/NASA-PDS/registry-api/issues/522
.. _registry-api#426: https://github.com/NASA-PDS/registry-api/issues/426
.. _registry-api#491: https://github.com/NASA-PDS/registry-api/issues/491
.. _registry-api#488: https://github.com/NASA-PDS/registry-api/issues/488
.. _registry-api#486: https://github.com/NASA-PDS/registry-api/issues/486
.. _registry-api#506: https://github.com/NASA-PDS/registry-api/issues/506
.. _registry-api#436: https://github.com/NASA-PDS/registry-api/issues/436
.. _registry-api#490: https://github.com/NASA-PDS/registry-api/issues/490
.. _registry-api#497: https://github.com/NASA-PDS/registry-api/issues/497
.. _registry-api#485: https://github.com/NASA-PDS/registry-api/issues/485
.. _registry-api#493: https://github.com/NASA-PDS/registry-api/issues/493
.. _registry-api#484: https://github.com/NASA-PDS/registry-api/issues/484
.. _registry-api#495: https://github.com/NASA-PDS/registry-api/issues/495
.. _registry-api#516: https://github.com/NASA-PDS/registry-api/issues/516
.. _registry-api#492: https://github.com/NASA-PDS/registry-api/issues/492
.. _registry-api#469: https://github.com/NASA-PDS/registry-api/issues/469
.. _registry-api#434: https://github.com/NASA-PDS/registry-api/issues/434
.. _registry-api#511: https://github.com/NASA-PDS/registry-api/issues/511
.. _registry-api#494: https://github.com/NASA-PDS/registry-api/issues/494
.. _registry-api#298: https://github.com/NASA-PDS/registry-api/issues/298
.. _registry-api#487: https://github.com/NASA-PDS/registry-api/issues/487
.. _registry-client#3: https://github.com/NASA-PDS/registry-client/issues/3
.. _registry-common#50: https://github.com/NASA-PDS/registry-common/issues/50
.. _registry-common#53: https://github.com/NASA-PDS/registry-common/issues/53
.. _registry-legacy-solr#130: https://github.com/NASA-PDS/registry-legacy-solr/issues/130
.. _registry-legacy-solr#76: https://github.com/NASA-PDS/registry-legacy-solr/issues/76
.. _registry-mgr#78: https://github.com/NASA-PDS/registry-mgr/issues/78
.. _registry-mgr#69: https://github.com/NASA-PDS/registry-mgr/issues/69
.. _roundup-action#138: https://github.com/NASA-PDS/roundup-action/issues/138
.. _roundup-action#142: https://github.com/NASA-PDS/roundup-action/issues/142
.. _roundup-action#139: https://github.com/NASA-PDS/roundup-action/issues/139
.. _s3-browser-cloudfront#23: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/23
.. _s3-browser-cloudfront#22: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/22
.. _s3-browser-cloudfront#113: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/113
.. _s3-browser-cloudfront#68: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/68
.. _search-ui-legacy#30: https://github.com/NASA-PDS/search-ui-legacy/issues/30
.. _search-ui-legacy#35: https://github.com/NASA-PDS/search-ui-legacy/issues/35
.. _software-issues-repo#76: https://github.com/NASA-PDS/software-issues-repo/issues/76
.. _software-issues-repo#86: https://github.com/NASA-PDS/software-issues-repo/issues/86
.. _software-issues-repo#98: https://github.com/NASA-PDS/software-issues-repo/issues/98
.. _software-issues-repo#99: https://github.com/NASA-PDS/software-issues-repo/issues/99
.. _software-issues-repo#100: https://github.com/NASA-PDS/software-issues-repo/issues/100
.. _system-i-n-t#52: https://github.com/NASA-PDS/system-i-n-t/issues/52
.. _system-i-n-t#54: https://github.com/NASA-PDS/system-i-n-t/issues/54
.. _system-i-n-t#55: https://github.com/NASA-PDS/system-i-n-t/issues/55
.. _validate#696: https://github.com/NASA-PDS/validate/issues/696
.. _validate#675: https://github.com/NASA-PDS/validate/issues/675
.. _validate#832: https://github.com/NASA-PDS/validate/issues/832
.. _validate#816: https://github.com/NASA-PDS/validate/issues/816
.. _validate#817: https://github.com/NASA-PDS/validate/issues/817
.. _validate#831: https://github.com/NASA-PDS/validate/issues/831
.. _validate#837: https://github.com/NASA-PDS/validate/issues/837
.. _validate#849: https://github.com/NASA-PDS/validate/issues/849
.. _validate#873: https://github.com/NASA-PDS/validate/issues/873
.. _validate#874: https://github.com/NASA-PDS/validate/issues/874
.. _validate#903: https://github.com/NASA-PDS/validate/issues/903
.. _validate#905: https://github.com/NASA-PDS/validate/issues/905
.. _validate#860: https://github.com/NASA-PDS/validate/issues/860
.. _validate#857: https://github.com/NASA-PDS/validate/issues/857
.. _validate#861: https://github.com/NASA-PDS/validate/issues/861
.. _validate#915: https://github.com/NASA-PDS/validate/issues/915
.. _validate#822: https://github.com/NASA-PDS/validate/issues/822
.. _validate#936: https://github.com/NASA-PDS/validate/issues/936
.. _validate#902: https://github.com/NASA-PDS/validate/issues/902
.. _validate#1034: https://github.com/NASA-PDS/validate/issues/1034
.. _validate#923: https://github.com/NASA-PDS/validate/issues/923
.. _validate#1054: https://github.com/NASA-PDS/validate/issues/1054
.. _validate#950: https://github.com/NASA-PDS/validate/issues/950
.. _validate#919: https://github.com/NASA-PDS/validate/issues/919
.. _validate#826: https://github.com/NASA-PDS/validate/issues/826
.. _validate#933: https://github.com/NASA-PDS/validate/issues/933
.. _validate#969: https://github.com/NASA-PDS/validate/issues/969
.. _validate#823: https://github.com/NASA-PDS/validate/issues/823
.. _validate#824: https://github.com/NASA-PDS/validate/issues/824
.. _web-analytics#30: https://github.com/NASA-PDS/web-analytics/issues/30
.. _web-analytics#32: https://github.com/NASA-PDS/web-analytics/issues/32
.. _web-analytics#12: https://github.com/NASA-PDS/web-analytics/issues/12
.. _web-analytics#39: https://github.com/NASA-PDS/web-analytics/pull/39
.. _web-analytics#24: https://github.com/NASA-PDS/web-analytics/issues/24
.. _Software Release Summary (B15.0): https://nasa-pds.github.io/releases/15.0/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md