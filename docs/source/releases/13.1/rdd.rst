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

No PDS4 Standards Updates

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
|`deep-archive#137`_ Pagination handling does not appear to work properly for pds-deep-registry-archive   ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`deep-archive#134`_ Cannot connect to any PDS API endpoints for pds-deep-archive-registry                ||:yellow_circle:|   |s.high                    |
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
|`doi-service#377`_ DOI Service does not accurately parse <author_list> and <editor_list> in XML labels   ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`doi-service#398`_ Still -- Unable to generate / export json report of DOI metadata                      ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                           |I&T Status          |Priority / Bug Severity   |
+================================================================================================================================+====================+==========================+
|`doi-service#283`_ As a publisher, I want to be notified when a new DOI has been minted or significant update to the metadata   ||:yellow_circle:|   |p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================================+====================+==========================+
|`doi-service#363`_ Enhance weekly reporting to push to ADS SFTP server   ||:yellow_circle:|   |p.must-have               |
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
|`harvest#102`_ Harvest skips path that is the root of a soft link                           ||:yellow_circle:|   |s.high                    |
+--------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`harvest#112`_ --overwrite flag is not respected for <bundles> elements in harvest config   ||:yellow_circle:|   |s.high                    |
+--------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------+--------------------+--------------------------+
|Issue                                                 |I&T Status          |Priority / Bug Severity   |
+======================================================+====================+==========================+
|`harvest#106`_ Improve skipped product INFO message   ||:yellow_circle:|   |p.should-have             |
+------------------------------------------------------+--------------------+--------------------------+

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

+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                               |I&T Status          |Priority / Bug Severity   |
+====================================================================================================+====================+==========================+
|`pds-api#240`_ API Client cannot connect to current deployed API                                    ||:yellow_circle:|   |s.high                    |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#220`_ Past versions are being returned by API, by default                                  ||:yellow_circle:|   |s.high                    |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#200`_ API performance degradation from B12.1 release                                       ||:yellow_circle:|   |s.high                    |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#213`_ Accept header of text/csv returns blank lines                                        ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#215`_ vnd.nasa.pds.pds4+xml format does not return information                             ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#199`_ `hits` appears to be showing the current page count, not the overall number of its   ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#214`_ vnd.nasa.pds.pds4+json format does return information                                ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                        |I&T Status          |Priority / Bug Severity   |
+=============================================================================================================+====================+==========================+
|`pds-api#198`_ As a user, I want query responses for empty results to be clearly documented                  ||:yellow_circle:|   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`pds-api#221`_ As a user, I want to query only the latest versions of products unless explicitly requested   ||:yellow_circle:|   |p.must-have               |
+-------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                   |I&T Status          |Priority / Bug Severity   |
+========================================================================+====================+==========================+
|`pds-api#194`_ Develop NASA/PDS Skin for Search API Swagger interface   ||:yellow_circle:|   |unknown                   |
+------------------------------------------------------------------------+--------------------+--------------------------+

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

+-----------------------------------------------------------------------------+------------------+--------------------------+
|Issue                                                                        |I&T Status        |Priority / Bug Severity   |
+=============================================================================+==================+==========================+
|`pds4-information-model#507`_ Bug generating BepiColombo SERENA dictionary   ||:blue_circle:|   |s.medium                  |
+-----------------------------------------------------------------------------+------------------+--------------------------+
|`pds4-information-model#506`_ hyb2 has incorrect namespace for IM v1.14      ||:blue_circle:|   |s.medium                  |
+-----------------------------------------------------------------------------+------------------+--------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                    |I&T Status          |Priority / Bug Severity   |
+=========================================================================================================================================+====================+==========================+
|`pds4-information-model#473`_ As a user, I want to describe a relationship between an attribute in the model and the column of a table   ||:yellow_circle:|   |p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

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

+----------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                             |I&T Status          |Priority / Bug Severity   |
+==================================================================================+====================+==========================+
|`portal-tasks#47`_ [SECURITY] JQuery upgrade needed to avoid possible injection   ||:yellow_circle:|   |s.high                    |
+----------------------------------------------------------------------------------+--------------------+--------------------------+
|`portal-tasks#54`_ Possible XSS vulnerability on data set view pages              ||:yellow_circle:|   |s.critical                |
+----------------------------------------------------------------------------------+--------------------+--------------------------+
|`portal-tasks#31`_ Data release manager pages missing login session check         ||:yellow_circle:|   |s.medium                  |
+----------------------------------------------------------------------------------+--------------------+--------------------------+

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

+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                          |I&T Status          |Priority / Bug Severity   |
+===============================================================================================================+====================+==========================+
|`registry#150`_ TLS termination listening on wrong port                                                        ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#97`_ registry-manager won't set archive-status on some collections                                   ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#118`_ archive status value was not changed on bundle's contents                                      ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#146`_ OpenSearch service of Registry won't start on Linux                                            ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#136`_ follow on to #118, registry-manager still unable to change archive status on bundle contents   ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry#120`_ Continuous Delivery not working with OpenSearch                                                ||:blue_circle:|     |s.medium                  |
+---------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                     |I&T Status          |Priority / Bug Severity   |
+==========================================================================================+====================+==========================+
|`registry#34`_ Propose a solution for set-archive-status on a docker compose deployment   ||:yellow_circle:|   |p.must-have               |
+------------------------------------------------------------------------------------------+--------------------+--------------------------+

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

+---------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                      |I&T Status          |Priority / Bug Severity   |
+===========================================================================================================================+====================+==========================+
|`registry-api#227`_ Keyword search does not work on registry-api deployed on pds.nasa.gov                                  ||:yellow_circle:|   |s.medium                  |
+---------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#190`_ /all suffix returns a message which I don't understand                                                 ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#224`_ registry-api does not return latest version of product metadata when multiple versions are harvested   ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#202`_ observational end-point returns collections                                                            ||:yellow_circle:|   |s.high                    |
+---------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                      |I&T Status          |Priority / Bug Severity   |
+===========================================================================================================================================+====================+==========================+
|`registry-api#208`_ As a registry-tool/registry-user I want to ensure leading multiple forward-slashes in request paths are stripped out   ||:yellow_circle:|   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`registry-api#212`_ As a user, I want the API to support redundant `/` in the url                                                          ||:yellow_circle:|   |p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

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

+--------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                       |I&T Status          |Priority / Bug Severity   |
+============================================================================================+====================+==========================+
|`registry-harvest-service#25`_ Harvest service sometimes skips collection inventory files   ||:yellow_circle:|   |s.high                    |
+--------------------------------------------------------------------------------------------+--------------------+--------------------------+

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

+-----------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                              |I&T Status          |Priority / Bug Severity   |
+===================================================================================+====================+==========================+
|`roundup-action#96`_ Roundup failing on unstable build                             ||:blue_circle:|     |s.medium                  |
+-----------------------------------------------------------------------------------+--------------------+--------------------------+
|`roundup-action#98`_ git push in roundup action failing w/ remote ahead of local   ||:yellow_circle:|   |s.low                     |
+-----------------------------------------------------------------------------------+--------------------+--------------------------+
|`roundup-action#103`_ unstable build failed                                        ||:yellow_circle:|   |s.medium                  |
+-----------------------------------------------------------------------------------+--------------------+--------------------------+

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
`validate#481`_ B13.1 Content Validation Improvements: Intermingled Headers
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                                                    |I&T Status          |Level         |Priority / Bug Severity   |
+=========================================================================================================+====================+==============+==========================+
|`validate#425`_ Refactor content validation to more robustly handle intermingled Headers                 ||:green_circle:|    |enhancement   |p.must-have               |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|`validate#480`_ Validate does not calculate overlaps correctly when Header is not first object in file   ||:yellow_circle:|   |bug           |s.medium                  |
+---------------------------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


`validate#557`_ Dockerize Validate
++++++++++++++++++++++++++++++++++

+---------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+
|Issue                                                                                  |I&T Status          |Level         |Priority / Bug Severity   |
+=======================================================================================+====================+==============+==========================+
|`validate#556`_ As a user, I want to be able to use validate from a docker container   ||:yellow_circle:|   |requirement   |p.should-have             |
+---------------------------------------------------------------------------------------+--------------------+--------------+--------------------------+


Other Updates
~~~~~~~~~~~~~
Bugs
++++

+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                                                                               |I&T Status          |Priority / Bug Severity   |
+====================================================================================================================================================+====================+==========================+
|`validate#503`_ validate passes confusing message to the command window                                                                             ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#474`_ Validate can't find files in directory specified by <directory_path_name>                                                           ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#529`_  ERROR  [error.array.value_out_of_min_max_range] evaluation is not correct                                                          ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#511`_ Table_Character not accurately checking field formats                                                                               ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#499`_ validate doesn't flag a data file with only LF                                                                                      ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#564`_ Array object validation regression in v3.0.3                                                                                        ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#531`_ ERROR  [error.table.bad_file_read] incorrectly reports that GroupFieldBinary group_length is larger than size of contained fields   ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#576`_ validate does not correctly handle field format checks for hex values                                                               ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#453`_ Validate should not check PDF/A validity if content validation is disabled                                                          ||:green_circle:|    |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#444`_ pds4.bundle option seems to not travel through enough subdirectories                                                                ||:green_circle:|    |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#554`_ --spot-check-data flag throws IOException                                                                                           ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#155`_ Fix uncaught exception error when validating an array object                                                                        ||:yellow_circle:|   |s.low                     |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#473`_ NullPointerException when Table_Delimited is missing records attribute                                                              ||:yellow_circle:|   |s.low                     |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#544`_ validate gives a error.table.bad_field_read error                                                                                   ||:yellow_circle:|   |p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------+--------------------+--------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------------------------------+--------------------+--------------------------+
|Issue                                                                                       |I&T Status          |Priority / Bug Severity   |
+============================================================================================+====================+==========================+
|`validate#537`_ Refactor `getMessageCountBasedOnProblemType` function using introspection   ||:blue_circle:|     |unknown                   |
+--------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#569`_ Improve error message when file is truncated and cannot be read             ||:yellow_circle:|   |p.could-have              |
+--------------------------------------------------------------------------------------------+--------------------+--------------------------+
|`validate#436`_ Improve error messages for overlapping objects in a label                   ||:yellow_circle:|   |p.should-have             |
+--------------------------------------------------------------------------------------------+--------------------+--------------------------+

Liens
=====

+--------+--------+------------+
|Issue   |Title   |Rationale   |
+========+========+============+

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
.. _deep-archive#137: https://github.com/NASA-PDS/deep-archive/issues/137
.. _deep-archive#134: https://github.com/NASA-PDS/deep-archive/issues/134
.. _doi-service#377: https://github.com/NASA-PDS/doi-service/issues/377
.. _doi-service#398: https://github.com/NASA-PDS/doi-service/issues/398
.. _doi-service#283: https://github.com/NASA-PDS/doi-service/issues/283
.. _doi-service#363: https://github.com/NASA-PDS/doi-service/issues/363
.. _doi-ui#130: https://github.com/NASA-PDS/doi-ui/issues/130
.. _doi-ui#167: https://github.com/NASA-PDS/doi-ui/issues/167
.. _harvest#102: https://github.com/NASA-PDS/harvest/issues/102
.. _harvest#112: https://github.com/NASA-PDS/harvest/issues/112
.. _harvest#106: https://github.com/NASA-PDS/harvest/issues/106
.. _pds-api#240: https://github.com/NASA-PDS/pds-api/issues/240
.. _pds-api#220: https://github.com/NASA-PDS/pds-api/issues/220
.. _pds-api#200: https://github.com/NASA-PDS/pds-api/issues/200
.. _pds-api#213: https://github.com/NASA-PDS/pds-api/issues/213
.. _pds-api#215: https://github.com/NASA-PDS/pds-api/issues/215
.. _pds-api#199: https://github.com/NASA-PDS/pds-api/issues/199
.. _pds-api#214: https://github.com/NASA-PDS/pds-api/issues/214
.. _pds-api#198: https://github.com/NASA-PDS/pds-api/issues/198
.. _pds-api#221: https://github.com/NASA-PDS/pds-api/issues/221
.. _pds-api#194: https://github.com/NASA-PDS/pds-api/issues/194
.. _pds4-information-model#507: https://github.com/NASA-PDS/pds4-information-model/issues/507
.. _pds4-information-model#506: https://github.com/NASA-PDS/pds4-information-model/issues/506
.. _pds4-information-model#473: https://github.com/NASA-PDS/pds4-information-model/issues/473
.. _pds4-jparser#57: https://github.com/NASA-PDS/pds4-jparser/issues/57
.. _portal-tasks#47: https://github.com/NASA-PDS/portal-tasks/issues/47
.. _portal-tasks#54: https://github.com/NASA-PDS/portal-tasks/issues/54
.. _portal-tasks#31: https://github.com/NASA-PDS/portal-tasks/issues/31
.. _registry#150: https://github.com/NASA-PDS/registry/issues/150
.. _registry#97: https://github.com/NASA-PDS/registry/issues/97
.. _registry#118: https://github.com/NASA-PDS/registry/issues/118
.. _registry#146: https://github.com/NASA-PDS/registry/issues/146
.. _registry#136: https://github.com/NASA-PDS/registry/issues/136
.. _registry#120: https://github.com/NASA-PDS/registry/issues/120
.. _registry#34: https://github.com/NASA-PDS/registry/issues/34
.. _registry-api#227: https://github.com/NASA-PDS/registry-api/issues/227
.. _registry-api#190: https://github.com/NASA-PDS/registry-api/issues/190
.. _registry-api#224: https://github.com/NASA-PDS/registry-api/issues/224
.. _registry-api#202: https://github.com/NASA-PDS/registry-api/issues/202
.. _registry-api#208: https://github.com/NASA-PDS/registry-api/issues/208
.. _registry-api#212: https://github.com/NASA-PDS/registry-api/issues/212
.. _registry-harvest-service#25: https://github.com/NASA-PDS/registry-harvest-service/issues/25
.. _registry-mgr#57: https://github.com/NASA-PDS/registry-mgr/issues/57
.. _roundup-action#96: https://github.com/NASA-PDS/roundup-action/issues/96
.. _roundup-action#98: https://github.com/NASA-PDS/roundup-action/issues/98
.. _roundup-action#103: https://github.com/NASA-PDS/roundup-action/issues/103
.. _validate#481: https://github.com/NASA-PDS/validate/issues/481
.. _validate#425: https://github.com/NASA-PDS/validate/issues/425
.. _validate#480: https://github.com/NASA-PDS/validate/issues/480
.. _validate#557: https://github.com/NASA-PDS/validate/issues/557
.. _validate#556: https://github.com/NASA-PDS/validate/issues/556
.. _validate#503: https://github.com/NASA-PDS/validate/issues/503
.. _validate#474: https://github.com/NASA-PDS/validate/issues/474
.. _validate#529: https://github.com/NASA-PDS/validate/issues/529
.. _validate#511: https://github.com/NASA-PDS/validate/issues/511
.. _validate#499: https://github.com/NASA-PDS/validate/issues/499
.. _validate#564: https://github.com/NASA-PDS/validate/issues/564
.. _validate#531: https://github.com/NASA-PDS/validate/issues/531
.. _validate#576: https://github.com/NASA-PDS/validate/issues/576
.. _validate#453: https://github.com/NASA-PDS/validate/issues/453
.. _validate#444: https://github.com/NASA-PDS/validate/issues/444
.. _validate#554: https://github.com/NASA-PDS/validate/issues/554
.. _validate#155: https://github.com/NASA-PDS/validate/issues/155
.. _validate#473: https://github.com/NASA-PDS/validate/issues/473
.. _validate#544: https://github.com/NASA-PDS/validate/issues/544
.. _validate#537: https://github.com/NASA-PDS/validate/issues/537
.. _validate#569: https://github.com/NASA-PDS/validate/issues/569
.. _validate#436: https://github.com/NASA-PDS/validate/issues/436
.. _Software Release Summary (B13.1): https://nasa-pds.github.io/releases/13.1/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md
