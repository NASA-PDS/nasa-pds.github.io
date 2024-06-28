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

+-------------------------------+------------------------------------------------------+
| Ref                           | Title                                                |
+===============================+======================================================+
| `pds4-information-model#784`_ | Never finished CCB-325 lien for browse and ancillary |
+-------------------------------+------------------------------------------------------+

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


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                | I&T Status        | Priority / Bug Severity   |
+======================================================================================================+===================+===========================+
| `data-upload-manager#116`_ DUM Lambda Service can return pre-signed S3 URL's to non-existing buckets | |:yellow_circle:| | p.must-have               |
+------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `data-upload-manager#110`_ DUM Client does not properly sanitize double-quotes from INI config       | |:yellow_circle:| | s.high                    |
+------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                          | I&T Status        | Priority / Bug Severity   |
+================================================================================================================+===================+===========================+
| `data-upload-manager#92`_ As a user, I want to skip upload of files already in S3 (nucleus staging bucket)     | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `data-upload-manager#98`_ As a user, I want an end summary report in logs to show statistics of files uploaded | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                              | I&T Status        | Priority / Bug Severity   |
+====================================================================================+===================+===========================+
| `harvest#127`_ ref_lid_* fields are not added to the Registry schema prior to load | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                         | I&T Status        | Priority / Bug Severity   |
+===============================================================================================================+===================+===========================+
| `harvest#158`_ As a data custodian, I want to load URLs / file paths without unnecessary / additional slashes | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================================================+===================+===========================+
| `pds4-information-model#770`_ ERROR 11179 data dictionary class is missing for overwrite | |:yellow_circle:| | s.high                    |
+------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#776`_ Unable to build LDDs for 1E00                              | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
No planned updates realized for this build in this repository.

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
Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================================================================================+===================+===========================+
| `registry-pds3-catalog#16`_ As a user, I want to provide search/access links using the hsk.cat files within the data set | |:yellow_circle:| | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================================================================+===================+===========================+
| `registry-sweepers#112`_ `superseded_by` fields with `null` values causing multiple versions of same products to appear in API searches | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+---------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================+===================+===========================+
| `roundup-action#138`_ Maven deploy no longer works due to Maven central upgrade | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------+-------------------+---------------------------+

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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+----------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                        | I&T Status        | Priority / Bug Severity   |
+==============================================================================================+===================+===========================+
| `s3-browser-cloudfront#22`_ As a data user, I want to view ODR S3 bucket with S3 browser app | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================+===================+===========================+
| `search-ui-legacy#30`_ Fix code scanning alert per Log Injection | |:yellow_circle:| | s.critical                |
+------------------------------------------------------------------+-------------------+---------------------------+

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
`software-issues-repo#86`_ Complete Tasks and Artifacts Supporting NASA A&A Process
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`software-issues-repo#98`_ B15.0 Release Planning
+++++++++++++++++++++++++++++++++++++++++++++++++
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
`validate#832`_ Review Handling of Special Constants, Field Formats, and High Priority Bug Fixes
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                         | I&T Status        | Level       | Priority / Bug Severity   |
+===============================================================================================================================================+===================+=============+===========================+
| `validate#816`_ As a user, I want a WARNING to be thrown when a delimited or character table value does not match the expected `field_format` | |:yellow_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#817`_ As a user, I want an ERROR to be thrown when a character table value does not match the expected `validation_format`          | |:yellow_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#831`_ validate incorrectly handles special constant high_instrument_saturation                                                      | |:yellow_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#837`_ In text tables, validate attempts to match pattern associated with `data_type` before checking `Special_Constants`            | |:yellow_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#849`_ Validate stalls when validating collection inventory file with duplicates records                                             | |:yellow_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#873`_ Validate 3.5.0-snapshot Giving Unexpected Errors for Matching Filenames in Separate Directories                               | |:yellow_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#874`_ SXXP0003 Error when running on PDS3 data sets for v3.3.3 or v3.4.1                                                            | |:yellow_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#903`_ Validate not retrying on sch load failure                                                                                     | |:yellow_circle:| | bug         | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#905`_ Validate 3.5.0-snapshot gives error when encountering Document objects/files used in other Document products.                 | |:yellow_circle:| | bug         | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`validate#860`_ Add Warning Messages for Context Product Name Mismatches
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                                     | I&T Status        | Level       | Priority / Bug Severity   |
+===========================================================================================================================================================+===================+=============+===========================+
| `validate#857`_ As a user, I want to receive a WARNING message when the `Observing_System_Component.name` does not match the value in the context product | |:yellow_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#861`_ As a user, I want to receive a WARNING message when the `Target_Identification.name` does not match the value in the context product      | |:yellow_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================================================================+===================+===========================+
| `validate#823`_ Validate V.3.4.1 reports file read errors on products which read correctly under V.3.2.0 | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#826`_ validate is slow or runs out of memory when validating a bundle                          | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#923`_ Configuration file parser does not reject incorrect options                              | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#936`_ Validate does not show correct filename for PDF/A failures when validating a directory   | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#822`_ Check for unlabeled files no longer works                                                | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#915`_ context_ref_mismatch does not run except when -R pds4.label                              | |:yellow_circle:| | s.low                     |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#933`_ Missing operation documentation                                                          | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#902`_ Validate error during JPEG content validation                                            | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#919`_ Validate throws an error when UnsignedBitString has 61 bits                              | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                       | I&T Status        | Priority / Bug Severity   |
+=============================================================+===================+===========================+
| `validate#824`_ Check for PDF/A-1a only if Product_Document | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------+-------------------+---------------------------+

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

+------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================+===================+===========================+
| `web-analytics#12`_ Sync script fails silently if aws call fails | |:yellow_circle:| | s.medium                  |
+------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================================================+===================+===========================+
| `web-analytics#24`_ As a user, I want a mission-specific dashboard showing instrument and product type download metrics | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `web-analytics#39`_ update repo with template files                                                                     | |:yellow_circle:| | unknown                   |
+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
.. _pds4-information-model#784: https://github.com/NASA-PDS/pds4-information-model/issues/784
.. _data-upload-manager#51: https://github.com/NASA-PDS/data-upload-manager/issues/51
.. _data-upload-manager#50: https://github.com/NASA-PDS/data-upload-manager/issues/50
.. _data-upload-manager#87: https://github.com/NASA-PDS/data-upload-manager/issues/87
.. _data-upload-manager#116: https://github.com/NASA-PDS/data-upload-manager/issues/116
.. _data-upload-manager#110: https://github.com/NASA-PDS/data-upload-manager/issues/110
.. _data-upload-manager#92: https://github.com/NASA-PDS/data-upload-manager/issues/92
.. _data-upload-manager#98: https://github.com/NASA-PDS/data-upload-manager/issues/98
.. _deep-archive#162: https://github.com/NASA-PDS/deep-archive/issues/162
.. _doi-service#430: https://github.com/NASA-PDS/doi-service/issues/430
.. _harvest#127: https://github.com/NASA-PDS/harvest/issues/127
.. _harvest#158: https://github.com/NASA-PDS/harvest/issues/158
.. _nucleus#101: https://github.com/NASA-PDS/nucleus/issues/101
.. _pds4-information-model#770: https://github.com/NASA-PDS/pds4-information-model/issues/770
.. _pds4-information-model#776: https://github.com/NASA-PDS/pds4-information-model/issues/776
.. _planetary-data-cloud#108: https://github.com/NASA-PDS/planetary-data-cloud/issues/108
.. _registry-pds3-catalog#16: https://github.com/NASA-PDS/registry-pds3-catalog/issues/16
.. _registry-sweepers#112: https://github.com/NASA-PDS/registry-sweepers/issues/112
.. _roundup-action#138: https://github.com/NASA-PDS/roundup-action/issues/138
.. _s3-browser-cloudfront#22: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/22
.. _search-ui-legacy#30: https://github.com/NASA-PDS/search-ui-legacy/issues/30
.. _software-issues-repo#86: https://github.com/NASA-PDS/software-issues-repo/issues/86
.. _software-issues-repo#98: https://github.com/NASA-PDS/software-issues-repo/issues/98
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
.. _validate#823: https://github.com/NASA-PDS/validate/issues/823
.. _validate#826: https://github.com/NASA-PDS/validate/issues/826
.. _validate#923: https://github.com/NASA-PDS/validate/issues/923
.. _validate#936: https://github.com/NASA-PDS/validate/issues/936
.. _validate#822: https://github.com/NASA-PDS/validate/issues/822
.. _validate#915: https://github.com/NASA-PDS/validate/issues/915
.. _validate#933: https://github.com/NASA-PDS/validate/issues/933
.. _validate#902: https://github.com/NASA-PDS/validate/issues/902
.. _validate#919: https://github.com/NASA-PDS/validate/issues/919
.. _validate#824: https://github.com/NASA-PDS/validate/issues/824
.. _web-analytics#30: https://github.com/NASA-PDS/web-analytics/issues/30
.. _web-analytics#32: https://github.com/NASA-PDS/web-analytics/issues/32
.. _web-analytics#12: https://github.com/NASA-PDS/web-analytics/issues/12
.. _web-analytics#24: https://github.com/NASA-PDS/web-analytics/issues/24
.. _web-analytics#39: https://github.com/NASA-PDS/web-analytics/pull/39
.. _Software Release Summary (B15.0): https://nasa-pds.github.io/releases/15.0/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md