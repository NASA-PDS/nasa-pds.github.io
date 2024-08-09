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

+-------------------------------+------------------------------------------------------------------------+
| Ref                           | Title                                                                  |
+===============================+========================================================================+
| `pds4-information-model#784`_ | Complete CCB-325 lien implementation for Browse and Ancillary products |
+-------------------------------+------------------------------------------------------------------------+

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
`harvest#131`_ Enhance support for searching lid/lidvid references
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+------------------------------------------------------------------------------------+-------------------+---------+---------------------------+
| Issue                                                                              | I&T Status        | Level   | Priority / Bug Severity   |
+====================================================================================+===================+=========+===========================+
| `harvest#127`_ ref_lid_* fields are not added to the Registry schema prior to load | |:yellow_circle:| | bug     | s.medium                  |
+------------------------------------------------------------------------------------+-------------------+---------+---------------------------+


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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+----------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================+===================+===========================+
| `monitoring#14`_ As a user, I want a daily budget reports sent to my email inbox | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------+-------------------+---------------------------+

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
`pds-api#24`_ [registry] Handle PDS Supplemental Metadata
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#76`_ [pds-api] Improve API Performance
+++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#75`_ [pds-api] B12.0 API Response Improvements
+++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#77`_ [pds-api] PDS4 Product Relationships
++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#79`_ [pds-api] PDS Core Registry
+++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#81`_ [pds-api] B12.0 Improve API query handling
++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#84`_ [pds-api] Initial Google-like Search
++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#111`_ B12.1 Response Format Improvements
+++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#114`_ Improve PDS API Development Workflow and Versioning
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#117`_ [pds-api] B12.1 API Response Improvements
++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#129`_ Prep for API v1.0 Release
++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#180`_ Refactor API Endpoints for Maintainability
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#181`_ Initial PDS Keyword Search Design
++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#230`_ Support latest product search from API
+++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#235`_ Enable Swagger Interface on pds.nasa.gov
+++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#274`_ Initialize a Wrapper API Client
++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`pds-api#284`_ Add downtime notification to top of API documentation
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================================+===================+===========================+
| `pds-api#130`_ pds api not able to search using URL parameters                                    | |:yellow_circle:| | s.low                     |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#251`_ link to registry-api documentation from registry page is incorrect                 | |:blue_circle:|   | s.low                     |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#213`_ Accept header of text/csv returns blank lines                                      | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#216`_ is "bites" a typo for "bytes" or "bits"?                                           | |:blue_circle:|   | s.low                     |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#214`_ vnd.nasa.pds.pds4+json format does return information                              | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#124`_ Changes to API per last tagged release not in SwaggerHub                           | |:blue_circle:|   | s.critical                |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#209`_ clarifications needed for fields reference in documentation                        | |:blue_circle:|   | s.low                     |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#220`_ Past versions are being returned by API, by default                                | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#164`_ version number invalid according to PEP validation in CI                           | |:blue_circle:|   | s.critical                |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#260`_ PDS API documents are unclear wrt quoting in queries                               | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#121`_ Deployed API + Registry does not contain product metadata for pds4+json response   | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#73`_ As a n00b paginator, there might be an off-by-1 error in the `limit` parameter      | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#259`_ API search returns 500 for anything besides simple queries                         | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#155`_ `products/{identifier}` missing properties object in application/json response     | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#257`_ Search API documentation seems outdated?                                           | |:blue_circle:|   | s.medium                  |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#206`_ fix broken link in API docs                                                        | |:blue_circle:|   | s.low                     |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#215`_ vnd.nasa.pds.pds4+xml format does not return information                           | |:green_circle:|  | s.medium                  |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#210`_ wildcards do not work as expected for all fields                                   | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#196`_ Swagger API page does not show the expected deployed API version                   | |:yellow_circle:| | s.low                     |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#240`_ API Client cannot connect to current deployed API                                  | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#262`_ PDS API is not respecting the sort field                                           | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#200`_ API performance degradation from B12.1 release                                     | |:yellow_circle:| | s.high                    |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#199`_ `hits` appears to be showing the current page count, not the overall number of its | |:yellow_circle:| | s.medium                  |
+---------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================================================================+===================+===========================+
| `pds-api#191`_ As a user, I want to get directions whenever I arrive on an API URL                        | |:yellow_circle:| | p.should-have             |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#139`_ As a user, I want to see API stable release specifications                                 | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#198`_ As a user, I want query responses for empty results to be clearly documented               | |:green_circle:|  | p.should-have             |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#225`_ As a user, I want to monitor the availability of the APIs in production                    | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#169`_ As a user, I want to have a PDS Search API user guide                                      | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#51`_ As a developer, I want a continuous deployment of the API available for testing             | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#68`_ As an API user, I want to know in the response how many hits are returned for an API query. | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#67`_ As an API user, I want to access supplemental metadata from Product_Metadata_Supplemental.  | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#175`_ As a user, I want to know how to query observational data only                             | |:yellow_circle:| | p.must-have               |
+-----------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================================================================================+===================+===========================+
| `pds-api#133`_ clarify what `keyword` parameter is for                                                                    | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#194`_ Develop NASA/PDS Skin for Search API Swagger interface                                                     | |:green_circle:|  | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#217`_ Update user guide to use new API endpoints                                                                 | |:blue_circle:|   | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#10`_ Propose an initial server stub based on swagger output                                                      | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#41`_ Manage field preselection in queries                                                                        | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#14`_ Define initial set of intra-discipline (product-level) search scope                                         | |:blue_circle:|   | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#17`_ Define initial structure for response format conventions and parameter definition                           | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#13`_ Deploy PDS API v0 (alpha) on pds-gamma test server                                                          | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#34`_ Deploy PDS API v0 (alpha) for beta testing                                                                  | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#188`_ Upgrade documentation to present version 1.0 of the search API                                             | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#43`_ Implement content negotiation                                                                               | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#6`_ Assign and iterate over applicable API spec sections with API WG                                             | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#47`_ develop a jupyter notebook demo where a user can browse PDS archive from bundle to product data file        | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#49`_ initiate a proposal for the API WG and ENG team                                                             | |:blue_circle:|   | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#183`_ Create a cookbook page on the content negotiation for the PDS Search API                                   | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#52`_ Get investigation area/targets/instruments from external ids                                                | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#202`_ Complete refactoring per API WG discussion on end-point redesign                                           | |:blue_circle:|   | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#40`_ add lexer to registry api                                                                                   | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#108`_ Update API endpoints to use `identifier` instead of `lidvid`                                               | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#136`_ Revise the pds-api README so that it gives a perspective on non search api (e.g. doi) from pds             | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#4`_ Convert PDS API Spec to Open API                                                                             | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#173`_ Replace summary-only=true by limit=0                                                                       | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#154`_ Refactor `meta` section of pds4+json and pds4+xml to use ops namespace                                     | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#145`_ Remove the x-total-count header from the API specification                                                 | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#110`_ Extend application/pds4+json support to all endpoints                                                      | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#31`_ Streamline testing of API server implementation                                                             | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#8`_ Design and elicit requirements for PDS API Spec                                                              | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#189`_ Update README to reflect best practices of other PDS repositories                                          | |:blue_circle:|   | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#5`_ Define collection-level search parameters                                                                    | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#35`_ Initial Federated API implementation                                                                        | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#12`_ Initial Query Syntax Lexer Implementation                                                                   | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#158`_ Improve linkages from Registry App Docs to API Docs                                                        | |:yellow_circle:| | p.must-have               |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#140`_ Merge unnecessary individual repository                                                                    | |:blue_circle:|   | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#1`_ Design initial collection-level search API                                                                   | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#172`_ Create user guide for the search api                                                                       | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#11`_ Identify a framework to generate python api client from a swagger file                                      | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#112`_ As an API client user, I want to consistently and robustly start local servers for development and testing | |:blue_circle:|   | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#137`_ As a user, I want to have a detailed description of the API q parameter syntax                             | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#142`_ flesh out the registry repository                                                                          | |:yellow_circle:| | unknown                   |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds-api#91`_ Disable XML and HTML responses from current registry-api-service implementation                             | |:yellow_circle:| | p.should-have             |
+---------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                            | I&T Status        | Priority / Bug Severity   |
+==================================================================================================================================+===================+===========================+
| `pds4-information-model#776`_ Unable to build LDDs for 1E00                                                                      | |:yellow_circle:| | s.medium                  |
+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#770`_ ERROR 11179 data dictionary class is missing for overwrite                                         | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `pds4-information-model#801`_ Lack of object initialization in the code leads to infinite when trying to run main more than once | |:yellow_circle:| | s.high                    |
+----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+-------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                               | I&T Status        | Priority / Bug Severity   |
+=====================================================================================+===================+===========================+
| `pds4-information-model#794`_ [namespace-registry] add new namespace `vikinglander` | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`planetary-data-engine#2`_ Evaluate SDE, Legacy Registry, and OpenSearch Keyword Search capabilities
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-engine#5`_ Complete Sinequa Useability Analysis
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`planetary-data-engine#7`_ Develop Query Test Suite and Success Criteria
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                             | I&T Status        | Priority / Bug Severity   |
+===================================================================================================================================+===================+===========================+
| `planetary-data-engine#13`_ Commits to the planetary-data-engine repo cannot be merged due to CI/CD build error related to sphinx | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+-----------------------------------------------------------+-------------------+---------------------------+
| Issue                                                     | I&T Status        | Priority / Bug Severity   |
+===========================================================+===================+===========================+
| `portal-tasks#95`_ Broken links for 1.21.0.0 and 1.22.0.0 | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------+-------------------+---------------------------+

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

+----------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                              | I&T Status        | Priority / Bug Severity   |
+====================================================================================================+===================+===========================+
| `registry#292`_ Secret detection is broken on branch titan_treks_utility_script                    | |:yellow_circle:| | s.medium                  |
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
`registry-api#505`_ Multi-tenancy Migration MVP Tasks
+++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                         | I&T Status        | Priority / Bug Severity   |
+===============================================================================+===================+===========================+
| `registry-api#431`_ Investigate sporadic 500 and 504 errors with registry API | |:yellow_circle:| | s.medium                  |
+-------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                                                  | I&T Status        | Priority / Bug Severity   |
+========================================================================================================================================================================================+===================+===========================+
| `registry-api#435`_ As a user, by default, I want to resolve the latest version of a product when given a product logical_identifier (LID) (`/products/{logical_identifier}` endpoint) | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#469`_ As a user, I want to filter the products by any available PDS4 property using a combination of comparison, logical, and precedence grouping operators              | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#485`_ As a user, by default, I want to search for only the latest versions of all products on the `/products/{identifier}/members/members` endpoint                      | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#434`_ As a user, I want to get a product description given a lidvid                                                                                                      | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#497`_ As a user, I want to receive metadata only in the API responses (no binary blobs)                                                                                  | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#511`_ As a user, I want to get all the products for a specific PDS4 product class                                                                                        | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#484`_ As a user, by default, I want to search for only the latest versions of all products on the `/products/{identifier}/members` endpoint                              | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#516`_ As a user, I want to get a description of the API when I request it from its base URL in a web browser                                                             | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#494`_ As a user, I want to filter the products by any available PDS4 property using comparison operators                                                                 | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#488`_ As a user, by default, I want to search for the latest versions of all products on the `/classes/{class}` endpoint unless explicitly requested                     | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#486`_ As a user, by default, I want to search for only the latest versions of all products on the `/products/{identifier}/member-of` endpoint                            | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#487`_ As a user, by default, I want to search only for the latest versions of all products on the `/products/{identifier}/member-of/member-of` endpoint                  | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-api#436`_ As a user, I want to get all product versions associated to one lid                                                                                                | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

--------

Registry-client
---------------
*A simple PDS Registry Client which authenticates users with PDS SSO and signs requests to the serverless OpenSearch (AOSS) hosting the Registry database.*

.. list-table:: 
   :widths: 15 15 15 15 15 15

   * - `User Guide <https://github.com/NASA-PDS/registry-client#readme>`_
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

+-----------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================+===================+===========================+
| `registry-common#50`_ Update registry-common library to support change to AWS interface | |:yellow_circle:| | s.critical                |
+-----------------------------------------------------------------------------------------+-------------------+---------------------------+
| `registry-common#53`_ Update OpenSearch API call to use `search()` instead of `get()`   | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------+-------------------+---------------------------+

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
Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================================================+===================+===========================+
| `registry-legacy-solr#93`_ As a user, I want to provide search/access links using the hsk.cat files within the data set | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================================================+===================+===========================+
| `roundup-action#138`_ Maven deploy no longer works due to Maven central upgrade                                         | |:yellow_circle:| | s.high                    |
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
No planned updates realized for this build in this repository.

Other Updates
~~~~~~~~~~~~~
Requirements
++++++++++++

+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                   | I&T Status        | Priority / Bug Severity   |
+=========================================================================================================================+===================+===========================+
| `s3-browser-cloudfront#22`_ As a data user, I want to view ODR S3 bucket with S3 browser app                            | |:yellow_circle:| | p.must-have               |
+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `s3-browser-cloudfront#68`_ As a manager, I want the S3-browser to be deployable and accessible from a '/some_path' URL | |:yellow_circle:| | p.should-have             |
+-------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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
`validate#249`_ Improvements for validating accumulating bundles / collections
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#250`_ Improvements to meet updated Standards Reference since initial requirements implementation
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#317`_ B12.0 Referential Integrity Improvements
++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#318`_ B12.0 Content Validation Improvements
+++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#409`_ B12.1 PDF/A Handling Improvements
+++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#414`_ Referential Integrity Checking with the Registry+API
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#426`_ B12.1 Content Validation Improvements
+++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#481`_ B13.1 Content Validation Improvements: Intermingled Headers
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#496`_ Support new lblx file extension
+++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#498`_ Improve Content Validation Performance through Spot Checking
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#534`_ B14.0 Content Validation Improvements: Additional Table Types, Additional File Areas
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#557`_ Dockerize Validate
++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#578`_ B13.1 Fix Must-Have Priority Bugs
+++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#606`_ Support for Encoded Video and Encoded Audio
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#607`_ Support for Improved Datetime Checks
++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#610`_ B14.0 Enhancements to Initial Version of Registry Referential Integrity Validator
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#629`_ Add Check for Schematron/Schema Version Mismatch
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#695`_ Update Validate Test Suite to Support Larger Data Sets
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#816`_ As a user, I want a WARNING to be thrown when a delimited or character table value does not match the expected `field_format`
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#817`_ As a user, I want an ERROR to be thrown when a character table value does not match the expected `validation_format`
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#822`_ Check for unlabeled files no longer works
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#823`_ Validate V.3.4.1 reports file read errors on products which read correctly under V.3.2.0
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#824`_ Check for PDF/A-1a only if Product_Document
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#826`_ validate is slow or runs out of memory when validating a bundle
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#831`_ validate incorrectly handles special constant high_instrument_saturation
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

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


`validate#833`_ Fix Performance and Content Validation Regressions
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+----------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                    | I&T Status        | Level       | Priority / Bug Severity   |
+==========================================================================================================+===================+=============+===========================+
| `validate#822`_ Check for unlabeled files no longer works                                                | |:yellow_circle:| | bug         | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#823`_ Validate V.3.4.1 reports file read errors on products which read correctly under V.3.2.0 | |:yellow_circle:| | bug         | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#824`_ Check for PDF/A-1a only if Product_Document                                              | |:yellow_circle:| | enhancement | p.should-have             |
+----------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#826`_ validate is slow or runs out of memory when validating a bundle                          | |:yellow_circle:| | bug         | s.medium                  |
+----------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`validate#837`_ In text tables, validate attempts to match pattern associated with `data_type` before checking `Special_Constants`
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#849`_ Validate stalls when validating collection inventory file with duplicates records
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#857`_ As a user, I want to receive a WARNING message when the `Observing_System_Component.name` does not match the value in the context product
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#860`_ Add Warning Messages for Context Product Name Mismatches
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

+-----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| Issue                                                                                                                                                     | I&T Status        | Level       | Priority / Bug Severity   |
+===========================================================================================================================================================+===================+=============+===========================+
| `validate#857`_ As a user, I want to receive a WARNING message when the `Observing_System_Component.name` does not match the value in the context product | |:yellow_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+
| `validate#861`_ As a user, I want to receive a WARNING message when the `Target_Identification.name` does not match the value in the context product      | |:yellow_circle:| | requirement | p.should-have             |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+-------------+---------------------------+


`validate#861`_ As a user, I want to receive a WARNING message when the `Target_Identification.name` does not match the value in the context product
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#873`_ Validate 3.5.0-snapshot Giving Unexpected Errors for Matching Filenames in Separate Directories
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#874`_ SXXP0003 Error when running on PDS3 data sets for v3.3.3 or v3.4.1
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#880`_ Validate failing products that contain "collection" not in the beginning of filename
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#902`_ Validate error during JPEG content validation
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#903`_ Validate not retrying on sch load failure
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#905`_ Validate 3.5.0-snapshot gives error when encountering Document objects/files used in other Document products.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#915`_ `context_ref_mismatch` check only executes when -R pds4.label
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#919`_ Validate throws an error when UnsignedBitString has 61 bits
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#923`_ Configuration file parser does not reject incorrect options 
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#933`_ Missing operation documentation
+++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#936`_ Validate does not show correct filename for PDF/A failures when validating a directory
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

`validate#949`_ Validate does not appear to validate against the latest versions of context products 
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
    No requirements, enhancements, or bug fixes tickets identified for this theme in the current build. Click on the
    link in this section title for details.

Other Updates
~~~~~~~~~~~~~
Bugs
++++

+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                           | I&T Status        | Priority / Bug Severity   |
+=================================================================================================================================================================+===================+===========================+
| `validate#178`_ Improve performance when content validation is disabled                                                                                         | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#327`_ validate fails to process large data file                                                                                                       | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#294`_ Content validation incorrectly reports error for floating-point values out of specified min/max range                                           | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#754`_ Validate 3.3.0 erroneously reports data objects out of offset order                                                                             | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#401`_ validate does not flag <CR> within lid_reference                                                                                                | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#209`_ Packed_Data_Fields and bit fields do not validate as expected                                                                                   | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#473`_ NullPointerException when Table_Delimited is missing records attribute                                                                          | |:green_circle:|  | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#593`_ Regression in validate no longer enabling CRLF to be embedded within a Table_Character record                                                   | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#516`_ validate embedded in an app bundled as a fat-jar raise exception on product validation                                                          | |:blue_circle:|   | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#439`_ Incorrect Warning for Missing document_standard_id is Stream_Text                                                                               | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#690`_ Validate does not accurately check for missing_constant values                                                                                  | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#854`_ validate 3.5.0-SNAPSHOT attempts to look at all files, not just *.xml                                                                           | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#364`_ validate does not allow ".XML" as an extension for a label file                                                                                 | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#2`_ Suppress INFO messages related to initial fix for JAXB vulnerability                                                                              | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#298`_ validate misses double quotes within a delimited table                                                                                          | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#761`_ Validate gives errors for 'NaN' values in IEEE754 data                                                                                          | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#419`_ validate 2.2.0-SNAPSHOT warns about a pretty benign bundle + readme.txt                                                                         | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#469`_ Validate content validation does not handle properly special_constants and field_statistics when they both appear                               | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#781`_ Validate making incorrect assumption that first object has and object length == `file_size`                                                     | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#334`_ validate 2.1.0 snapshot fails on a label with 2 table_character                                                                                 | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#71`_ Unable to use catalog file after update to always force remote schemas                                                                           | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#723`_ Installation instructions need updates for Windows                                                                                              | |:green_circle:|  | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#431`_ warning.table.characters_between_fields missing for last record in table                                                                        | |:green_circle:|  | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#464`_ Validate is reporting an "Uncaught exception while validating" error on Windows                                                                 | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#739`_ Intermittent network failures attempting repeated downloads of schemas/schematrons                                                              | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#435`_ Array Content Validator is not accepting values at the min/max due to false precision                                                           | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#748`_ Buffer limit IOException thrown with validate-refs                                                                                              | |:blue_circle:|   | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#183`_ Memory leak issue has returned after Saxon downgrade                                                                                            | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#153`_ Update validate to throw error when a file has a space in the filename                                                                          | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#411`_ Validate repo cannot be checked out on Windows without errors                                                                                   | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#326`_ File-size check fails for large data files                                                                                                      | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#561`_ Validate incorrectly enforces file naming requirements on bundles/collections                                                                   | |:green_circle:|  | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#519`_ Validate should throw record length error when record delimiter does not occur in correct location                                              | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#441`_ Validate is reporting a 'String index out of range' error for a text file                                                                       | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#461`_ [SECURITY] Patch log4j library                                                                                                                  | |:yellow_circle:| | s.critical                |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#507`_ validate having issues checking some file content on windows                                                                                    | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#514`_ Validate does not catch NaNs in Binary Tables                                                                                                   | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#300`_ validate -u flag reports an error on Windows                                                                                                    | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#297`_ Content validation of ASCII_Integer field does not accept value with leading zeroes                                                             | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#155`_ Fix uncaught exception error when validating an array object                                                                                    | |:green_circle:|  | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#335`_ validate gives a NullPointerException during validation of a directory containing Table_Character products                                      | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#597`_ Validate does not maintain history of other versions it comes across as it traverses directories causing erroneous WARNING messages             | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#356`_ validate labels error.sub_directory.unallowed_name as a warning                                                                                 | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#214`_ validate outputs an extra '.'                                                                                                                   | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#173`_ Bug with #149 fix: Product counter is invalid and does not reset after each collection                                                          | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#479`_ validate erroneously flags PDF/A-1a compliant file                                                                                              | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#6`_ Improve pds4.bundle unlabeled files check to handle files without a file suffix                                                                   | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#145`_ Incorrect help information for --spot-check-data flag                                                                                           | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#234`_ Validate gives incorrect records mismatch WARNING for interleaved data objects                                                                  | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#52`_ Incorrect package declarations under gov.nasa.tools.web.ui                                                                                       | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#611`_ Missing validation of valid_maximum and valid_minimum from Special_Constants                                                                    | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#747`_ validate flags IEEE 754 "infinity" values as invalid                                                                                            | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#427`_ validate does not work correct when path name contains a space on mac                                                                           | |:green_circle:|  | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#144`_ Fix string == comparison issues per vulnerability scan                                                                                          | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#372`_ Issues with logic for reading latest version of collections, and file read logging lost with v2.* of validate                                   | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#63`_ Validate Table_Character groups and their specified lengths match the specified group_length                                                     | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#554`_ --spot-check-data flag throws IOException                                                                                                       | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#529`_  ERROR  [error.array.value_out_of_min_max_range] evaluation is not correct                                                                      | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#531`_ ERROR  [error.table.bad_file_read] incorrectly reports that GroupFieldBinary group_length is larger than size of contained fields               | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#750`_ Validate-refs with manifest of file paths does not seem to read the files correctly                                                             | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#844`_ Exception when trying to handle `missing_constant` == `Infinity`                                                                                | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#551`_ Validate fails regression test on issue 188                                                                                                     | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#72`_ Catalog file flag expects a List of files requiring it not be the last argument                                                                  | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#649`_ validate does not validate a collection if collection.xml pointed to                                                                            | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#499`_ validate doesn't flag a data file with only LF                                                                                                  | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#408`_ Validate 2.1.0-SNAPSHOT skips a collection XML label                                                                                            | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#328`_ validate bundle incorrectly reports "not a member of any collection" that it passed before                                                      | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#167`_ Content validation multi-threading issue                                                                                                        | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#273`_ Bug performing bundle validation with nested directories                                                                                        | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#545`_ Validate 2.4.0/3.0.0 fail with NPE/internal error on certain test cases                                                                         | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#299`_ Validate tool does not PASS a bundle with a single-character filename                                                                           | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#375`_ validate halts if label has name "collection" embedded                                                                                          | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#203`_ Assembly plugin non-fatal errors on Windows                                                                                                     | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#240`_ Unexpected error for data collection in a sub-directory                                                                                         | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#511`_ Table_Character not accurately checking field formats                                                                                           | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#139`_ Revisit PDS-605: L5.PRP.VA.36: Check that the LID for a product has the LID of its parent collection product as its base                        | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#11`_ Update allowable field_format values per Standards Reference definition regarding [+-] characters                                                | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#681`_ Validate incorrectly throws precision mismatch error for Table_Delimited                                                                        | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#562`_ Validate incorrectly enforces file naming requirements for base file names ending in a period, underscore, or hyphen                            | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#345`_ validate incorrectly flags integers bounded by "" in a .csv                                                                                     | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#146`_ Update parent LID integrity checking to fix bug introduced for collection integrity checking                                                    | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#644`_ Validate gives errors for 'NaN' and 'Inf' values in IEEE754 data                                                                                | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#257`_ Product with incorrect table binary definition pass validation                                                                                  | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#325`_ Validate Incorrectly Throws Error When Embedded Field_Character Contains <CR><LF>                                                               | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#9`_ Update content validation to fail when the value of an ASCII_Integer is all spaces                                                                | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#271`_ validate 1.25.0-SNAPSHOT raises an exception when validating a product                                                                          | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#763`_ Validate.bat does not execute on Windows                                                                                                        | |:green_circle:|  | s.critical                |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#657`_ validate incorrectly SKIPs label                                                                                                                | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#368`_ Product referential integrity check throws invalid WARNINGs                                                                                     | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#175`_ Fix schematron parsing bug introduced during performance improvements                                                                           | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#361`_ validate does not check Header of a File_Area_Ancillary nor does not provide a meaningful error message for an incorrect Table_Character offset | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#564`_ Array object validation regression in v3.0.3                                                                                                    | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#336`_ validate2.0.3 throws unexpected JavaExceptions, and after fix, it hangs when trying bundle validation                                           | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#180`_ Fix multi-threading bug where reporting finishes prior to threads completing execution                                                          | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#190`_ Validation fails to catch real value in ASCII_NonNegative_Integer field (Table_Delimited)                                                       | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#291`_ When validating a product with a bad schematron definition, bundle validation also fails indicating the associated product does not exist       | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#378`_ validate raises an unexpected error with doi attribute in the Citation_information class                                                        | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#474`_ Validate can't find files in directory specified by <directory_path_name>                                                                       | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#453`_ Validate should not check PDF/A validity if content validation is disabled                                                                      | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#684`_ Validation failures are contingent on presence of `<file_size>` attribute in `<File>` class                                                     | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#673`_ Validate does not handle Special_Constants valid_minimum and valid_maximum in accordance with information model                                 | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#189`_ Validate error reading tables > 2GiB                                                                                                            | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#165`_ Spot check bug throws internal_error when record number is multiple of spot check number                                                        | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#74`_ Validate execution script throws arguments error with v1.15.1                                                                                    | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#8`_ Large Data File Uncaught Exception Error                                                                                                          | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#170`_ Update validate to allow for empty fields in delimited tables                                                                                   | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#349`_ validate allows absolute path in directory_path_name but shouldn't                                                                              | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#333`_ validate -u exits badly                                                                                                                         | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#381`_ validate does not work correctly when the path name contains a space                                                                            | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#62`_ Context validation needs to be updated to include all possible product type use cases                                                            | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#379`_ FileService:printStackTraceToFile:ERROR when validating a product with overlapping fields                                                       | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#550`_ Validate partially fails regression test on issue 388                                                                                           | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#392`_ Validate throws incorrect overlap error when first Field_Bit has length 1                                                                       | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#674`_ validate does not handle special constants with data type of SignedLSB2                                                                         | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#220`_ Incorrect validation of number of records                                                                                                       | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#360`_ validate does not parse colon in Windows path                                                                                                   | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#631`_ Expected value in validate report for context reference name is not same as value in the context file                                           | |:green_circle:|  | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#424`_ Validate does not allow SIP tab file to have lines of differing lengths                                                                         | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#5`_ Improve file base name check according to Standards Reference                                                                                     | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#652`_ validate 3.3.0 snapshot produces incorrect SKIP/INFO messages                                                                                   | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#33`_ Validation succeeds despite throwing exception                                                                                                   | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#84`_ Update Validate to allow specification of schema/schematrons in config file                                                                      | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#614`_ invalid_object_definition occurs upon out-of-order data objects                                                                                 | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#55`_ Content validation does not work properly                                                                                                        | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#206`_ Validate incorrectly fails ASCII_Integer field that is space-padded (empty) in Table_Character                                                  | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#809`_ Validate fails to read files on Windows systems after Internal Reference check updates (#308)                                                   | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#204`_ Build and unit tests do not pass on Windows OS                                                                                                  | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#281`_ Validate fails to report error in   File.file_size                                                                                              | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#533`_ Bug in validate when reading products with a number of records > 4-byte range                                                                   | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#416`_ validate 2.1.0 indicates the table offset is not correct when validating a binary table inside a FITS                                           | |:yellow_circle:| | s.critical                |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#301`_ unclear error message for field count matching                                                                                                  | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#423`_ Validate does not allow a single-character subdirectory                                                                                         | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#380`_ stack trace being created during successful validate execution                                                                                  | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#310`_ Validate missing collections in bundle after CCB-282 updates                                                                                    | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#37`_ JAVA Path does not handle whitespaces in MAC as it used to                                                                                       | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#357`_ Validate allows CRLF within a Table_Delimited field                                                                                             | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#376`_ Checksums output lowercase and do not accept uppercase checksums                                                                                | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#160`_ Remove erroneous timing messages from log output                                                                                                | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#260`_ Missing documentation about deprecated flags                                                                                                    | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#616`_ validate does not correctly validate byte offsets to data objects                                                                               | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#256`_ validate should only do integrity checking on latest version of a collection when referenced by LID                                             | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#698`_ Investigate and Fix code scanning alert for potential improvements                                                                              | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#480`_ Validate does not calculate overlaps correctly when Header is not first object in file                                                          | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#429`_ validate warns "document standard id ... is not correct" on good labels                                                                         | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#201`_ Schematron doesn't fire if <?xml-model ...> has an extra space at the end                                                                       | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#137`_ Update delimited table handling to allow for empty fields                                                                                       | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#366`_ validate should not check if file is PDF/A if --skip-content-validation is enabled                                                              | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#679`_ Validate throws internal error when coming across non-label XML in a target directory                                                           | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#432`_ Requirement #308 does not appear to be working for checking referential integrity from products to others in the bundle                         | |:green_circle:|  | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#760`_ Uncaught exception thrown when only 1 of schemas/schematrons are provided via command-line                                                      | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#548`_ Validate fails regression test on issue 303                                                                                                     | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#337`_ Validate fails with Java Error                                                                                                                  | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#693`_ Upgrade verapdf dependency per transitive log4j vulnerability                                                                                   | |:yellow_circle:| | s.critical                |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#620`_ verbosity flag does not appear to output INFO messages                                                                                          | |:blue_circle:|   | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#671`_ Unexpected SKIP Message for bundle product when using validate-3.3.0-SNAPSHOT                                                                   | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#219`_ validate v1.22.3 has large performance degradation on products with many tables                                                                 | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#447`_ Validate does not correctly pass PDF/A files that are in a subdirectory                                                                         | |:yellow_circle:| | s.high                    |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#3`_ JAXB warning message with Java 9+                                                                                                                 | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#107`_ Registered context product resource lists only one of multiple instrument or target multiple types                                              | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#243`_ validate 1.24.0-SNAPSHOT chokes on a probably good file                                                                                         | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#475`_ Validate crashes on invalid # of records, and spurious file left behind                                                                         | |:green_circle:|  | p.wont-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#470`_ Fix validate compilation issues due to removal of veraPDF artifacts from maven central                                                          | |:yellow_circle:| | s.critical                |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#99`_ Fix bug introduce by --skip-context-validation feature                                                                                           | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#444`_ pds4.bundle option seems to not travel through enough subdirectories                                                                            | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#576`_ validate does not correctly handle field format checks for hex values                                                                           | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#457`_ validate flags .ASC extension as invalid but offers not expected suffices                                                                       | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#785`_ validate catches valid_maximum but not valid_minimum                                                                                            | |:green_circle:|  | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#118`_ Update Validate error/warning counts per ATM regression testing                                                                                 | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#503`_ validate passes confusing message to the command window                                                                                         | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#278`_ Registered context products file does not retain older versions of context products                                                             | |:yellow_circle:| | s.medium                  |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#177`_ Software raises a field_value_overlap error on Table_Binary Packed data fields                                                                  | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#34`_ Add missing core.properties dependency                                                                                                           | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#544`_ validate gives a error.table.bad_field_read error                                                                                               | |:green_circle:|  | p.must-have               |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#344`_ validate inexplicably writes to validate_stack_traces.log                                                                                       | |:yellow_circle:| | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#233`_ Product validation does not detect the number of table records correctly for Table + Array object                                               | |:yellow_circle:| | unknown                   |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#500`_ Validate does not allow `.arch_h` file name/data type                                                                                           | |:green_circle:|  | s.low                     |
+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Requirements
++++++++++++

+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                                                    | I&T Status        | Priority / Bug Severity   |
+==========================================================================================================================================================+===================+===========================+
| `validate#212`_ As a user, I want to validate all data types possible per the PDS4 Information Model                                                     | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#773`_ As a user, I want validate with the registry when a file is being referenced by more than one label                                      | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#1`_ As a user, I want to execute content validation against every nth file                                                                     | |:green_circle:|  | p.could-have              |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#462`_ As a user, I want validate to throw an error when a collection inventory contains an invalid secondary product reference                 | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#605`_ As a user, I want to validate MP4/H.264/AAC encoded video with audio as observational data                                               | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#663`_ As a user, I want to validate M4A/AAC encoded audio as observational data                                                                | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#741`_ As a user, I want validate's referential integrity tool to read a manifest of files and check referential integrity                      | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#596`_ As a user, I want to validate all products referenced from a collection exist within the archive                                         | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#662`_ As a user, I want to validate WAV encoded audio as observational data                                                                    | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#210`_ As a user, I want validate to raise a WARNING when differing versions of IM are used within a bundle                                     | |:yellow_circle:| | p.could-have              |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#415`_ As a user, I want to validate all internal references to products in the PDS archive are valid                                           | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#50`_ Add new target-manifest flag for user to provide a manifest (file) of file/directory paths to validate                                    | |:yellow_circle:| | unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#63`_ Validate Table_Character groups and their specified lengths match the specified group_length                                              | |:yellow_circle:| | unknown                   |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#797`_ As a user, I want to have the same information available in the validation report no matter which style I choose                         | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#316`_ As a user, I want to validate all internal references from one product to another exist within the archive                               | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#827`_ As a user, I want to have the parameter names used in 3.5.0 reports to be the same as they were in ≤3.4.1                                | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#164`_ As a user, I want to validate PDF files are PDF/A                                                                                        | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#343`_ As a user I want to see the name of a table/array in errors, if one is specified                                                         | |:green_circle:|  | p.could-have              |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#556`_ As a user, I want to be able to use validate from a docker container                                                                     | |:green_circle:|  | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#524`_ As a user, I want to receive an error when no products are found within the validation target                                            | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#658`_ As a user, I want the PDF error reports to be output in a user-specified directory                                                       | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#755`_ As a user, I want validate to throw an error when a file is being referenced by more than one label                                      | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#535`_ As a user, I want to receive a warning if records in file are greater than records value specified in label                              | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#367`_ As a user, I want to validate all files referenced by a Product_Document                                                                 | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#599`_ As a user, I want to be able to use both online and local schema/schematron files.                                                       | |:yellow_circle:| | p.could-have              |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#57`_ As a user, I want to be warned when there are alphanumeric characters between fields in Table_Character                                   | |:yellow_circle:| | p.could-have              |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#476`_ As a user, I want to check that are no duplicate LIDs/LIDVIDs in a File_Area_Inventory                                                   | |:green_circle:|  | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#308`_ As a user, I want to check that all Internal References are valid references to other PDS4 products within the current validating bundle | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#388`_ Improve PDF/A validation to include more robust reporting on failures                                                                    | |:yellow_circle:| | p.could-have              |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#188`_ As a user, I want to validate a bundle that uses multiple versions of the Information Model / Discipline LDDs                            | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#241`_ As a developer, I want an API method enable specifying of non-registered context products                                                | |:blue_circle:|   | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#15`_ Verify that all name/type attribute values correspond to names denoted context products                                                   | |:yellow_circle:| | p.could-have              |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#149`_ As a user, I want validate to check number of records/fields specified in label matches the records in the actual data table             | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#604`_ As a user, I want to validate MP4/H.264 encoded video as observational data                                                              | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#617`_ As a user, I would like to enforce browse file extension with encoding type                                                              | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#595`_ As a user, I want to validate all collections referenced from a bundle exist within the archive                                          | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#683`_ As a user, I want to receive a WARNING when table objects are out of order                                                               | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#217`_ As a user, I want to validate content for all possible PDS4 table types                                                                  | |:green_circle:|  | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#482`_ As a user, I want to validate labels/bundles/collections using the LBLX file extension                                                   | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#292`_ CCB-264: Make the Line Feed (LF) character an allowed record delimiter                                                                   | |:yellow_circle:| | p.must-have               |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#303`_ As a user, I want to the raise a WARNING if the object-defined size in the label does not match the file_size value                      | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#628`_ As a user, I want to throw a WARNING when a product's schematron version does not match the schema version                               | |:green_circle:|  | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#651`_ As a user, I want to support bit patterns within Special_Constants values                                                                | |:yellow_circle:| | p.should-have             |
+----------------------------------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

Enhancements
++++++++++++

+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| Issue                                                                                                                          | I&T Status        | Priority / Bug Severity   |
+================================================================================================================================+===================+===========================+
| `validate#41`_ Perform benchmarking on validate to enable documenting of system requirements                                   | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#23`_ Deprecate -f and -m flags                                                                                       | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#358`_ Improve validate performance by removing unnecessary file IO                                                   | |:blue_circle:|   | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#17`_ Validate schematron references and throw fatal error if invalid URI specified                                   | |:yellow_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#21`_ Update pom and readme to reference public docs                                                                  | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#26`_ Update build per pds4-tools rename and open source                                                              | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#412`_ Update PDF validation to check against flavour specified in PDF metadata                                       | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#29`_ Improve pds4.bundle validation performance                                                                      | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#246`_ Add output directory flag to validate-bundle tool                                                              | |:yellow_circle:| | p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#24`_ Update context check to retrieve and use latest context products from EN Registry                               | |:yellow_circle:| | p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#436`_ Improve error messages for overlapping objects in a label                                                      | |:green_circle:|  | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#707`_ Upgrade to Saxon 12.x                                                                                          | |:blue_circle:|   | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#19`_ Remove references to PDS Maven Repo and update packages to build without it                                     | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#230`_ Update validate per SR requirements for collection inventories                                                 | |:yellow_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#187`_ Update documentation to include more details about how/where to file bug reports                               | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#254`_ validate does not perform expediently when doing bundle-level validation against large bundles                 | |:yellow_circle:| | p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#28`_ Add capability for user to input JSON file with additional context products                                     | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#90`_ Update context checks to include data_to_investigation                                                          | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#434`_ Scaled value min/max error does not display scaled value                                                       | |:blue_circle:|   | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#197`_ Change behaviour for printing of "dots" to show progress                                                       | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#290`_ Migrate subset of existing regression tests to cucumber behavioral testing                                     | |:yellow_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#135`_ Update config to include telescopes and facilities telescopes and facilities                                   | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#30`_ Enhance content validation to decrease validation time to <=50% of current benchmark                            | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#322`_ Update installation documentation to require Java 1.9+                                                         | |:yellow_circle:| | p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#158`_ Update POM to use PDS Parent POM                                                                               | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#51`_ Provide the capability to specify multiple locations for pds4.bundle validation                                 | |:yellow_circle:| | p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#421`_ Improve warning message for missing_context_reference                                                          | |:blue_circle:|   | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#608`_ Update datetime regex for content validation                                                                   | |:yellow_circle:| | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#425`_ Refactor content validation to more robustly handle intermingled Headers                                       | |:green_circle:|  | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#20`_ Improve documentation about usage of flags in config file with latest flags                                     | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#43`_ Document multi-threaded architecture for maximized performance                                                  | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#65`_ Update Maven docs to refer to Github release assets                                                             | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#537`_ Refactor `getMessageCountBasedOnProblemType` function using introspection                                      | |:blue_circle:|   | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#31`_ Prepare repository for Maven Central deployment                                                                 | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#132`_ Add validated product counter to pass/fail reporting and end summary                                           | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#238`_ validate does not perform full bundle validation when using a specific bundle.xml                              | |:yellow_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#569`_ Improve error message when file is truncated and cannot be read                                                | |:green_circle:|  | p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#124`_ L5.PRP.VA.42	The tool shall average less than 1 second execution time when content validation is disabled.     | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#215`_ Throw warning when data exists after number of records                                                         | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#7`_ Update to support ComplexLSB8 data types and investigate Floating point exception                                | |:green_circle:|  | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#182`_ Upgrade to Saxon 9.9.1-7 to fix Schematron bug                                                                 | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#643`_ Document how to use validate-refs tool in Validate Operation User Guide                                        | |:green_circle:|  | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#567`_ Update ArrayObject exceptions to enable improved error messaging                                               | |:blue_circle:|   | p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#601`_ Create command-line script to wrap the new registry referential integrity checker                              | |:blue_circle:|   | p.must-have               |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#128`_ Develop validate-bundle script for Validation performance improvements using parallelization approach          | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#355`_ Improve validate reporting when trying to read a null row                                                      | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#194`_ Update validate-bundle to include report filepath flag                                                         | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#64`_ Complete engineering point build 1.15.1                                                                         | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#323`_ Upgrade to Java 9+                                                                                             | |:yellow_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#222`_ Reduce error messages for overlapping fields                                                                   | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#373`_ Update pds4 version mismatch warning message and problem type                                                  | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#47`_ Add flag to temporarily disable context validation                                                              | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#81`_ Validate and throw error when duplicate LIDs are found in Bundle                                                | |:yellow_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#374`_ Refactor PDF/A check handling to match with similar product checks                                             | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#56`_ Validate that Table_Character/Table_Binary fields match the field length definitions in the label               | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#264`_ Update installation documentation to include 64-bit Java as system requirement                                 | |:yellow_circle:| | p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#39`_ Investigate and fix memory leak causing validate crash on large bundles                                         | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#133`_ Deprecate --no-data-check to --skip-content-validation to fall in line with other argument naming              | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#708`_ Update inefficient regexes to potentially improve performance                                                  | |:yellow_circle:| | p.could-have              |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#42`_ Add capability to pds4.bundle validation to ignore product-level validation                                     | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#680`_ validate does not correctly diagnose errors in the record_length value for fixed width Table_Character objects | |:yellow_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#195`_ Improve installation procedure                                                                                 | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#377`_ Update rule documentation to remove "auto-detect" mention                                                      | |:blue_circle:|   | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#87`_ Update validate to apply catalog file and local schemas to discipline schema resolution                         | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#252`_ Implement initial behavioral testing framework with cucumber                                                   | |:yellow_circle:| | p.should-have             |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+
| `validate#50`_ Add new target-manifest flag for user to provide a manifest (file) of file/directory paths to validate          | |:yellow_circle:| | unknown                   |
+--------------------------------------------------------------------------------------------------------------------------------+-------------------+---------------------------+

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

+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Issue                                                                                                             | Title                                                                                                 | Rationale                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+===================================================================================================================+=======================================================================================================+=====================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================================+
| pds-swg_26_ [CR] Defer Registry/API new requirements, Add Performance Improvement Tasks                           | [CR] Defer Registry/API new requirements, Add Performance Improvement Tasks                           | Increased scope of NASA-PDS/registry#185 to use Cognito for multi-tenant OpenSearch requires developer needed for other tasks   NASA-PDS/registry-sweepers#92 was necessary in order to decrease cost and improve scalability of registry sweepers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_25_ [CR] Defer Nucleus / Cloud Tasks from Release Plan                                                    | [CR] Defer Nucleus / Cloud Tasks from Release Plan                                                    | Issues with NGAP and MCP access and policy definitions. Additionally, working to establish more refined OpenSearch deployment architecture for moving to multi-tenancy.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_24_ [CR] Defer Registry and Admin tasks from Release Plan                                                 | [CR] Defer Registry and Admin tasks from Release Plan                                                 | Registry enhancements delayed due to https://github.com/NASA-PDS/registry/issues/178.    JIRA migration delayed due to additional timeline available and lack of resources to focus on the task.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_22_ [CR] Defer Registry+API Tasks                                                                         | [CR] Defer Registry+API Tasks                                                                         | Numerous bugs arose from initial rollout of Registry Workshop and increased usage over the past 6 months that required more effort than expected. https://github.com/NASA-PDS/registry-api/issues/257    [registry#85](https://github.com/NASA-PDS/registry/issues/85) was missed on the roadmap and in our schedule.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_21_ [CR] Defer Validate Content Validation Improvements                                                   | [CR] Defer Validate Content Validation Improvements                                                   | Numerous bug fixes added onto the front half of the build implementation pushed out all other higher priority improvements. This will move onto B14.0 stack. Additionally, a lot of these tickets may have been fixed or improved from some of the bug fixes from B13.1, but we have not had the time to come up with sufficient test data to test all the table types.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_19_ [CR] Defer Validate File Path Handling and Referential Integrity check improvements from Release Plan | [CR] Defer Validate File Path Handling and Referential Integrity check improvements from Release Plan |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_18_ [CR] Defer Registry tasks due to loss of personnel and bug fixes                                      | [CR] Defer Registry tasks due to loss of personnel and bug fixes                                      | _enter rationale for deviation from plan here_                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_17_ [CR] Defer Cloud Pilot projects to B13.1                                                              | [CR] Defer Cloud Pilot projects to B13.1                                                              | All pilot projects are being tabled until next FY when the EN Team has a better grasp of NGAP and how we are able to easily architect and deploy these applications, services, and data into NGAP.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_16_ [CR] B12.1 Defer improved handling of product versioning                                              | [CR] B12.1 Defer improved handling of product versioning                                              | Not critical yet, focused for this release on a robust v1 release of the registry and management of scalable harvesting for bigger bundles.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_15_ [CR] B12.1 Defer Registry external source integration task                                            | [CR] B12.1 Defer Registry external source integration task                                            | <!-- enter rationale for deviation from plan here -->  With `Product_Metadata_Supplemental` and accompanying CSV ingestion supported, a workaround exists for ingesting database data. More use detailed use cases needed for what data needs to be ingested and how we can support it. Additionally, other API tasks have taken precedence ([Staging vs. Operational Data](https://github.com/nasa-pds/pds-registry-app/issues/190), [Handling "deprecated" LIDs and Versions](https://github.com/nasa-pds/pds-registry-app/issues/219))                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_14_ [CR] B12.1 Defer Validate Referential Integrity Checking and Logging Improvements                     | [CR] B12.1 Defer Validate Referential Integrity Checking and Logging Improvements                     | <!-- enter rationale for deviation from plan here -->  Validate CogE retired in December causing significant delays in content validation improvements and bug fixes (https://github.com/nasa-pds/validate/issues/426). Considering content validation is a critical component ensuring a valid archive, these tasks for improvements to existing capabilities is being tabled to B13.0.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_12_ [CR] Defer Validate Configuration Improvements from B12.0                                             | [CR] Defer Validate Configuration Improvements from B12.0                                             | _enter rationale for deviation from plan here_  Depending on triaged priority of bug fixes, the tend to move towards the top of validate dev queue as they are often blockers to allowing a user to successfully validate their archives.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_11_ [CR] B12.0 Add Information Model Tasks to Release Plan                                                | [CR] B12.0 Add Information Model Tasks to Release Plan                                                | The GEOM LDD split effort is fully underway and we have pretty much dug the hole too deep at this point. Pulling back on that effort is most likely a non-starter, so we have to pivot to support that. The "B12.0 Refactoring of IMTool" effort is not critical and should not impact LDDTool for the near-term.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_7_ [CR] Defer PDS UX Tasks to B12.0                                                                       | [CR] Defer PDS UX Tasks to B12.0                                                                      | Deferring these tasks to B12.0 in order to develop a comprehensive, detailed plan, milestones, and activities for a PDS Web Modernization Team. https://github.com/nasa-pds/pds.nasa.gov-ux/issues/70                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_6_ [CR] Defer PDS API Tasks to B12.0                                                                      | [CR] Defer PDS API Tasks to B12.0                                                                     | Inaccurate estimates for time to complete other designs and implementations with PDS API WG.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_5_ [CR] Defer Tracking Service Tasks to B12.0                                                             | [CR] Defer Tracking Service Tasks to B12.0                                                            | Tracking Service design and partial implementation was completed in 2018. Misunderstanding during handoff from previous developers that the software design did not include requirements definition, and design did not form to common API standards. Caused significant increase in scope for [requirements definition task](https://github.com/nasa-pds/tracking-service/issues/2)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_4_ [CR] Add additional PDS4 SCRs to Release Plan                                                          | [CR] Add additional PDS4 SCRs to Release Plan                                                         | Several additional SCRs passed by the CCB.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_2_ [CR] Defer Validate improvements to Build 11.1                                                         | [CR] Defer Validate improvements to Build 11.1                                                        | 1. Improvement from Build 10b, [Validate Table_Character groups and their specified lengths match the specified group_length](https://github.com/NASA-PDS/validate/issues/63), had numerous ripple effects throughout the validate software, which required numerous bug fixes that used all the schedule slack for Build 11.0 delivery.       https://github.com/NASA-PDS/validate/issues/149       https://github.com/NASA-PDS/validate/issues/222       https://github.com/NASA-PDS/validate/issues/177       https://github.com/NASA-PDS/validate/issues/215       https://github.com/NASA-PDS/validate/issues/220       https://github.com/NASA-PDS/validate/issues/233       https://github.com/NASA-PDS/validate/issues/234       https://github.com/NASA-PDS/validate/issues/243       https://github.com/NASA-PDS/validate/issues/243    2. Validate expert was pulled off onto M2020 Science Data System development work. Plans to train up new "expert" for Build 11.1. |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| pds-swg_1_ [CR] Add PDS.nasa.gov-UX Tasks                                                                         | [CR] Add PDS.nasa.gov-UX Tasks                                                                        | Rationale for late planning: User Experience staff was onboarded after Release Plan was presented to SWG. That staff was responsible for identifying tasks for this work.   Rationale for tasks being included: https://docs.google.com/presentation/d/1In0Tjh1cuECCqF68D3d_fybLByDRUHwQtrlDd8cromI/edit#slide=id.g88d0673ea2_0_0                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+-------------------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

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
.. _data-upload-manager#110: https://github.com/NASA-PDS/data-upload-manager/issues/110
.. _data-upload-manager#116: https://github.com/NASA-PDS/data-upload-manager/issues/116
.. _data-upload-manager#136: https://github.com/NASA-PDS/data-upload-manager/issues/136
.. _data-upload-manager#135: https://github.com/NASA-PDS/data-upload-manager/issues/135
.. _data-upload-manager#92: https://github.com/NASA-PDS/data-upload-manager/issues/92
.. _data-upload-manager#98: https://github.com/NASA-PDS/data-upload-manager/issues/98
.. _deep-archive#162: https://github.com/NASA-PDS/deep-archive/issues/162
.. _doi-service#430: https://github.com/NASA-PDS/doi-service/issues/430
.. _harvest#131: https://github.com/NASA-PDS/harvest/issues/131
.. _harvest#127: https://github.com/NASA-PDS/harvest/issues/127
.. _harvest#158: https://github.com/NASA-PDS/harvest/issues/158
.. _monitoring#14: https://github.com/NASA-PDS/monitoring/issues/14
.. _nucleus#101: https://github.com/NASA-PDS/nucleus/issues/101
.. _pds-api#24: https://github.com/NASA-PDS/pds-api/issues/24
.. _pds-api#76: https://github.com/NASA-PDS/pds-api/issues/76
.. _pds-api#75: https://github.com/NASA-PDS/pds-api/issues/75
.. _pds-api#77: https://github.com/NASA-PDS/pds-api/issues/77
.. _pds-api#79: https://github.com/NASA-PDS/pds-api/issues/79
.. _pds-api#81: https://github.com/NASA-PDS/pds-api/issues/81
.. _pds-api#84: https://github.com/NASA-PDS/pds-api/issues/84
.. _pds-api#111: https://github.com/NASA-PDS/pds-api/issues/111
.. _pds-api#114: https://github.com/NASA-PDS/pds-api/issues/114
.. _pds-api#117: https://github.com/NASA-PDS/pds-api/issues/117
.. _pds-api#129: https://github.com/NASA-PDS/pds-api/issues/129
.. _pds-api#180: https://github.com/NASA-PDS/pds-api/issues/180
.. _pds-api#181: https://github.com/NASA-PDS/pds-api/issues/181
.. _pds-api#230: https://github.com/NASA-PDS/pds-api/issues/230
.. _pds-api#235: https://github.com/NASA-PDS/pds-api/issues/235
.. _pds-api#274: https://github.com/NASA-PDS/pds-api/issues/274
.. _pds-api#284: https://github.com/NASA-PDS/pds-api/issues/284
.. _pds-api#130: https://github.com/NASA-PDS/pds-api/issues/130
.. _pds-api#251: https://github.com/NASA-PDS/pds-api/issues/251
.. _pds-api#213: https://github.com/NASA-PDS/pds-api/issues/213
.. _pds-api#216: https://github.com/NASA-PDS/pds-api/issues/216
.. _pds-api#214: https://github.com/NASA-PDS/pds-api/issues/214
.. _pds-api#124: https://github.com/NASA-PDS/pds-api/issues/124
.. _pds-api#209: https://github.com/NASA-PDS/pds-api/issues/209
.. _pds-api#220: https://github.com/NASA-PDS/pds-api/issues/220
.. _pds-api#164: https://github.com/NASA-PDS/pds-api/issues/164
.. _pds-api#260: https://github.com/NASA-PDS/pds-api/issues/260
.. _pds-api#121: https://github.com/NASA-PDS/pds-api/issues/121
.. _pds-api#73: https://github.com/NASA-PDS/pds-api/issues/73
.. _pds-api#259: https://github.com/NASA-PDS/pds-api/issues/259
.. _pds-api#155: https://github.com/NASA-PDS/pds-api/issues/155
.. _pds-api#257: https://github.com/NASA-PDS/pds-api/issues/257
.. _pds-api#206: https://github.com/NASA-PDS/pds-api/issues/206
.. _pds-api#215: https://github.com/NASA-PDS/pds-api/issues/215
.. _pds-api#210: https://github.com/NASA-PDS/pds-api/issues/210
.. _pds-api#196: https://github.com/NASA-PDS/pds-api/issues/196
.. _pds-api#240: https://github.com/NASA-PDS/pds-api/issues/240
.. _pds-api#262: https://github.com/NASA-PDS/pds-api/issues/262
.. _pds-api#200: https://github.com/NASA-PDS/pds-api/issues/200
.. _pds-api#199: https://github.com/NASA-PDS/pds-api/issues/199
.. _pds-api#191: https://github.com/NASA-PDS/pds-api/issues/191
.. _pds-api#139: https://github.com/NASA-PDS/pds-api/issues/139
.. _pds-api#198: https://github.com/NASA-PDS/pds-api/issues/198
.. _pds-api#225: https://github.com/NASA-PDS/pds-api/issues/225
.. _pds-api#169: https://github.com/NASA-PDS/pds-api/issues/169
.. _pds-api#51: https://github.com/NASA-PDS/pds-api/issues/51
.. _pds-api#68: https://github.com/NASA-PDS/pds-api/issues/68
.. _pds-api#67: https://github.com/NASA-PDS/pds-api/issues/67
.. _pds-api#175: https://github.com/NASA-PDS/pds-api/issues/175
.. _pds-api#133: https://github.com/NASA-PDS/pds-api/issues/133
.. _pds-api#194: https://github.com/NASA-PDS/pds-api/issues/194
.. _pds-api#217: https://github.com/NASA-PDS/pds-api/issues/217
.. _pds-api#10: https://github.com/NASA-PDS/pds-api/issues/10
.. _pds-api#41: https://github.com/NASA-PDS/pds-api/issues/41
.. _pds-api#14: https://github.com/NASA-PDS/pds-api/issues/14
.. _pds-api#17: https://github.com/NASA-PDS/pds-api/issues/17
.. _pds-api#13: https://github.com/NASA-PDS/pds-api/issues/13
.. _pds-api#34: https://github.com/NASA-PDS/pds-api/issues/34
.. _pds-api#188: https://github.com/NASA-PDS/pds-api/issues/188
.. _pds-api#43: https://github.com/NASA-PDS/pds-api/issues/43
.. _pds-api#6: https://github.com/NASA-PDS/pds-api/issues/6
.. _pds-api#47: https://github.com/NASA-PDS/pds-api/issues/47
.. _pds-api#49: https://github.com/NASA-PDS/pds-api/issues/49
.. _pds-api#183: https://github.com/NASA-PDS/pds-api/issues/183
.. _pds-api#52: https://github.com/NASA-PDS/pds-api/issues/52
.. _pds-api#202: https://github.com/NASA-PDS/pds-api/issues/202
.. _pds-api#40: https://github.com/NASA-PDS/pds-api/issues/40
.. _pds-api#108: https://github.com/NASA-PDS/pds-api/issues/108
.. _pds-api#136: https://github.com/NASA-PDS/pds-api/issues/136
.. _pds-api#4: https://github.com/NASA-PDS/pds-api/issues/4
.. _pds-api#173: https://github.com/NASA-PDS/pds-api/issues/173
.. _pds-api#154: https://github.com/NASA-PDS/pds-api/issues/154
.. _pds-api#145: https://github.com/NASA-PDS/pds-api/issues/145
.. _pds-api#110: https://github.com/NASA-PDS/pds-api/issues/110
.. _pds-api#31: https://github.com/NASA-PDS/pds-api/issues/31
.. _pds-api#8: https://github.com/NASA-PDS/pds-api/issues/8
.. _pds-api#189: https://github.com/NASA-PDS/pds-api/issues/189
.. _pds-api#5: https://github.com/NASA-PDS/pds-api/issues/5
.. _pds-api#35: https://github.com/NASA-PDS/pds-api/issues/35
.. _pds-api#12: https://github.com/NASA-PDS/pds-api/issues/12
.. _pds-api#158: https://github.com/NASA-PDS/pds-api/issues/158
.. _pds-api#140: https://github.com/NASA-PDS/pds-api/issues/140
.. _pds-api#1: https://github.com/NASA-PDS/pds-api/issues/1
.. _pds-api#172: https://github.com/NASA-PDS/pds-api/issues/172
.. _pds-api#11: https://github.com/NASA-PDS/pds-api/issues/11
.. _pds-api#112: https://github.com/NASA-PDS/pds-api/issues/112
.. _pds-api#137: https://github.com/NASA-PDS/pds-api/issues/137
.. _pds-api#142: https://github.com/NASA-PDS/pds-api/issues/142
.. _pds-api#91: https://github.com/NASA-PDS/pds-api/issues/91
.. _pds4-information-model#776: https://github.com/NASA-PDS/pds4-information-model/issues/776
.. _pds4-information-model#770: https://github.com/NASA-PDS/pds4-information-model/issues/770
.. _pds4-information-model#801: https://github.com/NASA-PDS/pds4-information-model/issues/801
.. _pds4-information-model#794: https://github.com/NASA-PDS/pds4-information-model/issues/794
.. _planetary-data-cloud#108: https://github.com/NASA-PDS/planetary-data-cloud/issues/108
.. _planetary-data-engine#2: https://github.com/NASA-PDS/planetary-data-engine/issues/2
.. _planetary-data-engine#5: https://github.com/NASA-PDS/planetary-data-engine/issues/5
.. _planetary-data-engine#7: https://github.com/NASA-PDS/planetary-data-engine/issues/7
.. _planetary-data-engine#13: https://github.com/NASA-PDS/planetary-data-engine/issues/13
.. _portal-tasks#95: https://github.com/NASA-PDS/portal-tasks/issues/95
.. _registry#292: https://github.com/NASA-PDS/registry/issues/292
.. _registry#276: https://github.com/NASA-PDS/registry/issues/276
.. _registry-api#505: https://github.com/NASA-PDS/registry-api/issues/505
.. _registry-api#431: https://github.com/NASA-PDS/registry-api/issues/431
.. _registry-api#435: https://github.com/NASA-PDS/registry-api/issues/435
.. _registry-api#469: https://github.com/NASA-PDS/registry-api/issues/469
.. _registry-api#485: https://github.com/NASA-PDS/registry-api/issues/485
.. _registry-api#434: https://github.com/NASA-PDS/registry-api/issues/434
.. _registry-api#497: https://github.com/NASA-PDS/registry-api/issues/497
.. _registry-api#511: https://github.com/NASA-PDS/registry-api/issues/511
.. _registry-api#484: https://github.com/NASA-PDS/registry-api/issues/484
.. _registry-api#516: https://github.com/NASA-PDS/registry-api/issues/516
.. _registry-api#494: https://github.com/NASA-PDS/registry-api/issues/494
.. _registry-api#488: https://github.com/NASA-PDS/registry-api/issues/488
.. _registry-api#486: https://github.com/NASA-PDS/registry-api/issues/486
.. _registry-api#487: https://github.com/NASA-PDS/registry-api/issues/487
.. _registry-api#436: https://github.com/NASA-PDS/registry-api/issues/436
.. _registry-client#3: https://github.com/NASA-PDS/registry-client/issues/3
.. _registry-common#50: https://github.com/NASA-PDS/registry-common/issues/50
.. _registry-common#53: https://github.com/NASA-PDS/registry-common/issues/53
.. _registry-legacy-solr#93: https://github.com/NASA-PDS/registry-legacy-solr/issues/93
.. _registry-legacy-solr#76: https://github.com/NASA-PDS/registry-legacy-solr/issues/76
.. _registry-mgr#78: https://github.com/NASA-PDS/registry-mgr/issues/78
.. _registry-sweepers#112: https://github.com/NASA-PDS/registry-sweepers/issues/112
.. _roundup-action#138: https://github.com/NASA-PDS/roundup-action/issues/138
.. _roundup-action#139: https://github.com/NASA-PDS/roundup-action/issues/139
.. _s3-browser-cloudfront#22: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/22
.. _s3-browser-cloudfront#68: https://github.com/NASA-PDS/s3-browser-cloudfront/issues/68
.. _search-ui-legacy#30: https://github.com/NASA-PDS/search-ui-legacy/issues/30
.. _software-issues-repo#76: https://github.com/NASA-PDS/software-issues-repo/issues/76
.. _software-issues-repo#86: https://github.com/NASA-PDS/software-issues-repo/issues/86
.. _software-issues-repo#98: https://github.com/NASA-PDS/software-issues-repo/issues/98
.. _validate#249: https://github.com/NASA-PDS/validate/issues/249
.. _validate#250: https://github.com/NASA-PDS/validate/issues/250
.. _validate#317: https://github.com/NASA-PDS/validate/issues/317
.. _validate#318: https://github.com/NASA-PDS/validate/issues/318
.. _validate#409: https://github.com/NASA-PDS/validate/issues/409
.. _validate#414: https://github.com/NASA-PDS/validate/issues/414
.. _validate#426: https://github.com/NASA-PDS/validate/issues/426
.. _validate#481: https://github.com/NASA-PDS/validate/issues/481
.. _validate#496: https://github.com/NASA-PDS/validate/issues/496
.. _validate#498: https://github.com/NASA-PDS/validate/issues/498
.. _validate#534: https://github.com/NASA-PDS/validate/issues/534
.. _validate#557: https://github.com/NASA-PDS/validate/issues/557
.. _validate#578: https://github.com/NASA-PDS/validate/issues/578
.. _validate#606: https://github.com/NASA-PDS/validate/issues/606
.. _validate#607: https://github.com/NASA-PDS/validate/issues/607
.. _validate#610: https://github.com/NASA-PDS/validate/issues/610
.. _validate#629: https://github.com/NASA-PDS/validate/issues/629
.. _validate#695: https://github.com/NASA-PDS/validate/issues/695
.. _validate#816: https://github.com/NASA-PDS/validate/issues/816
.. _validate#817: https://github.com/NASA-PDS/validate/issues/817
.. _validate#822: https://github.com/NASA-PDS/validate/issues/822
.. _validate#823: https://github.com/NASA-PDS/validate/issues/823
.. _validate#824: https://github.com/NASA-PDS/validate/issues/824
.. _validate#826: https://github.com/NASA-PDS/validate/issues/826
.. _validate#831: https://github.com/NASA-PDS/validate/issues/831
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
.. _validate#833: https://github.com/NASA-PDS/validate/issues/833
.. _validate#822: https://github.com/NASA-PDS/validate/issues/822
.. _validate#823: https://github.com/NASA-PDS/validate/issues/823
.. _validate#824: https://github.com/NASA-PDS/validate/issues/824
.. _validate#826: https://github.com/NASA-PDS/validate/issues/826
.. _validate#837: https://github.com/NASA-PDS/validate/issues/837
.. _validate#849: https://github.com/NASA-PDS/validate/issues/849
.. _validate#857: https://github.com/NASA-PDS/validate/issues/857
.. _validate#860: https://github.com/NASA-PDS/validate/issues/860
.. _validate#857: https://github.com/NASA-PDS/validate/issues/857
.. _validate#861: https://github.com/NASA-PDS/validate/issues/861
.. _validate#861: https://github.com/NASA-PDS/validate/issues/861
.. _validate#873: https://github.com/NASA-PDS/validate/issues/873
.. _validate#874: https://github.com/NASA-PDS/validate/issues/874
.. _validate#880: https://github.com/NASA-PDS/validate/issues/880
.. _validate#902: https://github.com/NASA-PDS/validate/issues/902
.. _validate#903: https://github.com/NASA-PDS/validate/issues/903
.. _validate#905: https://github.com/NASA-PDS/validate/issues/905
.. _validate#915: https://github.com/NASA-PDS/validate/issues/915
.. _validate#919: https://github.com/NASA-PDS/validate/issues/919
.. _validate#923: https://github.com/NASA-PDS/validate/issues/923
.. _validate#933: https://github.com/NASA-PDS/validate/issues/933
.. _validate#936: https://github.com/NASA-PDS/validate/issues/936
.. _validate#949: https://github.com/NASA-PDS/validate/issues/949
.. _validate#178: https://github.com/NASA-PDS/validate/issues/178
.. _validate#327: https://github.com/NASA-PDS/validate/issues/327
.. _validate#294: https://github.com/NASA-PDS/validate/issues/294
.. _validate#754: https://github.com/NASA-PDS/validate/issues/754
.. _validate#401: https://github.com/NASA-PDS/validate/issues/401
.. _validate#209: https://github.com/NASA-PDS/validate/issues/209
.. _validate#473: https://github.com/NASA-PDS/validate/issues/473
.. _validate#593: https://github.com/NASA-PDS/validate/issues/593
.. _validate#516: https://github.com/NASA-PDS/validate/issues/516
.. _validate#439: https://github.com/NASA-PDS/validate/issues/439
.. _validate#690: https://github.com/NASA-PDS/validate/issues/690
.. _validate#854: https://github.com/NASA-PDS/validate/issues/854
.. _validate#364: https://github.com/NASA-PDS/validate/issues/364
.. _validate#2: https://github.com/NASA-PDS/validate/issues/2
.. _validate#298: https://github.com/NASA-PDS/validate/issues/298
.. _validate#761: https://github.com/NASA-PDS/validate/issues/761
.. _validate#419: https://github.com/NASA-PDS/validate/issues/419
.. _validate#469: https://github.com/NASA-PDS/validate/issues/469
.. _validate#781: https://github.com/NASA-PDS/validate/issues/781
.. _validate#334: https://github.com/NASA-PDS/validate/issues/334
.. _validate#71: https://github.com/NASA-PDS/validate/issues/71
.. _validate#723: https://github.com/NASA-PDS/validate/issues/723
.. _validate#431: https://github.com/NASA-PDS/validate/issues/431
.. _validate#464: https://github.com/NASA-PDS/validate/issues/464
.. _validate#739: https://github.com/NASA-PDS/validate/issues/739
.. _validate#435: https://github.com/NASA-PDS/validate/issues/435
.. _validate#748: https://github.com/NASA-PDS/validate/issues/748
.. _validate#183: https://github.com/NASA-PDS/validate/issues/183
.. _validate#153: https://github.com/NASA-PDS/validate/issues/153
.. _validate#411: https://github.com/NASA-PDS/validate/issues/411
.. _validate#326: https://github.com/NASA-PDS/validate/issues/326
.. _validate#561: https://github.com/NASA-PDS/validate/issues/561
.. _validate#519: https://github.com/NASA-PDS/validate/issues/519
.. _validate#441: https://github.com/NASA-PDS/validate/issues/441
.. _validate#461: https://github.com/NASA-PDS/validate/issues/461
.. _validate#507: https://github.com/NASA-PDS/validate/issues/507
.. _validate#514: https://github.com/NASA-PDS/validate/issues/514
.. _validate#300: https://github.com/NASA-PDS/validate/issues/300
.. _validate#297: https://github.com/NASA-PDS/validate/issues/297
.. _validate#155: https://github.com/NASA-PDS/validate/issues/155
.. _validate#335: https://github.com/NASA-PDS/validate/issues/335
.. _validate#597: https://github.com/NASA-PDS/validate/issues/597
.. _validate#356: https://github.com/NASA-PDS/validate/issues/356
.. _validate#214: https://github.com/NASA-PDS/validate/issues/214
.. _validate#173: https://github.com/NASA-PDS/validate/issues/173
.. _validate#479: https://github.com/NASA-PDS/validate/issues/479
.. _validate#6: https://github.com/NASA-PDS/validate/issues/6
.. _validate#145: https://github.com/NASA-PDS/validate/issues/145
.. _validate#234: https://github.com/NASA-PDS/validate/issues/234
.. _validate#52: https://github.com/NASA-PDS/validate/issues/52
.. _validate#611: https://github.com/NASA-PDS/validate/issues/611
.. _validate#747: https://github.com/NASA-PDS/validate/issues/747
.. _validate#427: https://github.com/NASA-PDS/validate/issues/427
.. _validate#144: https://github.com/NASA-PDS/validate/issues/144
.. _validate#372: https://github.com/NASA-PDS/validate/issues/372
.. _validate#63: https://github.com/NASA-PDS/validate/issues/63
.. _validate#554: https://github.com/NASA-PDS/validate/issues/554
.. _validate#529: https://github.com/NASA-PDS/validate/issues/529
.. _validate#531: https://github.com/NASA-PDS/validate/issues/531
.. _validate#750: https://github.com/NASA-PDS/validate/issues/750
.. _validate#844: https://github.com/NASA-PDS/validate/issues/844
.. _validate#551: https://github.com/NASA-PDS/validate/issues/551
.. _validate#72: https://github.com/NASA-PDS/validate/issues/72
.. _validate#649: https://github.com/NASA-PDS/validate/issues/649
.. _validate#499: https://github.com/NASA-PDS/validate/issues/499
.. _validate#408: https://github.com/NASA-PDS/validate/issues/408
.. _validate#328: https://github.com/NASA-PDS/validate/issues/328
.. _validate#167: https://github.com/NASA-PDS/validate/issues/167
.. _validate#273: https://github.com/NASA-PDS/validate/issues/273
.. _validate#545: https://github.com/NASA-PDS/validate/issues/545
.. _validate#299: https://github.com/NASA-PDS/validate/issues/299
.. _validate#375: https://github.com/NASA-PDS/validate/issues/375
.. _validate#203: https://github.com/NASA-PDS/validate/issues/203
.. _validate#240: https://github.com/NASA-PDS/validate/issues/240
.. _validate#511: https://github.com/NASA-PDS/validate/issues/511
.. _validate#139: https://github.com/NASA-PDS/validate/issues/139
.. _validate#11: https://github.com/NASA-PDS/validate/issues/11
.. _validate#681: https://github.com/NASA-PDS/validate/issues/681
.. _validate#562: https://github.com/NASA-PDS/validate/issues/562
.. _validate#345: https://github.com/NASA-PDS/validate/issues/345
.. _validate#146: https://github.com/NASA-PDS/validate/issues/146
.. _validate#644: https://github.com/NASA-PDS/validate/issues/644
.. _validate#257: https://github.com/NASA-PDS/validate/issues/257
.. _validate#325: https://github.com/NASA-PDS/validate/issues/325
.. _validate#9: https://github.com/NASA-PDS/validate/issues/9
.. _validate#271: https://github.com/NASA-PDS/validate/issues/271
.. _validate#763: https://github.com/NASA-PDS/validate/issues/763
.. _validate#657: https://github.com/NASA-PDS/validate/issues/657
.. _validate#368: https://github.com/NASA-PDS/validate/issues/368
.. _validate#175: https://github.com/NASA-PDS/validate/issues/175
.. _validate#361: https://github.com/NASA-PDS/validate/issues/361
.. _validate#564: https://github.com/NASA-PDS/validate/issues/564
.. _validate#336: https://github.com/NASA-PDS/validate/issues/336
.. _validate#180: https://github.com/NASA-PDS/validate/issues/180
.. _validate#190: https://github.com/NASA-PDS/validate/issues/190
.. _validate#291: https://github.com/NASA-PDS/validate/issues/291
.. _validate#378: https://github.com/NASA-PDS/validate/issues/378
.. _validate#474: https://github.com/NASA-PDS/validate/issues/474
.. _validate#453: https://github.com/NASA-PDS/validate/issues/453
.. _validate#684: https://github.com/NASA-PDS/validate/issues/684
.. _validate#673: https://github.com/NASA-PDS/validate/issues/673
.. _validate#189: https://github.com/NASA-PDS/validate/issues/189
.. _validate#165: https://github.com/NASA-PDS/validate/issues/165
.. _validate#74: https://github.com/NASA-PDS/validate/issues/74
.. _validate#8: https://github.com/NASA-PDS/validate/issues/8
.. _validate#170: https://github.com/NASA-PDS/validate/issues/170
.. _validate#349: https://github.com/NASA-PDS/validate/issues/349
.. _validate#333: https://github.com/NASA-PDS/validate/issues/333
.. _validate#381: https://github.com/NASA-PDS/validate/issues/381
.. _validate#62: https://github.com/NASA-PDS/validate/issues/62
.. _validate#379: https://github.com/NASA-PDS/validate/issues/379
.. _validate#550: https://github.com/NASA-PDS/validate/issues/550
.. _validate#392: https://github.com/NASA-PDS/validate/issues/392
.. _validate#674: https://github.com/NASA-PDS/validate/issues/674
.. _validate#220: https://github.com/NASA-PDS/validate/issues/220
.. _validate#360: https://github.com/NASA-PDS/validate/issues/360
.. _validate#631: https://github.com/NASA-PDS/validate/issues/631
.. _validate#424: https://github.com/NASA-PDS/validate/issues/424
.. _validate#5: https://github.com/NASA-PDS/validate/issues/5
.. _validate#652: https://github.com/NASA-PDS/validate/issues/652
.. _validate#33: https://github.com/NASA-PDS/validate/issues/33
.. _validate#84: https://github.com/NASA-PDS/validate/issues/84
.. _validate#614: https://github.com/NASA-PDS/validate/issues/614
.. _validate#55: https://github.com/NASA-PDS/validate/issues/55
.. _validate#206: https://github.com/NASA-PDS/validate/issues/206
.. _validate#809: https://github.com/NASA-PDS/validate/issues/809
.. _validate#204: https://github.com/NASA-PDS/validate/issues/204
.. _validate#281: https://github.com/NASA-PDS/validate/issues/281
.. _validate#533: https://github.com/NASA-PDS/validate/issues/533
.. _validate#416: https://github.com/NASA-PDS/validate/issues/416
.. _validate#301: https://github.com/NASA-PDS/validate/issues/301
.. _validate#423: https://github.com/NASA-PDS/validate/issues/423
.. _validate#380: https://github.com/NASA-PDS/validate/issues/380
.. _validate#310: https://github.com/NASA-PDS/validate/issues/310
.. _validate#37: https://github.com/NASA-PDS/validate/issues/37
.. _validate#357: https://github.com/NASA-PDS/validate/issues/357
.. _validate#376: https://github.com/NASA-PDS/validate/issues/376
.. _validate#160: https://github.com/NASA-PDS/validate/issues/160
.. _validate#260: https://github.com/NASA-PDS/validate/issues/260
.. _validate#616: https://github.com/NASA-PDS/validate/issues/616
.. _validate#256: https://github.com/NASA-PDS/validate/issues/256
.. _validate#698: https://github.com/NASA-PDS/validate/issues/698
.. _validate#480: https://github.com/NASA-PDS/validate/issues/480
.. _validate#429: https://github.com/NASA-PDS/validate/issues/429
.. _validate#201: https://github.com/NASA-PDS/validate/issues/201
.. _validate#137: https://github.com/NASA-PDS/validate/issues/137
.. _validate#366: https://github.com/NASA-PDS/validate/issues/366
.. _validate#679: https://github.com/NASA-PDS/validate/issues/679
.. _validate#432: https://github.com/NASA-PDS/validate/issues/432
.. _validate#760: https://github.com/NASA-PDS/validate/issues/760
.. _validate#548: https://github.com/NASA-PDS/validate/issues/548
.. _validate#337: https://github.com/NASA-PDS/validate/issues/337
.. _validate#693: https://github.com/NASA-PDS/validate/issues/693
.. _validate#620: https://github.com/NASA-PDS/validate/issues/620
.. _validate#671: https://github.com/NASA-PDS/validate/issues/671
.. _validate#219: https://github.com/NASA-PDS/validate/issues/219
.. _validate#447: https://github.com/NASA-PDS/validate/issues/447
.. _validate#3: https://github.com/NASA-PDS/validate/issues/3
.. _validate#107: https://github.com/NASA-PDS/validate/issues/107
.. _validate#243: https://github.com/NASA-PDS/validate/issues/243
.. _validate#475: https://github.com/NASA-PDS/validate/issues/475
.. _validate#470: https://github.com/NASA-PDS/validate/issues/470
.. _validate#99: https://github.com/NASA-PDS/validate/issues/99
.. _validate#444: https://github.com/NASA-PDS/validate/issues/444
.. _validate#576: https://github.com/NASA-PDS/validate/issues/576
.. _validate#457: https://github.com/NASA-PDS/validate/issues/457
.. _validate#785: https://github.com/NASA-PDS/validate/issues/785
.. _validate#118: https://github.com/NASA-PDS/validate/issues/118
.. _validate#503: https://github.com/NASA-PDS/validate/issues/503
.. _validate#278: https://github.com/NASA-PDS/validate/issues/278
.. _validate#177: https://github.com/NASA-PDS/validate/issues/177
.. _validate#34: https://github.com/NASA-PDS/validate/issues/34
.. _validate#544: https://github.com/NASA-PDS/validate/issues/544
.. _validate#344: https://github.com/NASA-PDS/validate/issues/344
.. _validate#233: https://github.com/NASA-PDS/validate/issues/233
.. _validate#500: https://github.com/NASA-PDS/validate/issues/500
.. _validate#212: https://github.com/NASA-PDS/validate/issues/212
.. _validate#773: https://github.com/NASA-PDS/validate/issues/773
.. _validate#1: https://github.com/NASA-PDS/validate/issues/1
.. _validate#462: https://github.com/NASA-PDS/validate/issues/462
.. _validate#605: https://github.com/NASA-PDS/validate/issues/605
.. _validate#663: https://github.com/NASA-PDS/validate/issues/663
.. _validate#741: https://github.com/NASA-PDS/validate/issues/741
.. _validate#596: https://github.com/NASA-PDS/validate/issues/596
.. _validate#662: https://github.com/NASA-PDS/validate/issues/662
.. _validate#210: https://github.com/NASA-PDS/validate/issues/210
.. _validate#415: https://github.com/NASA-PDS/validate/issues/415
.. _validate#50: https://github.com/NASA-PDS/validate/issues/50
.. _validate#63: https://github.com/NASA-PDS/validate/issues/63
.. _validate#797: https://github.com/NASA-PDS/validate/issues/797
.. _validate#316: https://github.com/NASA-PDS/validate/issues/316
.. _validate#827: https://github.com/NASA-PDS/validate/issues/827
.. _validate#164: https://github.com/NASA-PDS/validate/issues/164
.. _validate#343: https://github.com/NASA-PDS/validate/issues/343
.. _validate#556: https://github.com/NASA-PDS/validate/issues/556
.. _validate#524: https://github.com/NASA-PDS/validate/issues/524
.. _validate#658: https://github.com/NASA-PDS/validate/issues/658
.. _validate#755: https://github.com/NASA-PDS/validate/issues/755
.. _validate#535: https://github.com/NASA-PDS/validate/issues/535
.. _validate#367: https://github.com/NASA-PDS/validate/issues/367
.. _validate#599: https://github.com/NASA-PDS/validate/issues/599
.. _validate#57: https://github.com/NASA-PDS/validate/issues/57
.. _validate#476: https://github.com/NASA-PDS/validate/issues/476
.. _validate#308: https://github.com/NASA-PDS/validate/issues/308
.. _validate#388: https://github.com/NASA-PDS/validate/issues/388
.. _validate#188: https://github.com/NASA-PDS/validate/issues/188
.. _validate#241: https://github.com/NASA-PDS/validate/issues/241
.. _validate#15: https://github.com/NASA-PDS/validate/issues/15
.. _validate#149: https://github.com/NASA-PDS/validate/issues/149
.. _validate#604: https://github.com/NASA-PDS/validate/issues/604
.. _validate#617: https://github.com/NASA-PDS/validate/issues/617
.. _validate#595: https://github.com/NASA-PDS/validate/issues/595
.. _validate#683: https://github.com/NASA-PDS/validate/issues/683
.. _validate#217: https://github.com/NASA-PDS/validate/issues/217
.. _validate#482: https://github.com/NASA-PDS/validate/issues/482
.. _validate#292: https://github.com/NASA-PDS/validate/issues/292
.. _validate#303: https://github.com/NASA-PDS/validate/issues/303
.. _validate#628: https://github.com/NASA-PDS/validate/issues/628
.. _validate#651: https://github.com/NASA-PDS/validate/issues/651
.. _validate#41: https://github.com/NASA-PDS/validate/issues/41
.. _validate#23: https://github.com/NASA-PDS/validate/issues/23
.. _validate#358: https://github.com/NASA-PDS/validate/issues/358
.. _validate#17: https://github.com/NASA-PDS/validate/issues/17
.. _validate#21: https://github.com/NASA-PDS/validate/issues/21
.. _validate#26: https://github.com/NASA-PDS/validate/issues/26
.. _validate#412: https://github.com/NASA-PDS/validate/issues/412
.. _validate#29: https://github.com/NASA-PDS/validate/issues/29
.. _validate#246: https://github.com/NASA-PDS/validate/issues/246
.. _validate#24: https://github.com/NASA-PDS/validate/issues/24
.. _validate#436: https://github.com/NASA-PDS/validate/issues/436
.. _validate#707: https://github.com/NASA-PDS/validate/issues/707
.. _validate#19: https://github.com/NASA-PDS/validate/issues/19
.. _validate#230: https://github.com/NASA-PDS/validate/issues/230
.. _validate#187: https://github.com/NASA-PDS/validate/issues/187
.. _validate#254: https://github.com/NASA-PDS/validate/issues/254
.. _validate#28: https://github.com/NASA-PDS/validate/issues/28
.. _validate#90: https://github.com/NASA-PDS/validate/issues/90
.. _validate#434: https://github.com/NASA-PDS/validate/issues/434
.. _validate#197: https://github.com/NASA-PDS/validate/issues/197
.. _validate#290: https://github.com/NASA-PDS/validate/issues/290
.. _validate#135: https://github.com/NASA-PDS/validate/issues/135
.. _validate#30: https://github.com/NASA-PDS/validate/issues/30
.. _validate#322: https://github.com/NASA-PDS/validate/issues/322
.. _validate#158: https://github.com/NASA-PDS/validate/issues/158
.. _validate#51: https://github.com/NASA-PDS/validate/issues/51
.. _validate#421: https://github.com/NASA-PDS/validate/issues/421
.. _validate#608: https://github.com/NASA-PDS/validate/issues/608
.. _validate#425: https://github.com/NASA-PDS/validate/issues/425
.. _validate#20: https://github.com/NASA-PDS/validate/issues/20
.. _validate#43: https://github.com/NASA-PDS/validate/issues/43
.. _validate#65: https://github.com/NASA-PDS/validate/issues/65
.. _validate#537: https://github.com/NASA-PDS/validate/issues/537
.. _validate#31: https://github.com/NASA-PDS/validate/issues/31
.. _validate#132: https://github.com/NASA-PDS/validate/issues/132
.. _validate#238: https://github.com/NASA-PDS/validate/issues/238
.. _validate#569: https://github.com/NASA-PDS/validate/issues/569
.. _validate#124: https://github.com/NASA-PDS/validate/issues/124
.. _validate#215: https://github.com/NASA-PDS/validate/issues/215
.. _validate#7: https://github.com/NASA-PDS/validate/issues/7
.. _validate#182: https://github.com/NASA-PDS/validate/issues/182
.. _validate#643: https://github.com/NASA-PDS/validate/issues/643
.. _validate#567: https://github.com/NASA-PDS/validate/issues/567
.. _validate#601: https://github.com/NASA-PDS/validate/issues/601
.. _validate#128: https://github.com/NASA-PDS/validate/issues/128
.. _validate#355: https://github.com/NASA-PDS/validate/issues/355
.. _validate#194: https://github.com/NASA-PDS/validate/issues/194
.. _validate#64: https://github.com/NASA-PDS/validate/issues/64
.. _validate#323: https://github.com/NASA-PDS/validate/issues/323
.. _validate#222: https://github.com/NASA-PDS/validate/issues/222
.. _validate#373: https://github.com/NASA-PDS/validate/issues/373
.. _validate#47: https://github.com/NASA-PDS/validate/issues/47
.. _validate#81: https://github.com/NASA-PDS/validate/issues/81
.. _validate#374: https://github.com/NASA-PDS/validate/issues/374
.. _validate#56: https://github.com/NASA-PDS/validate/issues/56
.. _validate#264: https://github.com/NASA-PDS/validate/issues/264
.. _validate#39: https://github.com/NASA-PDS/validate/issues/39
.. _validate#133: https://github.com/NASA-PDS/validate/issues/133
.. _validate#708: https://github.com/NASA-PDS/validate/issues/708
.. _validate#42: https://github.com/NASA-PDS/validate/issues/42
.. _validate#680: https://github.com/NASA-PDS/validate/issues/680
.. _validate#195: https://github.com/NASA-PDS/validate/issues/195
.. _validate#377: https://github.com/NASA-PDS/validate/issues/377
.. _validate#87: https://github.com/NASA-PDS/validate/issues/87
.. _validate#252: https://github.com/NASA-PDS/validate/issues/252
.. _validate#50: https://github.com/NASA-PDS/validate/issues/50
.. _web-analytics#30: https://github.com/NASA-PDS/web-analytics/issues/30
.. _web-analytics#32: https://github.com/NASA-PDS/web-analytics/issues/32
.. _web-analytics#12: https://github.com/NASA-PDS/web-analytics/issues/12
.. _web-analytics#24: https://github.com/NASA-PDS/web-analytics/issues/24
.. _web-analytics#39: https://github.com/NASA-PDS/web-analytics/pull/39
.. _pds-swg_26: https://github.com/NASA-PDS/pds-swg/issues/26
.. _pds-swg_25: https://github.com/NASA-PDS/pds-swg/issues/25
.. _pds-swg_24: https://github.com/NASA-PDS/pds-swg/issues/24
.. _pds-swg_22: https://github.com/NASA-PDS/pds-swg/issues/22
.. _pds-swg_21: https://github.com/NASA-PDS/pds-swg/issues/21
.. _pds-swg_19: https://github.com/NASA-PDS/pds-swg/issues/19
.. _pds-swg_18: https://github.com/NASA-PDS/pds-swg/issues/18
.. _pds-swg_17: https://github.com/NASA-PDS/pds-swg/issues/17
.. _pds-swg_16: https://github.com/NASA-PDS/pds-swg/issues/16
.. _pds-swg_15: https://github.com/NASA-PDS/pds-swg/issues/15
.. _pds-swg_14: https://github.com/NASA-PDS/pds-swg/issues/14
.. _pds-swg_12: https://github.com/NASA-PDS/pds-swg/issues/12
.. _pds-swg_11: https://github.com/NASA-PDS/pds-swg/issues/11
.. _pds-swg_7: https://github.com/NASA-PDS/pds-swg/issues/7
.. _pds-swg_6: https://github.com/NASA-PDS/pds-swg/issues/6
.. _pds-swg_5: https://github.com/NASA-PDS/pds-swg/issues/5
.. _pds-swg_4: https://github.com/NASA-PDS/pds-swg/issues/4
.. _pds-swg_2: https://github.com/NASA-PDS/pds-swg/issues/2
.. _pds-swg_1: https://github.com/NASA-PDS/pds-swg/issues/1
.. _Software Release Summary (B15.0): https://nasa-pds.github.io/releases/15.0/index.html
.. _PDS Standalone: https://nasa-pds.github.io/releases/11.1/index.html#standalone-tools-and-libraries
.. _PDS Discipline Nodes: https://nasa-pds.github.io/releases/11.1/index.html#discipline-node-services
.. _PDS Engineering Node Only: https://nasa-pds.github.io/releases/11.1/index.html#enineering-node-services
.. _PDS Deep Archive Software Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-deep-archive/blob/master/docs/pds4_nssdca_delivery_design_20191219.docx
.. _PDS DOI Service Requirements and Design Document (SRD/SDD): https://github.com/NASA-PDS/pds-doi-service/blob/master/docs/design/pds-doi-service-srd.md